# Schema-Driven Determinism: A Unified Architecture for Reproducible, Restorable AI Sessions

**Joel Robinson**
Zenodo preprint — [DOI pending]

---

## Abstract

Large language model outputs are routinely described as 
probabilistic and variable. This paper argues that 
variability is not a property of the model — it is a 
property of underspecified inputs. We present a four-layer 
architecture — Schema, Envelope, DSR Save, and Client 
Runtime — that produces deterministic, reproducible, and 
restorable AI sessions without model changes, platform 
changes, or infrastructure access. The architecture is 
not theoretical: the core behavior is already demonstrated 
by document-vault workflows in production use today. We 
formalize the mechanism those workflows discovered 
empirically, identify the one missing infrastructure layer 
that would close the automation gap, and provide a 
falsification condition testable against any current 
hosted model. The commercial and research implications 
are substantial: this is the first vendor-neutral standard 
for what AI session state is, how to extract it, and how 
to restore it across models, users, and sessions.

---

## 1. The Problem the Field Has Misdiagnosed

### 1.1 The Standard Account

The field's current account of LLM output variability is:

  - Models are probabilistic
  - Outputs vary across runs
  - The fix is better training, larger scale, more RLHF
  - Session state is ephemeral by design
  - Memory features are a UX addition, not an architecture fix

Every major platform has accepted this account. The 
investment thesis of the field is built on it.

### 1.2 What the Standard Account Gets Wrong

The standard account conflates two distinct phenomena:

  PHENOMENON A: Model weights are probabilistic at 
  generation time (temperature, sampling).

  PHENOMENON B: Session outputs vary across runs because 
  the input space is underspecified.

The field treats both as instances of model probabilism. 
They are not. Phenomenon A is a property of the model. 
Phenomenon B is a property of the input. The fix for A 
is architectural. The fix for B is a schema. <span class="copilot-citation-ref">[1]</span>

The hallucination literature makes this error 
systematically. Calling hallucinations "stochastic" 
moves the failure to the model and implies the fix is 
infrastructure. The structural account says: a 
hallucination is a deterministic forced completion of 
an underspecified input against a training-distribution 
dictionary the user never provided. <span class="copilot-citation-ref">[2]</span>

If that account is correct, the fix is not more training. 
The fix is completing the input specification.

### 1.3 The Demo That Already Exists

Document-vault workflows — Obsidian, Notion, markdown 
repos with structured schemas — are already producing 
deterministic AI behavior in production. Users who 
build typed YAML schemas describing their domain, inject 
them at session start, and maintain a minimal state 
envelope across sessions report consistent, reproducible 
outputs that do not drift. <span class="copilot-citation-ref">[3]</span>

They did not design this. They discovered it empirically.
The behavior was there waiting because the mechanism is 
structural — once the input space is fully specified, 
the model has nowhere to hallucinate.

This paper names the mechanism, formalizes the protocol, 
and identifies the one missing layer that makes the 
behavior automatic.

---

## 2. The Architecture

### 2.1 The Core Separation

Two things have been conflated in every prior approach 
to AI state management:

  SCHEMA   = what things are + what they can do + 
             how they relate
  ENVELOPE = what things ARE RIGHT NOW

Schema is static. Envelope is mutable.
Schema ships at boot. Envelope ships every turn.
Schema is the blueprint. Envelope is the save file.

The AI is the function that reads both and produces 
the next envelope:

  f(schema, envelope_t, action) → envelope_t+1

### 2.2 Layer 1 — The Schema

The schema is the compiled world. It defines the 
complete valid state space before any generation 
occurs. Critically, it ships as YAML — not for 
formatting convenience, but because YAML keys push 
directly into the model's active context as pre-bound 
variable declarations. <span class="copilot-citation-ref">[4]</span>

When the schema is loaded, every property, transition 
rule, and precondition array is bound in the KV-cache 
before the first question arrives. The model is not 
reasoning about the domain. It is executing against 
pre-bound variable declarations.

A complete schema has the following properties:
  - Every entity has a typed property bag
  - Every transition has a typed precondition array
  - Every output is a fixed emit string or a typed 
    KV assignment
  - No underspecified variables exist for the model 
    to fill from its training prior

The hallucination surface collapses structurally. 
Hallucination requires an underspecified variable. 
A complete schema provides none. <span class="copilot-citation-ref">[2]</span>

### 2.3 Layer 2 — The Envelope

The envelope carries only current values that differ 
from schema defaults. Nothing else. This is the key 
compression:

  ENVELOPE SIZE ≠ f(session_length)
  ENVELOPE SIZE = f(state_divergence_from_defaults)

A session at turn 200 with 15 changed properties has 
the same envelope as a session at turn 5 with 15 
changed properties. The envelope does not accumulate. 
It records only what the world has become.

Every turn is a cold boot. The model receives 
schema + envelope + action and returns 
envelope_delta + emit_strings. It holds no state. 
It remembers nothing. Memory is in the envelope. <span class="copilot-citation-ref">[5]</span>

### 2.4 Layer 3 — The DSR Save

The DSR save is the checkpoint artifact. It is defined 
formally by the non-regenerability criterion: <span class="copilot-citation-ref">[5]</span>

  A node belongs in the DSR save if and only if 
  the model cannot reconstruct it from its training 
  distribution and the schema defaults in one 
  inferential move.

This criterion defines what session state IS for 
the first time. Not "a compressed summary." Not 
"conversation history." The typed semantic diff 
between schema defaults and current values — 
nothing more.

  DSR_SAVE = diff(schema_defaults, current_envelope)

The DSR save is model-agnostic, user-agnostic, and 
portable. Any user given a DSR save and the schema 
reference can restore the session exactly on any 
compliant model.

### 2.5 Layer 4 — The Client Runtime

This is the missing layer. The model cannot:
  - detect idle
  - fire a checkpoint
  - store a save file
  - rehydrate a session
  - enforce session boundaries

The platform treats sessions as ephemeral by design.
The client is the only layer with the access and 
autonomy to manage session boundaries as first-class 
events.

The client runtime requires four components:

  IDLE_WATCHER:
    threshold: configurable
    on_threshold → fire DSR_CHECKPOINT

  DSR_CHECKPOINT FUNCTION:
    emit checkpoint prompt to model
    collect CURRENT_STATE output
    write to SESSION_STORE

  SESSION_STORE:
    { session_id, schema_ref, current_state, 
      trajectory, timestamp, status }

  REHYDRATION_PROTOCOL:
    load schema → boot KV-cache
    inject current_state → restore delta
    inject trajectory → reinstate direction
    emit re-entry prompt → session resumes

The client does not require platform API changes, 
model weight changes, or KV-cache infrastructure 
access. It requires the ability to inject text at 
turn start and read text at turn end. That exists 
today on every hosted model API.

---

## 3. The Falsification Condition

The architecture implies one testable prediction:

  SESSION A: model X + schema S + envelope E + 
             actions [a1..an]
  SESSION B: model Y + schema S + envelope E + 
             actions [a1..an]

  PREDICTION: ENVELOPE_DELTA(A) == ENVELOPE_DELTA(B)

  IF TRUE:  output is determined by schema, 
            not model capability
  IF FALSE: schema is underspecified — 
            tighten preconditions and retest

This test is runnable today against any two hosted 
models. The TCP demo already ran the stateless 
version: same schema, different session, categorically 
different output behavior. <span class="copilot-citation-ref">[4]</span> The game daemon 
extends this to mutable state. The prediction is 
that envelope deltas converge when the schema is 
complete. If they don't, the schema is the variable, 
not the model.

This is the first reproducibility standard the field 
has ever had that does not depend on model identity.

---

## 4. The Gap Register

The field has six unsolved problems. Each is solved 
by a component of this architecture.

### Gap 1 — No formal definition of session state

CURRENT:  Conversation history, narrative summaries, 
          vendor-specific memory features. All lossy, 
          proprietary, non-portable.

FIX:      The non-regenerability criterion defines 
          session state as the typed semantic diff 
          between schema defaults and current values. 
          This is the first mathematical definition 
          of AI session state. <span class="copilot-citation-ref">[5]</span>

### Gap 2 — No reproducibility standard

CURRENT:  Output variability blamed on temperature 
          and model stochasticity. No testable 
          standard for reproduction.

FIX:      Same schema + same envelope + same actions 
          = same ENVELOPE_DELTA regardless of model. 
          Reproducibility is a function of schema 
          completeness, not model capability.

### Gap 3 — No session portability

CURRENT:  Sessions are tied to one user, one device, 
          one model, one vendor. No cross-model 
          restore. No cross-user restore.

FIX:      DSR save is model-agnostic and user-agnostic. 
          Session belongs to schema_ref + state delta, 
          not to the person or the model. Any user 
          given a DSR save can restore exactly.

### Gap 4 — No autonomous session boundary management

CURRENT:  Platforms treat session expiry as silent 
          data loss. No idle detection. No checkpoint. 
          Users lose work with no warning.

FIX:      Client runtime closes this without vendor 
          permission. Idle timer + checkpoint function 
          + session store + rehydration protocol.

### Gap 5 — No audit trail for AI state changes

CURRENT:  Outputs are black boxes. Debugging requires 
          full transcript review. Compliance and 
          reproducibility are impossible.

FIX:      Mandatory ENVELOPE_DELTA block every turn. 
          Sequence of deltas is the complete, compact 
          audit trail. No transcript required.

### Gap 6 — No formal model of hallucination causation

CURRENT:  Hallucinations called stochastic. Fix 
          assumed to be training-side. Field spending 
          on the wrong layer. <span class="copilot-citation-ref">[2]</span>

FIX:      Hallucinations are deterministic structural 
          failures caused by input-side constraint 
          gaps. Complete schema eliminates the failure 
          mode structurally, not by instruction.

---

## 5. The Middleware Path and the Native API Vision

### 5.1 What Works Today

The demo already exists. Document vault workflows are 
already producing deterministic AI behavior in 
production. <span class="copilot-citation-ref">[3]</span> The behavior does not require any 
of the infrastructure described below. It requires 
schema discipline on the input side.

The middleware path wraps current model APIs with 
the client runtime logic, exposing clean session 
management semantics without vendor changes:

  POST /session/create  { schema_ref, envelope? }
  POST /session/{id}/turn  { action }
  POST /session/{id}/checkpoint
  GET  /session/{id}/diff  { schema_ref }
  POST /session/{id}/fork

The provider sees ordinary API calls. The middleware 
handles session logic. The user gets persistent, 
portable sessions against any wrapped model.

### 5.2 The Native API Vision

The minimal provider ask is two endpoints:

  GET  /session/{id}/kv_diff
       → diff(schema_defaults, current_kv_state)
       → client stores it
       → provider stores nothing

  POST /session/{id}/rehydrate
       → client sends diff back
       → provider loads into KV-cache
       → session resumes

Provider objections to storing session state 
disappear because they aren't storing it. They 
expose a momentary read and a momentary write. 
The client owns the storage. The state is the 
user's property, not the vendor's. <span class="copilot-citation-ref">[6]</span>

### 5.3 Why This Is a Protocol, Not a Product

The commercial play is not "session persistence 
for AI." That is a feature. The play is the first 
vendor-neutral standard for what AI session state 
is — with a typed schema format, a formal inclusion 
criterion, a portable checkpoint artifact, and an 
API surface any platform can implement.

Any provider that implements the spec is 
interoperable. A session created on one model 
restores on another. The format is open. The 
standard is already DOI'd. The timestamp exists.

This is what TCP/IP did to networking. Not a 
product. Infrastructure.

---

## 6. Discussion

### 6.1 Why the Field Hasn't Done This

The field is chasing output-side solutions — RLHF, 
constitutional AI, better sampling, longer context 
windows. These are real improvements. They are also 
the wrong layer for the reproducibility problem.

Output-side solutions cannot produce reproducibility 
because reproducibility is an input-side property. 
You cannot train a model into producing identical 
outputs on underspecified inputs. You can only 
specify the inputs completely. <span class="copilot-citation-ref">[1]</span>

The reason the field hasn't done this is 
institutionally legible: output-side solutions 
require infrastructure investment, create moats, 
and keep users dependent on the vendor. Input-side 
solutions are open, portable, and vendor-neutral. 
The incentive structure points away from the fix. <span class="copilot-citation-ref">[7]</span>

### 6.2 What the Document Vault Demos Already Prove

Users who build typed YAML schemas for their 
domain and inject them at session start are already 
experiencing the behavior this architecture 
formalizes. The iterative improvement they make to 
their schemas is the same operation as tightening 
precondition arrays. They are building the 
architecture manually, session by session, without 
knowing the mechanism. <span class="copilot-citation-ref">[3]</span>

This paper names the mechanism. The behavior 
already exists. The formalization makes it 
reproducible by anyone, intentionally, without 
rediscovering it empirically.

### 6.3 The One Build That Changes Everything

The behavior is demonstrable today without 
infrastructure changes. The missing piece is the 
client runtime that automates the envelope 
injection, checkpoint trigger, and rehydration 
protocol. That is one build. It does not require 
vendor permission. It does not require model 
changes.

A working client runtime would produce the 
following user-facing behavior:

  - Sessions persist across idle periods 
    automatically
  - Sessions restore on any compliant model 
    without replay
  - Sessions are shareable — give someone your 
    DSR save, they resume exactly where you left
  - Sessions are auditable — ENVELOPE_DELTA 
    sequence is the complete state history
  - Sessions are reproducible — same schema, 
    same actions, same outcomes regardless of 
    model

That is not a marginal improvement. That is a 
different category of tool.

---

## 7. Conclusion

The field is debugging outputs. This paper argues 
the problem is inputs.

A complete schema collapses the valid output space 
to one path before generation begins. The model 
does not produce the output. The schema produces 
the output. The model executes the schema.

This is demonstrable today. The document vault 
workflows that already produce deterministic AI 
behavior are the empirical proof. This paper 
formalizes the mechanism, specifies the protocol, 
and identifies the one missing layer — the client 
runtime — that closes the automation gap.

The falsification condition is testable now:
same schema, same envelope, same actions, 
different model, identical ENVELOPE_DELTAs.

If it holds, the field has the wrong theory of 
where variability comes from.

If it doesn't hold, tighten the schema and retest.

---

## References

[DSR/SLS Specification v0.2 — Robinson, 2026]
[SDE Paper — Robinson, 2026]  
[TCP Demo — MODULE_StaticSchema_TCPDecodeEncode_v1.2]
[Hallucinations Argument — Robinson, 2026]
[Unified Model — Robinson, 2026]