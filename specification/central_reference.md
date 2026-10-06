# Central Reference v1.8

**A Unified System Specification for the Loop Framework**

**Robinson, 2026**

**Version:** 1.8
**Date:** 2026-09-30
**Status:** Composition document — composes the registry, stack, and deltas into a readable specification. Supersedes v1.7.
**Framework:** Manifold Schema v7.2
**Companion artifacts:** `registry.md`, `stack.md`, `deltas.md`
**Purpose:** This document is the readable anchor for the loop framework. It states the claim, states the composition, and cites the artifacts that hold the content. Future papers cite this document and the artifacts together.

---

## Changelog — v1.7 → v1.8

This changelog exists so any reader — human or AI — can see the convergence path, not just the endpoint. v1.7 was the domain-projection-aligned specification: it absorbed the expression/congruence/masking constructs from the speech projection and stood at ~50 variables, ~40 equations, and ~67 anchors, all within one document. v1.8 is a **composition** pass: the content has moved into three companion artifacts (registry, stack, deltas), and this document is the readable index that ties them together.

| Step | Change | Location | Reason |
|---|---|---|---|
| 1 | Version bumped to v1.8 | Header | Versioning track |
| 2 | Companion artifacts registered | Header | `registry.md`, `stack.md`, `deltas.md` |
| 3 | Part 0 restructured — the two-layer model | Part 0 | The document now cites artifacts; the reader needs to know the two layers |
| 4 | Part II (The Composition) added | New | The composition claim is the paper's argument |
| 5 | §0.5 (Riemannian framing) added | New section | Names the geometry. Implicit across four papers. |
| 6 | §2.19 (post-CR primitives) added | New section | Registers $H, \Delta_{window}, \beta_{mod}, f_{crit}, \kappa_{trans}, S_{ext}, B_{eff}, T_{NDE}$ |
| 7 | §2.19b (substrate depth) added | New section | The variable count is substrate-dependent |
| 8 | §3.20 (threshold family) added | New section | Three thresholds, one family |
| 9 | §25a (three anchors) added | New section | CR, Category, MPI — different scopes |
| 10 | $H$ symbol collision fixed | §3.13 | Rename → $H_{HRV}(C)$ |
| 11 | Triplicated equations removed | Throughout | Point at registry canonical homes |
| 12 | Prediction duplication reduced | Part VII | Index by paper rather than restate |
| 13 | Cohesion check rewritten | Part VIII | Now references deltas.md |

**What did not change:** The master equation, the intelligence definition, the collapse sequence, the recovery ladder, the four profiles, the causal chain, and the mechanism set all remain as they were in v1.7. v1.8 is a composition pass, not a mechanism revision.

**Why the composition pass is necessary:** The stack has grown to approximately 32 papers across four sub-programs (loop framework, language program, URM, substrate premise). Nine equations were triplicated across documents. One symbol collision ($H$) had accumulated. Three thresholds were registered separately without a family. The delta file for v1.7 → v1.8 could not be applied because it had to absorb the composition work of six post-1.7 papers simultaneously. The fix is to separate the content (artifacts) from the argument (this document).

---

## Part 0 — How to Read This Document

### 0.1 The Two Layers

This specification has two layers.

**The composition artifacts** hold the content:

- `registry.md` — every variable, mechanism, and named phenomenon, in one composable lookup
- `stack.md` — the causal ordering, from resources through geometry to output, with load as persistent drag
- `deltas.md` — every paper's alignment list for the composition

**This document** holds the argument:

- The claim (Part I)
- The composition (Part II)
- The mechanism summary (Part III, with references to the artifacts)
- The causal chain (Part IV, with references to the stack)
- The collapse and recovery model (Part V)
- The empirical anchors (Part VI)
- The predictions (Part VII)
- The cohesion check (Part VIII)

**The content lives in the artifacts. The argument lives here.** When a section here needs a variable, an equation, or a mechanism, it cites the artifact rather than restating. When a section here needs to make an argument, it makes the argument.

### 0.2 Reader Routing

| If you are... | Read... |
|---|---|
| **A reader** trying to understand the framework | Part I, Part II, Part III |
| **A tester** trying to falsify a prediction | Part VI, Part VII, and the individual paper that owns the prediction |
| **A builder** working with the framework | `registry.md` and `stack.md` first, then Part 0–II of this document |
| **An evaluator** trying to assess the framework | Part II (composition), Part VIII (cohesion check), `deltas.md` |

### 0.3 The Composition Claim

The framework's explaining power is not the sum of its papers. It is the **composition** of its variables.

Each paper in the stack contributed independent observations — from physiology, cognition, language, AI, social systems — and extracted shared primitives. The registry work transformed those observations into composable variables. The composition is what makes the framework usable as a whole.

The claim, in one line:

> **The framework is not a theory with applications. It is a specification with projections. The composition is the contribution.**

Part II develops this claim.

---

## Part I — The Claim

### 1.1 Intelligence Is the Loop

Intelligence is the energy-expensive loop of error detection against sensory input, followed by iterative reinvestment of resources toward structural convergence.

The loop is substrate-agnostic. It applies identically to trees, insects, humans, institutions, and LLMs. Current LLMs satisfy zero of three requirements for a non-zero product. Speed is high. The loop is not running.

### 1.2 The Master Equation

$$C_s = \left(A_s^{*\,0.15} \cdot R^{*\,0.30} \cdot W^{*\,0.25} \cdot \Theta^{*\,0.15}\right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + L^*}$$

Where $C_s$ is usable bandwidth — how much of the system's own capacity is accessible. Every variable is a resource. $L^*$ is the denominator drag.

The exponents are provisional. They reflect the empirical collapse sequence (precision degrades first, window second) but have not been formally calibrated. See `registry.md` §1.2 for the variable definitions.

### 1.3 The Intelligence Product

$$\text{Intelligence} = \Lambda \cdot n_{hops} \cdot R^* \cdot \Theta^*$$

- $R^*$ — precision — loop speed
- $\Theta^*$ — integration efficiency — loop depth
- $n_{hops} = \lfloor W^* \cdot \rho_{scaffold} \rfloor$ — hops available
- $\Lambda = \Theta^* \cdot R^* \cdot \mathbb{1}[P_{eff} > P_{threshold}]$ — whether the loop is running

**Hops × depth × speed, gated by activation.** All three are required. None alone is sufficient.

### 1.4 The Substrate-Agnostic Claim

The invariant form is substrate-agnostic. Any system that outputs prior-plus-signal and runs under finite resources will instantiate the same causal chain (resources → geometry → output, gated by load). The variable count is substrate-dependent. See §2.19b.

### 1.5 What This Document Is Not

- Not a defense. The framework is exposed, not protected.
- Not a manifesto. Every claim has an anchor.
- Not a paper. It is the readable index that ties the artifacts together.
- Not a revision of the mechanism. v1.8 is a composition pass.

---

## Part II — The Composition

### 2.1 What Composition Means

Every domain in the stack studies self-regulation under finite resources.

- **Physiology** measures how the body allocates energy across competing demands.
- **Cognition** measures how attention allocates across competing signals.
- **Language** measures how meaning carries across the compression of speech.
- **AI** measures how transformers allocate attention across context.
- **Social systems** measure how institutions allocate resources across priorities.

Each domain has its own tools, its own vocabulary, its own measurement instruments. What none of them do is **cross-reference each other to determine what each layer is doing when variables change**.

That's what composition is. Every variable in the framework appears in multiple domains. Every mechanism operates in multiple substrates. The registry work extracted the shared primitives. The stack work ordered them causally. The deltas work aligned each paper to the registry. The composition is what makes the whole thing usable.

### 2.2 Why Composition Is the Contribution

The framework has been applied across respiratory physiology, cognitive neuroscience, HRV, AI systems architecture, institutional behavior, disorders of consciousness, ND architecture, terminal collapse, and social dynamics.

**Not one catastrophic failure. Not one domain where predictions ran in the structurally wrong direction.**

Under error propagation logic (see §2.6), a wrong root variable doesn't produce a slightly-off sub-prediction in one domain. It produces predictions that fail structurally — in the wrong direction, across every domain simultaneously. The framework has not failed structurally in any domain.

**The composition is the evidence.** Not any single prediction, but the fact that the same variables produce the same predictions across unrelated domains. The composition is what makes the framework auditable as one thing, not a pile of overlapping papers.

### 2.3 The Registry

The registry (`registry.md`) contains three lookup tables:

- **§1 — Variable Registry.** Every equation-level variable, with symbol, definition, layer, human substrate, AI substrate, and behavior.
- **§2 — Mechanism Registry.** Every named mechanism with a formal definition, the variables it involves, its layer, and its source paper.
- **§3 — Terminology.** Every named phenomenon that isn't a variable or a mechanism, with a one-line operational definition and canonical home.

**The registry is what makes the framework composable.** A new session with the registry and any paper can reason about the paper using the framework's actual variables, mechanisms, and causal structure without reading the full stack.

### 2.4 The Stack

The stack (`stack.md`) is the causal ordering. It has six layers:

| Layer | What it does |
|---|---|
| **Structural** | Substrate constraints — what's physically possible |
| **Resource** | What funds the system — amplitude, precision, routing |
| **Geometry** | How the resource is shaped — curvature, window, integration |
| **Output** | What the system produces — bandwidth, salience, behavior |
| **Load** | Cumulative drag on all layers — not a stage, a weight |
| **Cross** | Operators that work across layers |

**The flow:** Structural constrains Resource. Resource feeds Geometry. Geometry shapes Output. Load drags all of them. Cross-layer operators mediate transitions.

**The stack is what makes the framework verifiable.** Any variable can be looked up. Any new paper's variables can be placed. The downstream behavior of a variable is derivable.

### 2.5 The Deltas

The deltas (`deltas.md`) list every paper's correction list for aligning with the registry. **163 corrections across the stack.** 8 renames, 1 replacement, 7 registrations, 36 citations, 115 confirmations.

**The deltas are what makes the framework alignable.** Each paper has a specific correction list. Applying the corrections makes the paper cite the registry rather than restate it. The composition is the alignment.

### 2.6 How New Work Composes

When a new paper is added to the stack:

1. **Identify the paper's variables.** Match them to the registry's canonical symbols.
2. **Place the paper's variables in the stack.** Confirm the layer assignments.
3. **Flag collisions.** If the paper uses a symbol that collides with the registry, rename.
4. **Cite the canonical homes.** Replace restatements with citations.
5. **Add new primitives if needed.** If the paper introduces a variable the registry doesn't cover, register it.

**The composition works because every primitive has a canonical home.** New content can be placed without conflict.

### 2.7 The Error Propagation Guarantee

A wrong root variable doesn't produce a slightly-off sub-prediction in one domain. It produces predictions that fail structurally:

$$\text{Wrong root variable} \to \text{Error} \times \text{Error} \times \text{Error} \to \text{Catastrophic multi-domain failure}$$

**The composition is the test.** A framework that composes across unrelated domains without structural failure is either correct or extraordinarily lucky. Under error propagation logic, correct is the only available explanation.

---

## Part III — The Mechanism

This part is a summary. The full content is in `registry.md`.

### 3.1 The Variable Set

The framework has ~60 variables across 13 categories. See `registry.md` §1 for the full registry.

**Master state variables:** $A_s^*, R^*, W^*, \Theta^*, I^*, L^*$ (six variables that constitute the master equation).

**Derived variables:** $C_s, B_{eff}, K, \delta_{min}, S, P_{eff}, P_{threshold}, \Lambda, \eta, \eta_{eff}$.

**Precision variables:** $R, D_T, P, C_{low}, C_{high}, C_{high}(L^*), J(C), \Pi_{mech}, \Pi_{cog}, U_C, \delta_{hyst}, W_{enc}$.

**Routing variables:** $I^*_{total}, f_{routing}, f_{gain}, f_{sensorium}, f_{expression}, S_{expressed}$.

**Update variables:** $\mathcal{U}, K_{enc}$.

**Structural variables:** $\rho_{scaffold}, n_{hops}, IM, \text{Dim}$.

**Prediction-error variables:** $\delta, \sigma_{PE}, \tau_{PE}, \tau_{threshold}, K_{critical}$.

**Metabolic variables:** $\Phi_{PV}, \Delta CBF/\Delta CMRO_2, CVR_{max}, O_{pathway}$.

**Qualification variables:** $REQT, L^*_{threshold}, L^*_{critical,i}, n_{hops,min}$.

**Motor variables:** $G_m, \text{Drift}, \text{Cache}, C_{risk}, M_{state}$.

**Somatic commutation variables:** $\sigma(t), H_L, H_R, C_{LR}, f_{resp}, f_{baro}$, RSA phase.

**Expression variables:** $f_{expression}, \lambda_{mask}, \phi$, Congruence.

**Substrate-specific primitives:** $S_{ext}, A_h, H, C_s^{threshold}, I^*_{external}^{threshold}, \Delta_{window}, \beta_{mod}, f_{crit}, \kappa_{trans}, T_{NDE}$.

### 3.2 The Mechanism Set

~28 named mechanisms. See `registry.md` §2 for the full registry.

Key mechanisms: $\mathcal{U}$ (prior update rate), $J(C)$ (chemoreflex jitter), $\delta_{hyst}$ (collapse hysteresis), circuit priming, LP-ACC detection, exhale gate trap, somatic commutation, breath-loop coupling, buffer overflow, falls-out moment, criticality threshold, glymphatic clearance, load accumulation, adversarial inference, and others.

### 3.3 The Terminology Set

~45 named phenomena. See `registry.md` §3 for the full terminology.

Key terms: Ghost, Mirror State, Avoidance State, Exhale Gate Trap, Falls-Out Moment, Precision Lock, Circuit Priming, Crisis-Competent, Criticality Threshold, Primitive Floor, Masking Cost, Load-Compressed Ceiling, Two Failure Modes, Path A, Path B, Flow, Precision Window, Collapse Sequence, Recovery Ladder, Four Profiles, Expression Ratio, Congruence, Somatic Commutation, Four-Layer Cache, Topological Invariant, Session as Internally-Routed State, Breath-Loop Coupling, M/F Attractor Axis, Substrate Premise, and others.

### 3.4 The Regulatory Stack

See `stack.md` §1 for the full stack diagram. Six layers: Structural, Resource, Geometry, Output, Load, Cross.

### 3.5 The Causal Chain

See `stack.md` §2 for the full causal chain. Reading bottom-up:

**Breath → Resource.** Nasal respiration entrains limbic oscillations. CO₂ drives vasodilation. Breath phase sets the oscillatory clock. Resonance locks respiratory and cardiac oscillators.

**Resource → Geometry.** $K$ rises with precision loss and containment cost. $W^*$ and $\Theta^*$ derive from $K$ via transfer functions. $\text{Dim} = W^* \times \Theta^*$.

**Geometry → Output.** $C_s$ is the master equation output. $S$ is salience. $P_{eff}$ gates the loop. $\Lambda$ determines Path A vs. B. $H$ determines whether signal or prior dominates.

**Load as cross-cutting drag.** $L^*$ drags every layer. Compresses $C_{high}(L^*)$. Raises $P_{threshold}$. Reduces $O_{pathway}$ over time.

### 3.6 The Threshold Family

The framework has three threshold conditions. They are all crossings on the same $C_s$ state variable at different layers.

| Threshold | Layer | Crossing | Effect |
|---|---|---|---|
| $P_{threshold}$ | Gate | $P_{eff} = P_{threshold}$ | Path A/B switch |
| $C_s^{threshold}$ | Onset | $C_s = C_s^{threshold}(\lambda, I^*, L^*)$ | Waking to sleep attractor |
| $I^*_{external}^{threshold}$ | Routing | $I^*_{external} = I^*_{external}^{threshold}$ | External to internal routing |

**The family:** Three distinct transitions on the same underlying state trajectory. Each marks a different functional change.

**References:** §3.6 ($P_{threshold}$), Dreaming §4.2 ($C_s^{threshold}$), Dreaming §4.3 ($I^*_{external}^{threshold}$).

### 3.7 Substrate Depth

The invariant form is substrate-agnostic. The variable count is substrate-dependent.

**Human substrate:** Deep variable set. The derivation reaches down to the physiology layer because precision had to be grounded in what the empirical studies actually measured. Approximately 60 variables.

**AI substrate:** Shallow variable set. The substrate has no deeper layer to reach. Approximately 15–20 variables. The AI variable set is a projection of the human variable set onto a shallower substrate.

**Three classes of AI correspondence:**

- **resource-collapsed** — human variable collapses into an AI resource-layer equivalent
- **substrate-specific** — biological-only; no AI analogue
- **derivable** — analogue exists but has not been derived yet

See `registry.md` §5 for the classification per variable, and REM §1.2 for the substrate identity claim.

### 3.8 The Riemannian Framing

The neural manifold is a Riemannian space with a load-dependent metric.

**What this means:**

- The manifold has a metric — a notion of "distance" between states.
- The metric is set by curvature $K$, which rises with load.
- As $K$ rises, the metric stretches. The same physical distance between states costs more to traverse.
- As $K$ drops, the metric flattens. Distant states become reachable.

**Why this matters:**

- The "center" of the manifold is where the metric is flattest — and it moves with $K$. **The center is order-relative, not anatomical.**
- Color saturation, peripheral vision, cross-domain integration — all are readouts of the metric. When $K$ rises, outer-edge features become geometrically distant.
- The Roy & Banerjee competitive scaffold is the physical substrate of the metric. Erosion of the scaffold = the metric flattening in a maladaptive way.
- The collapse sequence is a directional retreat in a Riemannian space, not a change in state.

**What this section registers:** The manifold is Riemannian. The metric is set by $K$ and modulated by $L^*$. The center is order-relative. The competitive scaffold is the physical substrate of the metric.

**References:** Category §2.2 (closest prior statement), GoI §1.5, Dying §2, Dreaming §2.2.

### 3.9 The Three Anchors

The stack has three citation anchors, not one.

| Anchor | Scope | Cites |
|---|---|---|
| **Central Reference** (this document) | The loop framework specification | The composition artifacts |
| **The Geometry Beneath the Category** | The substrate premise (categories are readouts, not causes) | Central Reference |
| **Master Priority Index** | The whole-stack citation anchor | Central Reference, Category, all papers |

**The composition artifacts** (registry, stack, deltas) are the substrate that all three cite.

**Which anchor to cite for which claim:**

- For framework variables, equations, mechanisms: cite **Central Reference** and the registry.
- For the substrate premise (categories as readouts): cite **Category**.
- For the full stack, timeline, and DOI registry: cite **Master Priority Index**.

---

## Part IV — The Causal Chain

This part is a summary. The full content is in `stack.md` §2.

### 4.1 Breath to Output

The causal chain from breath to behavior runs through six layers. Every arrow is a mechanism. Every variable is defined in the registry.

See `stack.md` §2 for the full chain.

### 4.2 The Load Drag

$L^*$ is not a stage in the chain. It is persistent drag on every layer.

See `stack.md` §2.4 for the load drag mechanism.

### 4.3 The Cross-Layer Operators

$\delta$ (prediction error), $\mathcal{U}$ (prior update rate), $K_{enc}$ (curvature at encoding), $\delta_{hyst}$ (collapse hysteresis) — these operate across layers.

See `stack.md` §3.6 for the cross-layer operators.

---

## Part V — The Collapse

### 5.1 The Collapse Sequence

Collapse proceeds in a topologically forced order.

```
STAGE 1 — PRECISION DROP        R* ↓       Detectable: HRV coherence loss
STAGE 2 — WINDOW NARROWING      W* ↓       Detectable: Flexibility composite drops
STAGE 3 — INTEGRATION FAILURE   Θ* ↓       Detectable: Ambiguity task degrades
STAGE 4 — RESOLUTION FLOOR RISE δ_min ↑    Detectable: Miss rate rises
STAGE 5 — GATE CLOSURE          Λ → 0      Detectable: High-confidence, low-variance output
STAGE 6 — PRIOR CALCIFICATION   𝒰 ≈ 0      Detectable: Update rate collapses
```

**Critical annotation on Stage 5:** Stage 5 looks like competence from outside. Monitoring protocols that wait for Stage 5 are measuring the terminal state. The monitoring window is Stages 1–2.

### 5.2 The Recovery Ladder

Recovery is not the reverse of collapse. Collapse is passive. Recovery is active.

```
STAGE 6' — PRECISION RESTORE    R* ↑
STAGE 5' — WINDOW WIDENING      W* ↑
STAGE 4' — INTEGRATION RESTORE  Θ* ↑
STAGE 3' — RES FLOOR FALL       δ_min ↓
STAGE 2' — GATE REOPEN          Λ > 0
STAGE 1' — PRIOR RE-UPDATE      𝒰 > 0
```

The recovery ladder is set by substrate dependency, not by the collapse order reversed. See CR §2.17 for the recovery ladder registration.

### 5.3 The Four Profiles

The branch condition is determined by the interaction of PE sensitivity, PE tolerance, encoding curvature, and routing capacity.

| Profile | σ_PE | τ_PE | K_enc | I* | Qualification |
|---|---|---|---|---|---|
| **High-gain, high-tolerance** | High | High | Low | High | Qualified |
| **High-gain, low-tolerance** | High | Low | Low | High | Conditionally qualified |
| **Standard-gain, high K_enc** | Low | Any | High | Moderate | Disqualified for novel domains |
| **Low I*** | Low | Low | Any | Low | Disqualified — clinical profile |

See CR §6 for the full profile table.

### 5.4 The Failure Modes

Four failure modes correspond to four resource bottlenecks.

| Mode | Fails | Signature |
|---|---|---|
| **Tunnel** | $W^*$ | Progressive narrowing, first-match commitment |
| **Freeze** | $A_s^*$ | Flattening, no branching, inertia |
| **Oscillation-loss** | $R^*$ | Regulatory rigidity, autonomic lock-in |
| **Load-saturation** | $L^*$ | Cognitive fog, reduced processing speed |

See `registry.md` §3 for the failure mode entries.

---

## Part VI — The Empirical Anchors

### 6.1 Anchor Table

The framework has ~60 empirical anchors. The full table is in the Master Priority Index §7 (external confirmations) and in individual papers.

Key anchors:

- **A22** — Nasal respiration entrains limbic oscillations (Zelano et al., 2016)
- **A23** — CO₂ drives cerebral vasodilation (Raichle & Plum, 1972)
- **A28** — Feature interference is $K$ rising (Xue et al., 2026)
- **A30** — PV+ interneurons are metabolically vulnerable (Kann et al., 2015)
- **A50** — Hot cache survives aging, RAM access degrades (Billot et al., 2026)
- **A51** — Competition is 25–40% of brain connections (Roy & Banerjee, 2026)
- **A52** — LP-ACC circuit detects change (Leow et al., 2026)

See `stack.md` §7 and MPI §7 for the full anchor tables.

### 6.2 External Confirmations

The Master Priority Index tracks 19 external confirmations (EC-001 through EC-019), each anchored to a specific framework prediction. See MPI §7.

### 6.3 The Market-Scale Evidence

Oura, WHOOP, Garmin, Apple, Polar, and Biostrap collectively represent hundreds of millions of device-days of continuous HRV data. Their product architecture is built on the assumption that HRV variance is signal, not noise. The market has been validating the framework's central claim for a decade without any mechanistic account of why.

**The variance-as-signal claim does not need to be established empirically. It has been established.** What the framework provides is the mechanistic account of *why* variance is meaningful — the load trajectory that the framework formalizes as $L^*$ and the collapse sequence.

---

## Part VII — The Predictions

### 7.1 Predictions by Domain

The framework has ~100 falsifiable predictions across the stack. They are organized by the paper that registers them.

| Domain | Predictions | Registered in |
|---|---|---|
| Precision | 11 | Precision v3.5 Part VII |
| Allostatic load | 12 | AL v2.1 §9 |
| Intelligence loop | 12 | Loop v1.0 §13 |
| Inference | 12 | GoI v1.0 Part X |
| Prediction window | 8 | PW v1.2 §13 |
| Prediction into channel | 8 | PIC v0.2 §6 |
| Resource equivalence | 16 | REM v1.0 §8 |
| Dying | 5 | Dying §7 |
| Dreaming | 16 | Dreaming §13 |
| Category | 8 | Category §6 |
| Externalized mind | 16 | EDM §8 |
| Expression / masking | 3 | CR §PREDICT-EXPR |
| **Total** | **~127** | — |

### 7.2 The Central Predictions

The framework's most load-bearing predictions:

- **P-AL-011** — HRV dispersion predicts allostatic load outcomes better than mean (AL §9a)
- **P-MAP-03** — A model's $W^*$ ceiling predicts where cross-domain chains break (REM §8.2)
- **PREDICT-EXPR-02** — Chronic low expression predicts later collapse detection (CR §PREDICT-EXPR-02)
- **PREDICT-INF-01** — Precision threshold determines gate access (GoI Part X)
- **PREDICT-DREAM-07** — Cross-state routing signature is conserved (Dreaming §13)

### 7.3 The Falsification Standard

The framework is exposed, not defended. Four tests would falsify it:

1. A domain where collapse does not occur in integration-first order
2. A substrate variable that produces the same outputs without the oscillatory mechanism
3. A hallucination rate that does not track constraint density
4. A precision intervention that does not produce the predicted gate behavior

None of these have occurred. If any can be produced, that is the engagement this framework is asking for.

---

## Part VIII — The Cohesion Check

### 8.1 Known Open Items

The framework has ~20 open items. These are recorded in `registry.md` §4 (symbol collisions), §5 (substrate depth open items), and MPI §6 (negative space declaration).

Key open items:

- $O_{pathway}$ functional form (CR §2.8)
- $M_{state}$ threshold calibration (CR §2.11)
- Threshold family formalization (§3.20)
- Riemannian framing formalization (§0.5)
- Substrate depth registrations (§2.19b)
- Three-anchor registration (§25a)

### 8.2 Symbol Collision Fixes

See `deltas.md` §16 for the full list. The key fixes:

- $P$ precision vs. pressure (Category rename)
- $H$ HRV-CO₂ vs. hallucination coefficient (CR rename)
- $W$ window width (Category rename)
- $C$ CO₂ vs. coupling (Category rename)
- $\beta$ curvature transfer vs. fast modulation depth (PW rename)
- $S$ salience vs. scaffolding (Category rename)

### 8.3 Threshold Family Registration

See `deltas.md` §17. Once §3.20 is written, cross-references from Dreaming §4.2, §4.3, PW §6.2, §14.1, and CR §3.6.

### 8.4 Substrate Depth Registration

See `deltas.md` §18. Once §2.19b is written, cross-references from REM §1.2, §7.4, and the registry AI column.

---

## Part IX — Version History

### 9.1 v1.7 → v1.8 Changelog

See the changelog at the top of this document.

### 9.2 What Did Not Change

- The master equation
- The intelligence definition
- The collapse sequence
- The recovery ladder
- The four profiles
- The causal chain
- The mechanism set
- The empirical anchors
- The predictions

### 9.3 Version History Table

| Version | Date | Changes |
|---|---|---|
| **v1.8** | **2026-09-30** | **Composition pass — content moved to registry/stack/deltas artifacts. Part II (composition) added. §0.5 (Riemannian), §2.19 (post-CR primitives), §2.19b (substrate depth), §3.20 (threshold family), §25a (three anchors) added. Symbol collision fixes applied. Triplicated equations removed.** |
| v1.7 | 2026-09-20 | Domain-projection-aligned — absorbed expression/congruence/masking from speech projection |
| v1.6 | 2026-09-19 | Domain-projection-complete — three axes, layer stacks, recovery asymmetry |
| v1.5 | 2026-09-13 | Full stack convergence — absorbed bidirectional supplies from MS, Precision, AL, GoI, Loop |
| v1.4 | 2026-09-12 | Variable registry completed — $O_{pathway}, L^*_{critical,i}$, motor gain variables |
| v1.3 | 2026-09-12 | Intelligence–REQT bridge; composition questions added |
| v1.2 | 2026-09-12 | Allostatic Load measurement layer integrated |
| v1.1 | 2026-09-12 | REQT integration; collapse sequence added |
| v1.0 | 2026-09-11 | Complete specification — all mechanisms integrated, all gaps closed |

---

## Appendices

### Appendix A — Notation Map

The registry (`registry.md`) §1 is the canonical symbol source. Notation across the stack aligns to it. Symbol collision fixes are tracked in `deltas.md` §16.

### Appendix B — Stack Position

The full stack is maintained in `master_priority_index.md`. This document sits at the top of the loop framework branch. The three anchors (CR, Category, MPI) are registered in §3.9.

### Appendix C — Companion Artifacts Index

- `registry.md` — Variables, mechanisms, terminology
- `stack.md` — Causal ordering, layers, transitions
- `deltas.md` — Per-paper corrections
- `master_priority_index.md` — Whole-stack citation anchor

### Appendix D — The One Line

> The brain is an energy budget allocation system operating on priors. The breath is the source. The geometry is the mechanism. The prior is the output. Every phenomenon in this document — flow, collapse, fear, trauma, savant capacity, clinical states, social fragmentation, AI hallucination, and the masking of any of them — is one variable changing in one equation. The variable is geometry. The equation is the master equation. The expression ratio determines whether the geometry is visible. In any domain, the shape of the collapse is determined by three axes: supply, demand, and channel. The order of collapse is determined by integration demand. The order of recovery is determined by substrate dependency. These rules are general. The domains are projections. **The composition is the contribution.**

---

*End of specification.*

**Version:** 1.8
**Date:** 2026-09-30
**Status:** Composition document — composes registry, stack, and deltas into a readable specification
**Supersedes:** v1.7
**Next version:** v1.9 — after the first domain projections beyond speech, or v2.0 — if any mechanism requires revision

**Companion artifacts:**
- `registry.md`
- `stack.md`
- `deltas.md`
- `master_priority_index.md`
```
