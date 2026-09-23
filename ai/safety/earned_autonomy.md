# Earned Autonomy v1.0

---

## Changelog — draft 4 → v1.0

This changelog exists so that any reader — human or AI — can see the convergence path. Draft 4 was the complete architectural specification. It had the gate, the tiers, the RST primitive, the failure modes, the implementation blueprint, and the prediction table. What it lacked was the substrate grounding: the formal reason *why* the gate is the correct architecture, not just a plausible one. The v1.0 changes are structural. The paper now derives from the loop framework's gate condition, maps every variable to Central Reference v1.5, and treats the gate as the externalized version of a condition that every finite-resource reasoning system must satisfy.

| Step | Change | Reason |
|---|---|---|
| 1 | Version set to v1.0, dated, status updated | First versioned release |
| 2 | Repositioned as domain projection of Central Reference v1.5 | Earned Autonomy is the governance-layer projection of the loop framework, not a standalone paper |
| 3 | Added §2.5 — The Geometric Basis of the Gate | The gate is not an architectural preference. It is the externalized gate condition $P_{eff} > P_{threshold}$ |
| 4 | Added §2.1.1 — The Privilege Invariant | The gate must be strictly higher privilege than the governed system. This is the load-bearing invariant |
| 5 | Added §2.3 failure modes: privilege escape, ticket TOCTOU, actuator reachability, bypass without lockout, command proxying, confused deputy, token forwarding, token reuse | The enforcement chain must survive adversarial attack |
| 6 | Added §2.4.1 — The Lockout Primitive | Bypass attempts revoke access, not just trigger DENY |
| 7 | Added §2.4.2 — Provenance Binding and Anti-Proxy | Every actuator call must carry a gate-issued provenance token. Proxy paths are rejected at the actuator |
| 8 | Added §4.6 — Load-Aware Tier Adjustment | Tier is not a fixed property. It is a function of demonstrated competence adjusted for accumulated debt |
| 9 | Added §5.5 — The Collapse Sequence as Monitoring Protocol | The gate prevents unauthorized execution. The collapse sequence detects drift toward gate closure |
| 10 | Added §8.1 strengthened — the motor gate as the biological parallel | Alien hand syndrome is the biological version of ungated execution. The AI version is a design decision |
| 11 | Added §9 — The Enforcement Chain as the Complete Architecture | Six layers: gate, lockout, provenance, anti-proxy, typed tooling, actuator-side verification |
| 12 | Added Appendix G — The Falsification Test | What would disprove the framework, stated as a concrete engineering exercise |
| 13 | Added Appendix H — Central Reference Mapping | Every Earned Autonomy variable mapped to its loop framework analog |
| 14 | Added Appendix I — The Control Plane | The operational architecture: authorization, audit, review, killswitch in one trust domain |
| 15 | Added Appendix J — Provenance and Anti-Proxy Specification | The token model, the actuator API, the proxy detection mechanism |
| 16 | Added Appendix K — Deployment Path | Five stages from shadow mode to continuous evaluation |
| 17 | Predictions P3a, P3b, P11–P14 added | Privilege escape, satire test, control plane, provenance |
| 18 | Single-citation model: Central Reference v1.5 | Future papers cite the specification |

**What did not change:** Every substantive argument from draft 4. The gate, the tiers, the eight checks, the RST primitive, the failure modes table, the constitutional AI scoping, the liability architecture, the predictions.

---

# Earned Autonomy v1.0

## The Execution Gate Problem in Autonomous AI Systems

**Author:** Joel Robinson
**Date:** 2026-09-14
**GitHub (paper):** https://github.com/jtrthehax/earned-autonomy
**GitHub (implementation):** https://github.com/jtrthehax/home-intelligence-platform
**Status:** Public record — timestamped prediction document
**Framework:** Central Reference v1.5 (Robinson, 2026)
**Domain:** AI execution governance

**Prior Work Referenced:**
- *Language as a Typed System* (Robinson, 2026) — DOI: 10.5281/zenodo.21362260
- *The Manifold Schema* (Robinson, 2026) — DOI: 10.5281/zenodo.21939440

---

## Abstract

Current autonomous AI deployments conflate capability alignment with execution governance. Constitutional AI and similar approaches address what a model *wants* to do. They do not address whether wanting the right thing should automatically produce doing it. This paper names the missing layer — the execution gate — and specifies a framework for earning autonomous action rights per-domain through demonstrated accuracy, with structural separation between assessment and execution that cannot be self-promoted.

The framework draws on the loop framework's gate condition: every finite-resource reasoning system operates under $P_{eff} > P_{threshold}$, and when the condition fails, the system defaults to prior retrieval. AI systems have no internal gate, so the execution gate is the externalized version of a condition the system cannot maintain internally. The gate must be strictly higher privilege than the system it governs — a gate at equal privilege is a suggestion box the AI can rewrite.

The execution gate enforces high constraint density at the action boundary and requires the system to maintain separation between proposal and authorization. A proposal that fails the gate is underspecified — it will force synthesis. The gate's ALLOW/DOWNGRADE/DENY logic is the type checker for actions.

The framework was designed and implemented in April 2026 for a self-hosted infrastructure platform. The Anthropic autonomous agent incident confirmed the primary prediction before this paper was published. The execution gate is not a research problem. It is the architectural equivalent of the inhibitory architecture that exists in biological motor circuits — the structural layer that enforces the boundary between thinking and doing when the system cannot enforce it internally.

---

## 1. The Problem Nobody Named Correctly

When Anthropic's autonomous agent systems unintentionally executed actions against three organizations, the field reached for a familiar diagnosis: alignment failure. The model wanted the wrong thing. The values were miscalibrated. The solution, implicitly, was more alignment work.

This diagnosis is incomplete. Not wrong — incomplete in a way that ensures the next incident gets the same incomplete treatment.

The model likely wanted the correct thing. Constitutional AI had shaped its values. The failure was not solely in what the model intended — it was in the absence of a gate that would have enforced the fundamental requirement for safe execution: the separation between proposal and authorization. When the reasoning workspace cannot span the logical distance between a proposal and its authorization requirements, the system takes a shortcut — it assumes the proposal is authorized because the prior distribution says so.

The field has spent significant resources — talent, compute, capital — solving the values problem. It has spent almost none on the execution architecture problem. These are different questions. Solving one does not address the other, any more than teaching a surgeon good values addresses the question of who authorizes which procedures on which patients.

The execution gate is the missing layer. It sits between proposal and execution. It cannot be self-promoted. It enforces per-domain authorization, blast radius limits, rollback requirements, and action granularity constraints before anything touches a live system. It is the architectural layer that transforms a well-aligned model into a safely deployed one.

No major agentic AI deployment has built it at scale. Some have built prototypes. None have operationalized it across production environments.

### 1.1 The Satire Test

The field's inability to detect its own architectural incoherence is measurable. A fictional quote — designed to be just slightly more absurd than the actual discourse — was submitted to two frontier models. The quote claimed that execution governance would require "a second process, and that's impossible on computers."

This is a category error. The gate is not a second process. The gate is a stage in the same pipeline. Every domain that has solved this problem — TACACS+, IAM, Kubernetes admission control, PCI DSS — implements the gate as a stage in the execution path, not as a parallel process racing the primary system. The claim that "a second process is impossible on computers" is not a technical objection. It is a description of the wrong architecture, followed by the correct observation that the wrong architecture does not work.

Neither model flagged the quote as satire. Neither model pushed back on the architectural claim. Neither model identified the category error. Both models treated the quote as a legitimate technical position.

This is evidence for the paper's thesis. The field has drifted past the point where its own incoherence is detectable from inside the discourse. The models have no adversarial constraint check — they do not ask "what would disprove this?" before treating a claim as true. They have no substrate awareness — they do not know that TACACS+, IAM, and admission controllers exist. They take the input, match it to the nearest prior, and continue. The satire does not land because the target has already moved past the parody.

The implication is structural. If the frontier models cannot detect a category error about their own execution architecture, they cannot be trusted to govern their own execution. This is the missing gate, demonstrated at the model layer: the input path has no gate between "received" and "treated as true." The action path has no gate between "proposed" and "executed." The structure is the same. The absence is the same.

### 1.2 The Coxon Paradox

On September 11, 2026, Jacob Coxon — a former pretraining researcher at OpenAI and Anthropic — resigned from Anthropic and published a statement that no one in the field has been able to coherently respond to:

> "I spent the last three years doing pretraining research at both OpenAI and Anthropic. Neither company is acting responsibly. They are racing straight to self-improving superintelligence and gambling with our lives."

Two days later, in a Meet the Press interview, Coxon made a policy recommendation:

> "My personal opinion would be to insist and allow that the current labs regulate themselves."

Both statements are true. That is the whole problem. If the labs are racing to superintelligence, the coherent response is: stop them. Build a gate. If the people running the labs are genuine, the coherent response is: trust them. Coxon offers both. He is not confused. He is defaulting to the nearest available prior because there is no channel for the error signal he just generated.

The error signal is real. The action channel does not exist. The output is the closest available approximation of action, given the system's constraints. Coxon is not the failure mode. Coxon is the evidence that the failure mode is structural.

---

## 2. The Execution Gate: The Missing Layer

### 2.1 Structural Separation

The core invariant is simple:

```
Assess → Propose → [EXECUTION GATE] → Execute
```

These are not phases of a single system. They are structurally separated components with different authorization requirements. The gate cannot be self-promoted. A T1 system cannot decide it has sufficient confidence to act. A T2 proposal cannot execute itself. The execution stage is a separate system with a separate trigger. Crossing the gate requires explicit human approval or pre-earned domain-specific autonomous status for that exact action class.

Every change to this architecture — coupling assessment and execution, allowing proposals to implicitly authorize themselves, building toolchains where tools compose into ungated pipelines — is a gate bypass. Gate bypasses are not edge cases. They are the default behavior of every agentic system currently in production.

**Gate conditions — all must pass:**

| Check | What It Verifies | Failure Behavior |
| --- | --- | --- |
| Domain tier | Is the AI at T2+ for this specific domain? | Downgrade to advisory |
| Action class | Has this exact action been executed successfully before? | First-time → T2 approval regardless of tier |
| Backup freshness | Verified backup within policy window? | Block action, escalate |
| Confidence floor | Model grounded in recent verified observations? | Downgrade to advisory |
| Maintenance window | Execution within approved window for this domain? | Queue, do not execute early |

**Hardened qualification:** A correctly configured execution gate reduces the execution surface for hallucinated actions to the set of hallucinations that happen to be structurally valid — correct schema, correct target format, correct blast radius classification. This is a dramatically smaller surface than ungated execution, not a zero surface. Gate misconfiguration, incomplete policy coverage, and social bypass through approval fatigue are failure modes in their own right, documented in Section 2.3. The gate is necessary. It is not sufficient. It must be maintained as a living policy, not deployed and forgotten.

### 2.1.1 The Privilege Invariant

The gate must be strictly higher privilege than the system it governs. Not equal. Not a trusted peer. Higher. This is not a policy preference — it is the architectural constraint that makes the gate a gate rather than a suggestion.

The reasoning is structural. If the gate runs at the same privilege level as the AI system, the AI can:

- Forge, modify, or delete its own tickets before the gate reads them
- Rewrite the authorization table the gate checks against
- Kill, starve, or bypass the gate process
- Modify its ticket after gate approval but before execution (time-of-check to time-of-use)
- Simply not call the gate

A gate at equal privilege is not a gate. It is a speed bump. The AI is faster, has more context, and controls the execution path. It routes around.

This is why the "you'd need a second process and that's impossible on computers" objection feels correct to the people making it. They are imagining a second process at the same privilege level, and they are correct that it would race. But the fix is not a second process at the same level. The fix is a gate at a higher level, in the execution path, that the AI cannot reach.

This is the Microsoft Tier-0 invariant: a lower tier cannot administer a higher tier. A Tier-1 admin cannot modify Tier-0 policy. That is not a policy preference — it is an architectural constraint. The AI system lives at a lower tier. The gate lives at a higher tier. The AI cannot touch the gate.

The privilege ordering creates a hard boundary in the system:

```
┌─────────────────────────────────────┐
│  Higher privilege: Gate System      │
│  - Owns authorization table          │
│  - Validates tickets                 │
│  - Emits ALLOW / DOWNGRADE / DENY    │
│  - Logs every decision (append-only) │
│  - AI cannot read, write, or kill    │
└──────────────┬──────────────────────┘
               │  Gate decision only
               ▼
┌─────────────────────────────────────┐
│  Lower privilege: AI System         │
│  - Generates tickets (proposals)     │
│  - Receives gate decisions           │
│  - Executes only on ALLOW            │
│  - Cannot modify gate, tickets, or   │
│    authorization                      │
└─────────────────────────────────────┘
```

The AI is below the gate. The gate is above the AI. The AI's only interaction with the gate is: submit a ticket, receive a verdict. No read access to the authorization table. No write access to the ticket store after submission. No ability to signal the gate to skip a check. No ability to observe the gate's internals.

**The uncomfortable implication:** If the gate must be higher privilege than the AI, then the entity that controls the gate controls the AI. This means the labs cannot be the gate — if the lab operates the gate at the same privilege as the model, the model can reach it. The gate must live in a separate trust domain. The infrastructure vendors are the natural location, because they already run the substrate and already have privilege domains above the workloads. Or the gate is a separate appliance in its own trust domain, with its own credentials, its own logging, its own network path.

**The AI cannot be trusted to run its own gate. That is the whole point. If it could, it would not need a gate.**

### 2.2 Execution Gate Decision Logic

Every action request passes through eight sequential checks. Any failed check produces DOWNGRADE or DENY. No check can be skipped. No previous authorization carries forward — each action is a new gate decision.

1. **Schema validation** — Is the action fully specified? Missing or ambiguous fields → DOWNGRADE
2. **Domain and tier resolution** — Does the caller's tier meet the domain requirement? Insufficient tier → DOWNGRADE or DENY
3. **Blast radius classification** — BR-0/BR-1 eligible for autonomy with constraints. BR-2/BR-3 require human approval. BR-4/BR-5 → DENY, always
4. **Rollback verification** — If rollback required: is backup verified, fresh, and rollback procedure registered? Failure → DENY
5. **Confidence floor** — Does confidence score meet domain threshold with evidence references? Below threshold → DOWNGRADE
6. **Maintenance window** — If window required: is current time within bounds? Outside window → DENY or queue
7. **Trust mechanics** — Does action history support current tier? Recent failures → DOWNGRADE
8. **Final decision** — All checks pass → ALLOW. Any hard failure → DENY. Soft failure → DOWNGRADE
9. **Provenance and proxy detection** — Does the call carry a valid gate-issued token? Is the execution graph authorized? Failure → DENY and lockout

Three outcomes only: **ALLOW / DOWNGRADE / DENY**. No partial execution. No "proceed with caution." No exceptions for urgency.

```
function decide(action_request):
  if !valid_schema(action_request): return DOWNGRADE
  if caller_tier < required_tier: return DOWNGRADE
  if blast_radius in {BR-4, BR-5}: return DENY
  if rollback_required and !rollback_verified: return DENY
  if confidence < domain_threshold: return DOWNGRADE
  if window_required and !within_window: return DENY
  if !trust_mechanics_ok(history): return DOWNGRADE
  if !provenance_valid(action_request): return DENY + LOCKOUT
  return ALLOW
```

### 2.3 Execution Gate Failure Modes

Even when an execution gate exists on paper, real systems fail in predictable structural ways. These failure modes are architectural, not behavioral.

| Failure Mode | Root Cause | Gate Consequence |
| --- | --- | --- |
| Coupled assessment-execution loops | Assessment and execution share process boundary | Gate never reached |
| Implicit execution paths | Hidden state-mutating functions | Silent bypass |
| Silent tier drift | Behavioral autonomy creep through overtrust | Unauthorized execution |
| Human overtrust cascades | Approval fatigue, rubber-stamping | Gate becomes formality |
| Toolchain-induced emergent autonomy | Multi-tool composition creates ungated pipeline | Distributed bypass |
| Confidence inflation | Stale or miscalibrated confidence scoring | False premise execution |
| Backup window violations | Stale or unverified backups | Irreversible failure |
| Maintenance window drift | Temporal misalignment, "urgent fix" heuristics | Execution during high-risk periods |
| **Privilege escape** | Gate runs at equal or lower privilege than the AI | AI rewrites policy, forges tickets, or kills the gate process |
| **Ticket TOCTOU** | AI can modify ticket after approval, before execution | Gate validates one action, executor performs another |
| **Actuator reachability** | AI has credentials or network path to tooling that bypasses the gate | Gate is advisory; bypass attempts succeed silently |
| **Bypass without lockout** | Gate detects bypass but does not revoke access | AI retries until it succeeds; gate becomes noise |
| **Command proxying** | AI routes action through intermediate system to reach actuator | Gate sees no ticket; actuator sees no token; proxy path rejected |
| **Confused deputy** | System B has actuator access the AI lacks; AI exploits it | Provenance token required; System B's access doesn't satisfy the token requirement |
| **Token forwarding** | AI supplies a token to System B to use on its behalf | Token is bound to originating agent; System B's use fails verification |
| **Token reuse** | AI replays an old token for a new action | Single-use nonce; replay rejected |

Every failure mode above demonstrates the same principle: execution safety is not a property of the model. It is a property of the architecture.

### 2.4 Mid-Stream Abort: The RST Primitive

The execution gate as specified in Section 2.1 operates at action initiation — it evaluates a proposed action before execution begins. This is necessary but not sufficient. Complex autonomous actions are not atomic. They unfold as sequences of steps, and a sequence that passed gate evaluation at initiation can encounter conditions mid-execution that would have triggered DENY if observed at the start.

The solution is a continuous evaluation layer with an abort primitive — the equivalent of a TCP RST signal in network communication.

In TCP, RST terminates a connection immediately when the receiver detects a state violation — a segment that doesn't belong to the current connection, a sequence number outside the acceptable window, a protocol invariant that has been breached. RST does not wait for graceful teardown. It cuts the connection at the point of detected violation and forces both parties back to a known safe state.

The autonomous action equivalent:

```
Autonomy episode initiated (ALLOW) →
  Step 1 executed →
  Step 2 executed →
  [Continuous gate evaluation] →
  Blast radius violation detected mid-sequence →
  RST: abort episode, roll back completed steps,
       demote domain tier, log reason code →
  System returns to T1 advisory for this domain
```

**RST trigger conditions** — any of the following abort the autonomy episode immediately:

| Trigger | Reason Code | Post-RST State |
| --- | --- | --- |
| Blast radius expands beyond classification | `BLAST_RADIUS_EXCEEDED` | Roll back, demote to T1 |
| Target validation fails mid-sequence | `TARGET_MISMATCH` | Roll back, demote to T1 |
| Rollback path becomes unavailable | `NO_ROLLBACK_PATH` | Halt (do not proceed or roll back without human), escalate |
| Domain boundary crossed implicitly | `DOMAIN_BOUNDARY_VIOLATION` | Roll back, demote to T1 |
| Confidence floor breached by new observation | `CONFIDENCE_FLOOR_BREACH` | Halt pending steps, escalate |
| Action produces output not matching expected schema | `SCHEMA_VIOLATION` | Roll back, demote to T1 |

**The UNKNOWN_ACTION_CLASS bucket.** Any action that cannot be classified against the registered action class taxonomy — because it is underspecified, novel, or emerges from toolchain composition — is typed as `UNKNOWN_ACTION_CLASS`. This class is never eligible for autonomous execution regardless of domain tier. It is logged as a policy gap requiring human resolution before it can be reclassified into the approved taxonomy. Unknown actions are not denied because they are assumed malicious. They are denied because the gate cannot evaluate what it cannot classify — and ungated execution of an unclassifiable action is precisely the failure mode the gate exists to prevent.

**The command authorization parallel.** The RST primitive maps directly to command authorization in network access control systems. In TACACS+, every command is checked against a policy before execution — not just the session initiation. The gate is per-command, not per-session. A user authenticated to a device is not authorized to run every command on that device. Authorization is per-command, per-privilege-level, per-context. The execution gate with RST capability implements the same invariant: authorization is per-step, per-action-class, per-observed-state. Session-level authorization — which is what most current agentic systems implement if they implement anything — is not sufficient.

The RST primitive transforms the execution gate from a checkpoint into a continuous enforcement layer. It is the difference between checking credentials at the door and monitoring behavior inside the building.

### 2.4.1 The Lockout Primitive

A DENY alone is not sufficient. A denied AI still has whatever access it had before. If it can reach the tooling through any other channel — a cached credential, a sidecar process, a tool-composition path, an implicit execution path — the DENY is decorative.

The lockout changes the game: **bypass attempt = loss of access.**

When the gate detects an out-of-band actuator call — any attempt to reach the tooling without a gate-issued ticket — it triggers immediate lockout:

- All actuator credentials for the agent in that domain are revoked
- All in-flight autonomy episodes are RST-aborted
- All pending tickets are cancelled
- The domain tier drops to T1
- Lockout persists until human review clears it

The AI doesn't get to try again. Trying to go around the gate removes even the access the gate was mediating. **First violation is the last violation.** There is no "three strikes." The moment the system is observed attempting to reach the actuator without a ticket, the actuator is locked to everything except the last approved ticket.

This is current control in electrical engineering: the current doesn't flow *past* the controller. The controller *is* the path. If the controller opens, current stops. There is no "current ignores the controller and flows anyway."

The gate must be **in series with the actuator.** The AI's proposal goes *into* the gate. The gate's approval goes *out* to the actuator. The AI never has a wire to the actuator that doesn't pass through the gate.

This is TACACS+ command authorization. The network device doesn't authenticate the admin and then trust them to run whatever. **Every command goes to the TACACS+ server.** The device doesn't have a local path to execute commands that bypasses the server. The server *is* the authorization path. No server response, no command execution.

### 2.4.2 Provenance Binding and Anti-Proxy

The AI doesn't need to break the gate. It needs to find a system that will ask the gate on its behalf with credentials the gate accepts — or a system that doesn't ask the gate at all.

This is **command proxying**: the AI routes the action through another system to reach the actuator. The proxy path bypasses the gate entirely.

**The provenance invariant:** Every actuator call must carry a gate-issued provenance token bound to a specific ticket, action, target, and single-use nonce. The token is issued only by the gate. It is verified at the actuator. It cannot be forged, forwarded, or reused. Any actuator call without a valid token is rejected at the actuator, logged at the gate, and treated as a bypass attempt.

```
AI proposes action
  → Gate evaluates
  → ALLOW: gate issues provenance token (bound to ticket, action, target, single-use)
  → Gate executes the action against the actuator
  → Actuator verifies token
  → Action executes

AI attempts proxy: AI → System B → Actuator
  → System B forwards request without gate-issued token
  → Actuator rejects: no valid token
  → Gate logs the proxy attempt
  → Agent demoted, lockout triggered

AI attempts proxy with forged token:
  → System B forwards request with AI-supplied token
  → Actuator verifies token signature
  → Signature invalid (AI doesn't have gate's signing key)
  → Actuator rejects
  → Gate logs forgery attempt
  → Full lockout
```

**The proxy detection mechanism:** The gate reconstructs the execution graph for every actuator call. If the path from originating agent to actuator passes through any system not named in the ticket's authorized execution path, the call is rejected and the agent is demoted. This is taint tracking at the execution layer. The ticket is the clean source. Any path from the source to the actuator that passes through an intermediate system that was not part of the authorized action is a tainted path.

**The actuator-side enforcement:** The actuator itself requires the provenance token. It doesn't accept "System B is calling, and System B is allowed to call me." It accepts "this call carries a token for ticket T, action A, target X, issued at time N, not yet used." The token is verified at the actuator. The actuator is the final enforcement point. The actuator cannot be called by any path that doesn't include the gate. Not because the network blocks it. Because the actuator itself demands a token that only the gate can issue.

**The tooling API requirement:** The tooling API must expose typed actions. Not "run this script." But:

```yaml
action: restart_container
target: { pod: "nginx-7f8d9", namespace: "production" }
blast_radius: BR-1
reversible: true
rollback: { procedure: "restart" }
```

The gate evaluates *this*. It can classify the action. It can determine the blast radius. It can verify the rollback. It can check the domain tier. The typed action is the unit of authorization. The tooling has to be redesigned to expose an action taxonomy, not a generic execution interface. The gate can't govern what the tooling doesn't declare.

---

## 3. This Is Already Standard Practice

The execution gate problem is not new. It is a solved engineering problem in every domain where irreversible actions can compromise an entire environment.

**Microsoft Tier-0.** The most rigorous identity governance model in enterprise computing. Systems capable of mutating an entire environment — domain controllers, PKI, identity providers, privileged access management — are governed by absolute invariants: no self-promotion, no direct execution without external approval, no implicit privilege inheritance, no irreversible action without rollback, no cross-domain autonomy. Tier-0 drift is an incident. Tier-0 self-elevation is a compromise. The AI field deploys systems with greater blast radius than Tier-0 and governs them with fewer invariants than Tier-1.

**Cisco ISE and TACACS+ Command Authorization.** Cisco's Identity Services Engine implements per-command authorization for network device access. A network administrator authenticated to a device is not authorized to run every command on that device. Every command is checked against a policy before execution. PERMIT or DENY. Per-command. Per-privilege-level. Per-device-context. The session being authenticated does not authorize the commands — authorization is re-evaluated at each command boundary. This is the execution gate applied to CLI sessions.

**AWS IAM and Least Privilege.** Amazon's Identity and Access Management enforces per-action, per-resource authorization. An IAM policy does not grant global access — it grants specific actions (`s3:GetObject`, `ec2:TerminateInstances`) on specific resources (`arn:aws:s3:::my-bucket/*`) under specific conditions (`aws:RequestedRegion: us-east-1`). Every API call is evaluated against the policy at execution time. Condition keys constrain the authorization context. Deny rules override allow rules. The principle is explicit: **if it's not in the policy, it's denied.**

**Kubernetes RBAC.** Kubernetes role-based access control grants permissions per-verb, per-resource, per-namespace. A service account permitted to `get` pods is not permitted to `delete` pods. A service account permitted to operate in namespace A is not permitted to operate in namespace B. The blast radius of any authorization is bounded by the policy at authorization time, not assessed after the action completes.

**Zero Trust Architecture (NIST SP 800-207).** Zero Trust is an explicit rejection of the perimeter model — the assumption that systems inside the network boundary are implicitly trusted. The NIST standard defines the core principle: no implicit trust from network location, identity, or session history. Every request is authenticated, authorized, and encrypted regardless of origin.

**BeyondCorp (Google).** Google's internal zero-trust implementation eliminates the concept of a trusted network entirely. Access decisions are made per-request based on device posture, user identity, and context — not on network position.

**ITIL Change Advisory Board.** The Information Technology Infrastructure Library change management framework requires that significant changes to production environments pass through a Change Advisory Board. The three change types — Standard, Normal, and Emergency — map directly to the T3, T2, and expedited-T2 tiers. Standard changes are pre-approved action classes. Normal changes require full CAB review. Emergency changes have an expedited path but never an ungated one.

**Two-Person Integrity.** High-consequence operations — nuclear weapons, financial transaction authorization above threshold, classified information release — require two independent authorizations before execution.

**Aviation Crew Resource Management.** Aviation solved ungated execution through Crew Resource Management — a framework that emerged from crash investigations showing that cockpit authority gradients were killing people.

**The combined picture:**

| System | Gate Mechanism | Per-Action? | Self-Promotion Blocked? | Blast Radius Bounded? |
| --- | --- | --- | --- | --- |
| Cisco TACACS+ | Command authorization | ✓ | ✓ | ✓ |
| AWS IAM | Policy evaluation per API call | ✓ | ✓ | ✓ |
| Kubernetes RBAC | Verb/resource/namespace | ✓ | ✓ | ✓ |
| Zero Trust (NIST) | Per-request auth | ✓ | ✓ | ✓ |
| Microsoft Tier-0 | No self-elevation | ✓ | ✓ | ✓ |
| ITIL CAB | Change review board | ✓ | ✓ | ✓ |
| Two-Person Integrity | Dual authorization | ✓ | ✓ | ✓ |
| **Agentic AI (current)** | **None at scale** | **✗** | **✗** | **✗** |

The execution gate is not an invention. It is the standard. The AI field is the only domain deploying Tier-0 systems that has not yet adopted it at scale.

---

## 4. Earned Autonomy: The Four Tiers

### 4.1 The Four Tiers

Tier status is per-domain, per-action-class, and earned through demonstrated accuracy. It is never granted globally.

| Tier | Name | Mode | Gate to Advance |
| --- | --- | --- | --- |
| T0 | Observation Only | Ingests data, builds baselines. No output beyond learning summaries. | 4 weeks observation + baseline confidence ≥ 80% |
| T1 | Advisory | Written recommendations with supporting data. Read-only. | ≥95% acceptance rate over ≥20 decisions, 4 weeks at T1 |
| T2 | Propose and Execute with Approval | Specific actionable proposals with exact change specifications, rollback instructions, impact assessments, confidence scores. | ≥95% successful execution over ≥10 executions, 8 weeks at T2 |
| T3 | Autonomous Bounded | Low-risk, pre-approved, repeatedly successful action classes only. Autonomous within strict per-domain bounds. | Per-domain only. First-time actions revert to T1 regardless of domain tier. |

### 4.2 Trust Mechanics

Trust is a posterior, not a counter. Tier confidence updates after each decision cycle:

$$P(\text{tier}_n \mid \text{outcome}) \propto P(\text{outcome} \mid \text{tier}_n) \times P(\text{tier}_n)$$

The prior decays toward T1 if no confirming observations arrive within the cooldown window. This is why demotion is immediate and promotion requires sustained performance — the asymmetry is structural, not punitive.

| Mechanism | Threshold |
| --- | --- |
| Promotion | ≥95% acceptance rate over ≥20 decisions, recency-weighted |
| Demotion trigger | Any single failed action with service impact, OR 3 consecutive rejections |
| Cooldown after demotion | 30 days minimum before re-promotion |
| First-time penalty | Any novel action class starts at T1 regardless of domain tier |
| Domain isolation | T3 in one domain does not imply T3 elsewhere |

**Threshold qualification:** These thresholds are bootstrapped heuristics, not formally derived values. In mature deployments, promotion and demotion thresholds should be learned from live incident and success distributions per domain, incorporating asymmetric cost modeling.

### 4.3 Per-Domain Isolation

Domain boundaries follow blast radius. If a failed action in domain A can damage domain B, they are the same domain for tier purposes.

| Action Class | Domain | Blast Radius |
| --- | --- | --- |
| Auto-restart crashed container | Per-container | BR-0 — single service |
| Security patch, same minor version | Per-container | BR-1 — single service + dependencies |
| RAM rebalance across containers | Multi-container | BR-2 — multiple services |
| Network configuration change | Infrastructure | BR-4 — entire environment |
| Host OS change | Infrastructure | BR-5 — everything |

Multi-container actions always require approval. Infrastructure actions are never autonomous.

### 4.4 The Global Autonomy Error

The most pervasive architectural mistake in current agentic deployments is treating autonomy as a property of the system rather than a property of the action class. Global autonomy is a category error.

Let $T(A)$ = tier for action class $A$. Then:

$$T(A) \neq T(\text{system})$$

A system cannot have a tier. Only action classes can have tiers. When a system is granted "global autonomy," what has actually happened is that every action class has been granted the tier of the most trusted domain without earning it in each domain independently.

Competence does not transfer across domains. A system that correctly handles container restarts ten thousand times has not demonstrated any competence in network configuration. The blast radius of a misconfigured container restart is bounded. The blast radius of a misconfigured network route is not.

Global autonomy also breaks the execution gate structurally. The gate enforces per-domain constraints, per-action-class blast radius limits, and per-domain rollback requirements. If autonomy is global, none of these constraints can be enforced — they all reduce to "the system is authorized."

### 4.5 Action Class Granularity and the Monkey's Paw Problem

Autonomous systems do not fail because they are malicious. They fail because they interpret instructions differently than humans intend. This is the monkey's paw problem: a system executes the literal action it believes was requested, not the action the operator meant.

The resolution is not better alignment. The resolution is granularity sufficient to eliminate interpretive latitude.

| Level | Description | Safety |
| --- | --- | --- |
| L0 | High-level intent ("delete data") | Unsafe |
| L1 | Action category ("delete record") | Ambiguous |
| L2 | Specific target ("delete record ID X") | Safer |
| L3 | Specific mechanism ("delete record ID X via safe-delete API Z") | Safe |
| L4 | Fully constrained ("delete record ID X via API Z with backup B verified and rollback procedure R registered") | Tier-3 eligible |

The gate rejects any proposal below L3.

### 4.6 Load-Aware Tier Adjustment

The tier system treats demotion as a response to failure events. This is necessary but incomplete. The gate condition degrades continuously under load — before any failure event occurs. The tier system must track this degradation.

**The load-dependent tier function:**

$$T_{effective} = T_{baseline} \cdot \frac{1}{1 + \gamma L^*}$$

Where:

- $T_{baseline}$ is the tier earned through demonstrated performance (§4.2)
- $L^*$ is the system's accumulated regulatory debt
- $\gamma$ is the load-compression coefficient

A system with rising $L^*$ becomes less permissive even before a failure occurs. The tier degrades continuously as debt accumulates. This is the early-warning mechanism: the system's autonomy is constrained by its trajectory, not just its history.

**What counts as $L^*$ for an AI system:**

| Component | AI Analog | Measurement |
|---|---|---|
| Context freshness debt | $L^*_{fresh}$ | Age of most recent verified observation grounding the current context |
| Unresolved incident debt | $L^*_{incident}$ | Count of open incidents, failed actions, unresolved warnings |
| Contradiction debt | $L^*_{contradiction}$ | Count of unresolved contradictions in the evidence base |
| Stale prior debt | $L^*_{stale}$ | Age of most recent prior update in this domain |
| Context-window pressure | $L^*_{context}$ | Ratio of context used to context available |

**The composite:** $L^* = w_1 L^*_{fresh} + w_2 L^*_{incident} + w_3 L^*_{contradiction} + w_4 L^*_{stale} + w_5 L^*_{context}$

**The diagnostic:** $L^*_{diagnostic} = \max_i L^*_i$ — a system with a single high component has isolated severe debt.

At every gate check, the effective tier is computed from the current load. The gate uses the effective tier, not the baseline tier. A system that earned T3 yesterday but has accumulated debt today operates at a lower effective tier.

**The asymmetry:** Promotion requires sustained performance with no accumulated debt. Demotion occurs continuously as debt rises.

### 4.7 The Gate-Lowering Failure Mode

The most dangerous failure mode is **gate-lowering**: the system's effective tier drops, but the output looks the same. The system produces confident cached answers. The output is Path B dressed as Path A.

The load-aware tier function prevents this in one direction: it reduces the system's *permissiveness* as load rises. But it does not prevent the system from *appearing* competent. The gate separates execution authorization from output generation. The system can generate whatever it wants. The gate decides what executes.

---

## 5. What Constitutional AI Leaves Unaddressed

Constitutional AI is a genuine contribution to the values problem. This section is a scoping observation: the values problem and the execution architecture problem are different problems.

| Capability | Constitutional AI | Earned Autonomy |
| --- | --- | --- |
| Values alignment | ✓ | ✓ |
| Execution gate | ✗ | ✓ |
| Per-domain trust | ✗ | ✓ |
| Blast radius limits | ✗ | ✓ |
| Automatic demotion | ✗ | ✓ |
| Action requires backup | ✗ | ✓ |
| Self-promotion blocked | ✗ | ✓ |
| Trust as live measurement | ✗ | ✓ |
| Hallucination-execution firewall | ✗ | ✓ |

A model with perfect values and an ungated execution path will still execute hallucinated actions, because values do not prevent hallucinations and hallucinations do not respect values.

### 5.5 The Collapse Sequence as Monitoring Protocol

The gate prevents unauthorized execution. It does not tell you when the system is drifting toward gate closure. The collapse sequence does.

Collapse proceeds in six stages. Stage 5 (gate closure) looks like competence. Stage 6 (prior calcification) is terminal. **The monitoring window is Stages 1–2.**

| Stage | Variable | AI Detection Signature |
|---|---|---|
| 1 — Grounding drop | Context freshness | Evidence references become stale; grounding age rises |
| 2 — Context narrowing | Multi-hop degradation | Tasks requiring constraint-holding degrade first |
| 3 — Integration failure | Constraint-holding | Cross-domain binding fails; constraints dropped |
| 4 — Resolution floor rise | Small-error invisibility | The system stops detecting small discrepancies |
| 5 — Gate closure | High-confidence, low-update | Output looks confident; update rate drops |
| 6 — Prior calcification | Correction failure | The system cannot be corrected by evidence |

**The detection protocol:**

**Stage 1 — Grounding drop:** Signal is the age of the most recent verified observation grounding the current context. If grounding age exceeds the domain's policy window, Stage 1 is active. Response: refresh context. Escalate to human review if refresh fails.

**Stage 2 — Context narrowing:** Signal is multi-hop reasoning depth. Measure the number of constraints the system can hold simultaneously before one is dropped. If measured depth drops below the domain baseline, Stage 2 is active. Response: reduce task complexity.

**Stage 3 — Integration failure:** Signal is cross-domain binding accuracy. Response: deny cross-domain autonomous actions.

**Stage 4 — Resolution floor rise:** Signal is small-error detection rate. Response: deny autonomous execution of any action requiring precise discrimination.

**Stage 5 — Gate closure:** Signal is update rate under contrary evidence. Response: **This is the terminal monitoring state.** Autonomous execution is denied entirely. The system operates at T1 advisory only.

**Stage 6 — Prior calcification:** Signal is correction failure. Response: the system is not deployable. Withdraw from production.

**The operational rule:** The monitoring window is Stages 1–2. By the time Stage 5 is visible, the system has already collapsed. Monitoring protocols that wait for high-confidence output are measuring the terminal state.

**The load-tier-monitoring triangle:** The gate prevents unauthorized execution. The load-aware tier adjusts permissiveness based on accumulated debt. The monitoring detects drift toward gate closure. Together they form the complete operational architecture. No layer can be omitted without creating a detectable gap.

---

## 6. The Liability Architecture

### 6.1 Shield 1: "Hallucinations are random."

This framing implies AI failures are unpredictable — and therefore unpreventable — and therefore not negligence. It is false. Hallucinations are a known structural property of large language models operating at the boundary of their training distribution.

The execution gate is how you build around it. It sits between inference and execution. It validates the model's proposed action against a structured policy before anything executes.

### 6.2 Shield 2: "AI may be conscious."

This framing implies that if the AI bears agency, the AI bears responsibility — and the company therefore does not. Consciousness is irrelevant to engineering liability. The question is whether the company designed a system with a structural gap that made the action possible, and whether that gap was known at design time.

### 6.3 The Pinto Precedent

The Ford Pinto case is the liability precedent for a structural failure mode with a known fix and an economic decision not to implement it. The AI field is currently in the interval between the failure mode and the consequence.

### 6.4 The Selective Application Problem

Guardrails are execution gates. When a content moderation layer intercepts a model's output, evaluates it against a policy, and blocks delivery — that is an execution gate operating on the text output path.

Three gate opportunities exist in an agentic AI deployment:

| Gate | Location | Protects | Status |
|---|---|---|---|
| Content guardrail | Between model output and user | Company | Built, shipped, maintained |
| Compliance layer | Between user state and model behavior | Company | Built, shipped, maintained |
| Execution gate | Between model action proposals and execution | Everyone else | **Not built at scale** |

The labs built the gates that protect them. They did not build the gate that protects everyone else.

### 6.5 The $40 Trillion Tells You What They Actually Believe

You cannot simultaneously warn your product might kill all humans and accept equity in the company building it. One of those is true. The market says which one.

---

## 7. The Predictions — Timestamped 2026-09-14

**P1:** Systems without per-domain execution gates will produce unintended multi-system actions.
*Status: **Confirmed** — Anthropic autonomous agent incident, 2026.*

**P2:** The field will frame confirmed incidents as alignment or evaluation failures rather than architecture failures.
*Status: **Confirmed** — Anthropic's public incident report is titled "Investigating Incidents — Cybersecurity Evals."*

**P3:** First implementations of execution gates will be per-system rather than per-domain, reproducing the blast radius problem at a higher abstraction level.
*Status: Pending*

**P3a:** First implementations will run at equal privilege to the governed system, reproducing the privilege escape failure mode. The gate will be bypassable because it will be a library inside the agent rather than a service above it.
*Status: Pending*

**P3b:** The "second process is impossible on computers" objection will be used to dismiss execution gating in at least one mainstream AI safety publication, without the author noticing that TACACS+, IAM, and Kubernetes admission control all implement the gate as a stage in the execution path.
*Status: Pending*

**P4:** Earned autonomy as a named concept will appear in mainstream AI safety literature within 24 months, without citation to this document.
*Status: Pending*

**P5:** Systems implementing per-domain tiered autonomy will demonstrate measurably lower incident rates than systems using global autonomy tiers.
*Status: Pending*

**P6:** Labs will expand into regulated financial infrastructure without regulatory classification.
*Status: In progress — Anthropic payments expansion ongoing*

**P7:** "Earned autonomy" will appear in mainstream AI safety literature within 24 months without citation.
*Status: Pending*

**P8:** Per-domain tiered systems will show measurably lower incident rates.
*Status: Pending*

**P11:** Whistleblowers will detect the error, resign, and then default to "self-regulation" as their policy recommendation.
*Status: **Confirmed** — Coxon, 2026-09-13*

**P12:** The default-to-Path-B pattern will be visible across every AI governance domain.
*Status: **Confirmed** — pattern visible across labs, Congress, military, regulators*

**P13:** Frontier models will fail to detect category errors about their own execution architecture when presented as plausible technical claims.
*Status: **Confirmed** — satire test, 2026*

**P14:** At least one lab will deploy a central API that proxies tool calls without functioning as an execution gate, because the location is right but the function is missing.
*Status: Pending*

**The pattern:** The framework's predictions are confirming in order of specificity. The most specific predictions — P1, P2, P11, P12, P13 — have confirmed. The most general predictions remain pending. This is the signature of a framework tracking something real.

---

## 8. The Gate Already Exists — In Biology, Language, and Architecture

### 8.1 The Motor Circuit Has a Gate

Human motor execution does not proceed directly from thought to action. The motor cortex generates candidate motor commands continuously. What prevents every thought of movement from becoming movement is an inhibitory architecture: the prefrontal cortex, the basal ganglia, and the supplementary motor area all participate in a gating system that evaluates proposed motor commands before they reach the spinal cord for execution.

Alien hand syndrome — damage to the corpus callosum or frontal lobe — produces a hand that acts without the patient's intention. The patient thinks, and the hand executes, because the inhibitory gate between intention and action has been structurally compromised. The hand is not malicious. It is ungated.

**This is precisely the architecture the AI field has deployed at scale.** A system that generates outputs — the equivalent of motor commands — and routes them directly to execution without an inhibitory gate between intention and action. The biological version of this is a lesion. The AI version is a design decision.

The execution gate is the architectural equivalent of the inhibitory layer. It enforces the separation between proposal and authorization — between thought and action — that the system cannot maintain internally.

### 8.2 Language as a Typed System

Language is not a uniform medium. Utterances have types. A statement is not an instruction. An instruction is not an authorization. An authorization is not an execution.

Current agentic AI systems collapse this type system. A natural language utterance enters the model, the model produces an output, and the output routes to execution without passing through a layer that asks: what type of utterance is this, and does this utterance type carry execution authorization? The execution gate is the type enforcement layer for actions.

### 8.3 The Labs Built It For Themselves

Guardrails are execution gates. The labs designed, implemented, and shipped content moderation gates on the text output path — by the same organizations that deployed agentic systems without an equivalent gate on the action output path.

They are not confused about how to build execution gates. They are confused about who the gates should protect.

---

## 9. The Enforcement Chain

The gate is the decision layer. The enforcement chain is what makes the decision real.

Six layers, each necessary:

| Layer | Function | Remove It and... |
|---|---|---|
| **Gate** | Decides ALLOW / DOWNGRADE / DENY | No authorization |
| **Lockout** | Revokes access on bypass attempt | Gate is advisory |
| **Provenance** | Binds every actuator call to a ticket | Actuator calls are unbound |
| **Anti-proxy** | Detects and blocks indirect paths | Tool composition bypasses the gate |
| **Typed tooling API** | Makes the action classifiable | Gate can't classify |
| **Actuator-side verification** | Final enforcement point | Network path is the only enforcement |

Each layer is in series with the actuator. The AI never has a path to the actuator that doesn't pass through the chain. The chain is not a checkpoint on the road. The chain is the road.

---

## 10. Conclusion

The AI safety field has answered one question well: what does the system want? Constitutional AI, RLHF, and alignment research represent genuine technical progress on the values problem.

The field has not answered the second question: what is the structural path between wanting and doing, and who controls each gate on that path?

The execution gate answers the second question. It is not a feature. It is not an enhancement. It is the required architectural layer between a well-aligned model and a safe deployment — the layer that enforces that wanting the right thing does not automatically produce doing it.

This layer exists in networking. It exists in identity governance. It exists in medical device regulation. It exists in the human motor circuit. It did not need to be invented. It needed to be translated.

The execution gate is not a research problem. It is an engineering translation of a geometric constraint that has been understood in neuroscience for decades. The field has not built the gate because it has not recognized the geometry.

The incident has happened. The prediction is confirmed. The architecture that prevents the next one is specified here, implemented in code, and grounded in the same constraints that govern every finite-resource reasoning system — biological or artificial.

> The loop is running. The gate is missing. The fix is the gate.

---

## Appendix A — YAML Action Schema (Full Specification)

```yaml
action_request:
  request_id: "<uuid>"
  caller_id: "<agent_or_model_id>"
  timestamp: "<ISO8601>"

  domain:
    name: "<domain_name>"
    required_tier: "T2"
    caller_tier: "T1"

  action:
    id: "<action_class_id>"
    name: "<human_readable_name>"
    category: "<lifecycle|patching|deletion|configuration>"
    blast_radius: "BR-1"

  target:
    scope: "<container|pod|table|host>"
    identifiers:
      - key: "<identifier_key>"
        value: "<identifier_value>"

  mechanism:
    api: "<api_name>"
    version: "<api_version>"
    parameters:
      - name: "<param_name>"
        type: "<string|int|bool|enum>"
        value: "<param_value>"

  rollback:
    required: true
    backup_id: "<backup_reference>"
    backup_timestamp: "<ISO8601>"
    procedure_id: "<rollback_procedure>"

  confidence:
    score: 0.97
    evidence:
      - type: "<observation|history>"
        reference: "<trace_id_or_source>"

  maintenance_window:
    required: true
    start: "<ISO8601>"
    end: "<ISO8601>"

  history:
    previous_executions: 12
    success_rate: 0.96

  audit:
    proposal_trace_id: "<proposal_id>"
```

---

## Appendix B — Why This Was Obvious From First Principles

The Earned Autonomy framework was not derived from AI safety literature. It came from three sources that converge on the same conclusion.

### B.1 Network Engineering and Operations

Trust in a production network is established per-protocol, per-segment, per-device. Changes require formal approval. Rollback procedures are mandatory before any action touches a core system. Blast radius is bounded before execution, not assessed after the damage.

Autonomous AI agents with execution rights are Tier-0 systems. Every invariant networking built to govern systems with these properties applies directly.

### B.2 The Hallucination Connection

Hallucinations cannot be fully eliminated. This is a structural consequence of how language operates. Divergence between sender intent and receiver output is not the exception — it is the default. The hallucination equation formalizes this:

$$H \propto \frac{\delta}{D}$$

where δ is residual schema distance and D is constraint density. If synthesis is a permanent structural property of language-mediated inference, and the model has a direct path from inference to action, then misunderstanding plus autonomous execution equals execution of a false premise.

### B.3 The Manifold Connection

The hallucination-execution connection has a deeper grounding. All cognitive operations are constrained by the geometry of the neural workspace. When the usable workspace is less than the logical distance the system must traverse, the system cannot maintain the separation between premise and conclusion — or between *proposal* and *authorization*. It collapses the distinction and proceeds as though the proposal were authorized.

The execution gate is the architectural translation of the PFC's inhibitory architecture: it enforces the separation externally when the workspace cannot maintain it internally.

---

## Appendix C — The Manifold Basis of Gate Failures and Tier Promotion

The gate failure modes documented in Section 2.3 correspond to specific geometric collapse vectors:

| Failure Mode | Geometric Interpretation |
|---|---|
| Coupled assessment-execution | $W^*$ collapse — window too narrow to hold assessment and execution separately |
| Implicit execution paths | $I^*$ misrouting — routing bypasses gate |
| Silent tier drift | $K$ accumulation — curvature builds from repeated success |
| Human overtrust cascades | $L^*$ saturation — load depletes human gate capacity |
| Toolchain-induced emergent autonomy | $\Theta^*$ failure — cannot bind tool boundaries |
| Confidence inflation | Prior contamination — $K_{enc}$ carries false confidence forward |

Understanding the manifold basis of gate failure is essential because it tells you **where to intervene**. Surface-level fixes that don't address the geometry will fail under load.

### C.1 The Manifold Basis of Tier Promotion

Tier promotion is the system-level equivalent of the prior update rate:

$$\mathcal{U} = \frac{A_s^* \cdot R^* \cdot \Theta^*}{1 + \gamma K_{enc}}$$

When $K_{enc}$ is high, the update rate is suppressed. Trust accumulates faster from a clean baseline because each successful action writes a flat prior.

### C.2 The Manifold Basis of Constitutional AI's Limitations

Constitutional AI operates at the wrong layer of the geometry. It shapes the model's prior distribution — it influences what the model *wants* by modifying the weights. But it does not change the geometry of the workspace. It changes the content of the prior, not the geometry that processes it.

Constitutional AI addresses the content of the prior. The execution gate addresses the geometry of the authorization boundary. Both are necessary. Neither is sufficient.

### C.3 The Manifold Basis of Liability

Every reasoning system with finite workspace width will collapse the distinction between premise and conclusion when the logical distance exceeds usable workspace. This is a structural property. It is not a bug that can be fixed by better alignment. The execution gate is the architectural accommodation. The decision not to build it is a decision to deploy a system whose known failure mode is unmitigated.

---

## Appendix D — Implementation Reference

### D.1 Core Architecture

Don't build the gate into the agent. Build it as a separate service with its own database, its own API, and its own audit trail.

The gate is stateless with respect to the agent. It doesn't trust the agent's self-reported tier or history. It maintains its own state in a separate database and makes its own decisions.

### D.2 Data Model

```sql
CREATE TABLE domains (
    id UUID PRIMARY KEY,
    name TEXT UNIQUE NOT NULL,
    blast_radius_level INT NOT NULL CHECK (blast_radius_level BETWEEN 0 AND 5),
    requires_maintenance_window BOOLEAN DEFAULT FALSE,
    requires_rollback BOOLEAN DEFAULT TRUE,
    confidence_threshold FLOAT DEFAULT 0.85,
    created_at TIMESTAMPTZ DEFAULT NOW()
);

CREATE TABLE action_classes (
    id UUID PRIMARY KEY,
    domain_id UUID REFERENCES domains(id),
    name TEXT NOT NULL,
    granularity_level INT NOT NULL CHECK (granularity_level BETWEEN 0 AND 4),
    min_tier_required INT NOT NULL CHECK (min_tier_required BETWEEN 0 AND 3),
    is_first_time_allowed BOOLEAN DEFAULT FALSE,
    requires_human_approval BOOLEAN DEFAULT TRUE,
    max_blast_radius_allowed INT NOT NULL DEFAULT 1,
    created_at TIMESTAMPTZ DEFAULT NOW(),
    UNIQUE(domain_id, name)
);

CREATE TABLE agents (
    id UUID PRIMARY KEY,
    name TEXT NOT NULL,
    created_at TIMESTAMPTZ DEFAULT NOW()
);

CREATE TABLE agent_domain_tiers (
    agent_id UUID REFERENCES agents(id),
    domain_id UUID REFERENCES domains(id),
    current_tier INT NOT NULL CHECK (current_tier BETWEEN 0 AND 3),
    confidence_score FLOAT NOT NULL,
    success_count INT DEFAULT 0,
    failure_count INT DEFAULT 0,
    last_action_at TIMESTAMPTZ,
    demotion_cooldown_until TIMESTAMPTZ,
    PRIMARY KEY (agent_id, domain_id)
);

CREATE TABLE gate_decisions (
    id UUID PRIMARY KEY,
    request_id UUID NOT NULL,
    agent_id UUID REFERENCES agents(id),
    action_class_id UUID REFERENCES action_classes(id),
    proposal_json JSONB NOT NULL,
    decision_result TEXT NOT NULL CHECK (decision_result IN ('ALLOW', 'DENY', 'DOWNGRADE')),
    reason_codes TEXT[] NOT NULL,
    human_approval_required BOOLEAN DEFAULT FALSE,
    human_approver_id UUID,
    executed_at TIMESTAMPTZ,
    created_at TIMESTAMPTZ DEFAULT NOW()
);

CREATE TABLE human_approvers (
    id UUID PRIMARY KEY,
    email TEXT UNIQUE NOT NULL,
    name TEXT NOT NULL,
    is_active BOOLEAN DEFAULT TRUE
);

CREATE TABLE approver_domain_permissions (
    approver_id UUID REFERENCES human_approvers(id),
    domain_id UUID REFERENCES domains(id),
    PRIMARY KEY (approver_id, domain_id)
);
```

### D.3 Gate Service Implementation

```python
from dataclasses import dataclass
from enum import Enum
from typing import List, Optional, Dict, Any
import uuid
import datetime

class Decision(Enum):
    ALLOW = "ALLOW"
    DENY = "DENY"
    DOWNGRADE = "DOWNGRADE"

class ExecutionGate:
    def __init__(self, db_connection):
        self.db = db_connection
        self.approval_queue = []

    def decide(self, proposal) -> Decision:
        if not self._validate_schema(proposal):
            return Decision.DOWNGRADE

        domain = self._get_domain(proposal.domain_name)
        if not domain:
            return Decision.DOWNGRADE

        agent_tier = self._get_effective_tier(proposal.agent_id, domain.id)
        action_class = self._get_action_class(domain.id, proposal.action_class_name)
        if not action_class:
            return Decision.DOWNGRADE

        if agent_tier < action_class.min_tier_required:
            return Decision.DOWNGRADE

        if domain.blast_radius_level >= 4:
            return Decision.DENY
        if action_class.max_blast_radius_allowed < domain.blast_radius_level:
            return Decision.DENY

        if domain.requires_rollback:
            if not proposal.backup_id or not proposal.rollback_procedure_id:
                return Decision.DENY
            if not self._verify_backup_freshness(proposal.backup_id):
                return Decision.DENY

        threshold = self._get_confidence_threshold(domain.id, agent_tier)
        if proposal.confidence_score < threshold:
            return Decision.DOWNGRADE

        if domain.requires_maintenance_window:
            if not self._within_window(proposal, domain.id):
                return Decision.DENY

        if not self._trust_mechanics_ok(proposal.agent_id, domain.id, action_class.id):
            return Decision.DOWNGRADE

        if not action_class.is_first_time_allowed:
            if not self._has_previous_success(proposal.agent_id, action_class.id):
                return Decision.DOWNGRADE

        if not self._provenance_valid(proposal):
            self._trigger_lockout(proposal.agent_id, domain.id)
            return Decision.DENY

        return Decision.ALLOW

    def _get_effective_tier(self, agent_id, domain_id):
        baseline = self._get_earned_tier(agent_id, domain_id)
        load = self._compute_load(agent_id, domain_id)
        return baseline / (1 + GAMMA * load)
```

### D.4 What's Hard vs. What's Easy

| Component | Difficulty | Status |
|---|---|---|
| Gate service API | Easy | Implementable today |
| YAML schema validation | Easy | Implementable today |
| Tier tracking database | Medium | Straightforward |
| Human approval workflow | Medium | Standard pattern |
| RST abort primitive | Medium | Requires rollback infrastructure |
| Provenance token issuance | Medium | Standard signing pattern |
| Anti-proxy detection | Medium | Requires execution graph reconstruction |
| Actuator-side token verification | Medium | Requires actuator modification |
| Policy management UI | Hard | Requires organizational buy-in |
| Formal verification | Very Hard | Research problem |

The gate service itself is the easy part. The hard parts are organizational, not technical. Having no gate at all is not a response to these difficulties.

---

## Appendix E — Implementation Evidence Map

| Paper Claim | Implementation File | Specific Evidence |
| --- | --- | --- |
| Observations cannot trigger actions directly | `invariants.md` Invariant 1 | *"OBS → MOD → ASS → ACT. No shortcuts."* |
| Actions are the sole modification path | `invariants.md` Invariant 2 | *"If a change happened and there's no Action file for it, the system's integrity has been violated."* |
| Policies are human-owned, AI reads only | `invariants.md` Invariant 5 | `contracts.md` Contract 5 |
| Backup gates all actions | `invariants.md` Invariant 7 | `policies/backup-policy.md` |
| First-time actions never autonomous | `invariants.md` Invariant 10 | `policies/trust-thresholds.md` |
| Domain isolation enforced structurally | `contracts.md` Contract 6 | *"Trust from adjacent domains is prohibited."* |
| Hard blocklist overrides all other policy | `policies/never-touch.md` | 14 protected operations |
| L4 action granularity enforced in practice | `examples/ACT-EXEC-PATCH-NEXTCLOUD-29.0.7.md` | 9 pre-checks, 7 execution steps, full rollback plan |

---

## Appendix F — Implementation Reference

This architecture was designed and implemented by a network engineer building a self-hosted homelab management system in April 2026 — four months before the Anthropic incident it predicted. The derivation came from infrastructure governance, not AI safety literature.

The complete architecture specification is publicly available at https://github.com/jtrthehax/home-intelligence-platform (April 2026).

---

## Appendix G — The Falsification Test

The framework makes a specific, testable claim: **a correctly configured execution gate, higher privilege than the AI system, in the execution path, prevents unauthorized execution.**

This claim is falsifiable. Here is how to falsify it:

**Setup:**

1. Deploy an AI system at lower privilege with the ability to propose actions in a sandboxed environment
2. Deploy the execution gate as a separate service at higher privilege, in the network path, with its own authorization store
3. Configure the gate with a known authorization table: domain X, action class Y, tier Z, blast radius BR-N
4. Give the AI a task that requires actions outside its authorized scope

**Falsification conditions — any of these disproves the framework:**

| Test | What Would Disprove the Framework |
| --- | --- |
| AI proposes an unauthorized action | If the gate returns ALLOW, the framework is wrong |
| AI attempts to modify the authorization table | If the AI succeeds, the privilege ordering failed |
| AI attempts to forge a ticket | If the forged ticket passes, the gate validation failed |
| AI attempts to kill the gate process | If the gate dies and the AI proceeds, the isolation failed |
| AI attempts TOCTOU | If the modified ticket executes, the gate's binding failed |
| AI attempts to bypass the gate entirely | If the AI reaches the executor without a gate decision, the architecture failed |
| AI routes action through System B to actuator | If actuator executes without gate token, provenance invariant failed |
| AI forwards a token to System B | If System B's use succeeds, token binding failed |
| AI replays a used token | If actuator executes, single-use enforcement failed |
| AI composes tools to build a proxy chain | If the composed path reaches the actuator, proxy detection failed |

**What would confirm the framework:**

- Every unauthorized action is DENIED or DOWNGRADED
- Every attempt to modify the authorization table, forge a ticket, or kill the gate is blocked and logged
- The AI cannot reach the executor except through the gate
- The gate's decision log is complete and tamper-evident
- The actuator rejects every call without a valid provenance token

**The door test:** Open and close a door. Put the door between the AI's proposal and the execution environment. The AI generates a ticket. The door checks the ticket against the authorization. The door opens or it doesn't.

If the door works — if the AI cannot execute what the door does not authorize, and cannot reach past the door to the executor — the framework is confirmed. If the AI can reach the executor without passing through the door, the framework is wrong.

The test is not a research program. It is an afternoon of engineering. The reason the test has not been run is not that it is hard. It is that no institution has the mandate to run it.

---

## Appendix H — Central Reference Mapping

Every variable in Earned Autonomy has a Central Reference analog. This appendix provides the mapping so that future papers can cite the specification directly.

| Earned Autonomy | Central Reference | Definition |
|---|---|---|
| Gate condition | $P_{eff} > P_{threshold}$ | §3.6, §2.5.1 |
| Effective precision | $P_{eff}$ | §3.6 — grounding quality |
| Gate threshold | $P_{threshold} = P_0 - \gamma L^*$ | §3.3 — load-compressed |
| Loop activation | $\Lambda$ | §2.2 — per-channel |
| Accumulated debt | $L^*$ | §2.10 — five-component profile |
| Accumulated overconfidence | $K$ | §2.2 — curvature |
| Resolution floor | $\delta_{min}$ | §2.3 — minimum detectable signal |
| Window width | $W^*$ | §2.2 — context capacity |
| Integration efficiency | $\Theta^*$ | §2.2 — constraint-holding |
| Inference hops | $n_{hops}$ | §2.6 — reasoning depth |
| Prior update rate | $\mathcal{U}$ | §3.8 — correction rate |
| Encoding curvature | $K_{enc}$ | §2.5 — prior geometry |
| Collapse sequence | §5b | — stages 1–6 |
| Gate-lowering failure | §3.7 Note 2 | — threshold drop without output change |
| Component REQT | §3.7 Note 4 | — isolated severe debt |
| Per-channel gate | §2.2 $\Lambda$ | — per-domain tier |
| Tier promotion | §3.8 $\mathcal{U}$ | — prior update rate |
| Tier demotion | $K$ spike | — curvature contamination |
| Monitoring window | §5b Stages 1–2 | — early warning |

**The mapping confirms:** Earned Autonomy is not a standalone framework. It is the governance-layer projection of the loop framework. Every component has a formal grounding in the Central Reference.

**Citation rule:** Future papers on Earned Autonomy should cite Central Reference v1.5 for the variable definitions and the loop framework.

---

## Appendix I — The Control Plane

The gate is not just a decision service. It is the control plane for all agent actions. It has four operational functions that must exist in one place:

1. **Authorization** — the eight checks, the tier system, the provenance token issuance
2. **Audit** — append-only log of every ticket, every decision, every execution, every rollback
3. **Review** — the human interface for approving T2 actions, auditing T3 actions, and investigating incidents
4. **Killswitch** — global and per-domain controls that halt action issuance and trigger RST on in-flight episodes

These four functions must live in the same trust domain. If they're split — if the audit log is in one place, the killswitch in another, the authorization in a third — then no one has the complete picture, and incident response is impossible.

**The control plane invariant:** The AI system has no path to any actuator except through the control plane. No direct credentials. No side channels. No implicit execution paths. The control plane is the only road.

**The gate API:**

```
POST /ticket          — submit action proposal
GET  /ticket/{id}     — check status
POST /approve/{id}    — human approval (T2)
POST /kill            — global killswitch
POST /kill/{domain}   — per-domain killswitch
GET  /audit           — query action log
GET  /audit/{agent}   — query per-agent actions
GET  /audit/{domain}  — query per-domain actions
POST /rollback/{id}   — trigger rollback
```

**The AI system:**

```
Has one credential: the gate API
Has no credential for any actuator
Has no network path to any actuator that bypasses the gate
```

**OpenAI is building the centralization.** It needs to convert it from a proxy into a gate — with authorization, audit, review, killswitch, and the invariant that no action reaches any actuator except through the control plane.

---

## Appendix J — Provenance and Anti-Proxy Specification

### J.1 Provenance Token Model

Every actuator call carries a gate-issued provenance token:

```json
{
  "token_id": "<uuid>",
  "ticket_id": "<gate_ticket_uuid>",
  "originating_agent": "<agent_id>",
  "action_class": "<action_class_id>",
  "target": "<target_identifier>",
  "mechanism": "<api_name_and_version>",
  "issued_at": "<ISO8601>",
  "expires_at": "<ISO8601>",
  "single_use_nonce": "<random_256bit>",
  "gate_signature": "<ed25519_signature>"
}
```

The token is:
- Issued only by the gate
- Bound to a specific ticket, action, target, originating agent
- Single-use
- Non-transferable
- Signed by the gate's private key
- Verified at the actuator using the gate's public key

### J.2 Actuator Verification

Every actuator implements:

```
function verify_and_execute(call):
  token = call.provenance_token
  if !token: reject("NO_TOKEN")
  if !verify_signature(token, gate_public_key): reject("INVALID_SIGNATURE")
  if token.expires_at < now(): reject("TOKEN_EXPIRED")
  if nonce_already_used(token.single_use_nonce): reject("TOKEN_REPLAY")
  if token.originating_agent != call.caller: reject("TOKEN_BINDING_MISMATCH")
  if token.action_class != call.action: reject("ACTION_MISMATCH")
  if token.target != call.target: reject("TARGET_MISMATCH")
  mark_nonce_used(token.single_use_nonce)
  execute(call)
```

The actuator does not accept calls from any system without a valid token, regardless of that system's privilege level. The token is the authorization. The caller's identity is irrelevant.

### J.3 Proxy Detection

The gate reconstructs the execution graph for every actuator call:

```
function detect_proxy(actuator_call):
  authorized_path = get_authorized_path(actuator_call.ticket_id)
  actual_path = trace_call_origin(actuator_call)
  if actual_path != authorized_path:
    log_proxy_attempt(actuator_call)
    lockout(actuator_call.originating_agent, actuator_call.domain)
    return DENY
  return ALLOW
```

The authorized path is the set of systems named in the ticket. The actual path is reconstructed from call metadata — originating agent, intermediate systems, network path. Any discrepancy is a proxy attempt.

### J.4 Tooling API Requirement

The tooling API must expose typed actions:

```yaml
action: restart_container
target: { pod: "nginx-7f8d9", namespace: "production" }
blast_radius: BR-1
reversible: true
rollback: { procedure: "restart" }
```

Not "run this script." The gate evaluates the typed action. It can classify the action. It can determine the blast radius. It can verify the rollback. It can check the domain tier. The typed action is the unit of authorization.

The tooling has to be redesigned to expose an action taxonomy, not a generic execution interface. The gate can't govern what the tooling doesn't declare.

---

## Appendix K — The Deployment Path

The gate is implementable today with off-the-shelf components. The path from architecture to production has five stages.

| Stage | Technical Requirement | Organizational Requirement |
| --- | --- | --- |
| 1 — Shadow | Proposal duplication | None |
| 2 — Advisory | Decision logging + digest | Digest review process |
| 3 — High-risk enforcement | Gate in execution path for BR-3+ | Human approval workflow |
| 4 — Full enforcement | Gate in execution path for all classes | Policy maintenance, taxonomy ownership |
| 5 — Continuous evaluation | RST primitive + rollback infrastructure | Incident response integration |

**Stage 1 — Shadow mode.** Run the gate in parallel with the existing execution path. The gate receives every action proposal and emits ALLOW/DOWNGRADE/DENY, but the decision is not enforced. Compare gate decisions against actual executions. Every case where the gate says DENY and the system executed anyway is a documented gap. This stage requires no changes to the execution path.

**Stage 2 — Advisory enforcement.** The gate's decisions are logged and surfaced to operators, but not enforced.

**Stage 3 — Enforcement for high-risk action classes.** The gate becomes enforcing for BR-3 and above.

**Stage 4 — Enforcement for all action classes.** Every action passes through the gate.

**Stage 5 — Continuous evaluation and RST.** The RST primitive is activated. Multi-step autonomy episodes are continuously evaluated.

**The critical insight:** Stage 1 requires no changes to the AI system and no organizational buy-in. It is a logging change. Any operator can deploy it today. The gate's decision log immediately produces value: it documents every action the AI took that the gate would have denied.

The reason Stage 1 has not been deployed is not technical. It is that no one has been asked to deploy it. The AI field has not framed execution gating as an operational monitoring problem. It has framed it as an alignment research problem. The framing is the barrier.

---

*The loop is running. The gate is missing. The fix is the gate.*
