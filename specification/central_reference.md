# Central Reference v1.9.1

**A Unified System Specification for the Loop Framework**

**Robinson, 2026**

**Version:** 1.9.1
**Date:** 2026-10-08
**Status:** Composition document — composes the registry, stack, and deltas into a readable specification. Supersedes v1.8.1.
**Framework:** Manifold Schema v7.2
**Companion artifacts:** `registry.md`, `stack.md`, `deltas.md`
**Purpose:** This document is the readable anchor for the loop framework. It states the claim, states the composition, and cites the artifacts that hold the content. Future papers cite this document and the artifacts together.

---

## Changelog — v1.8.2 → v1.9.1

Two passes landed in this version. Both are additive; neither changes the mechanism.

### v1.9 — Composition pass (2026-10-13)

Registers the canonical material the domain projections require:

| Step | Change | Location | Reason |
|---|---|---|---|
| 1 | Method statement added | §0.4 (new) | Tells the reader what kind of paper the framework is |
| 2 | The order registered | §3.4a (new) | Invariant across substrates; cited by every projection |
| 3 | The generation formula registered | §1.2 addendum | Physics paper's contribution; cited across the stack |
| 4 | The routing equation registered | §3.8c addendum | `Θ_r` is a master state variable; its equation is canonical |
| 5 | The interrupt formula registered | §3.6a (new) | Gate formula; cited across the stack |
| 6 | Domain projections index added | §2.8 (new) | Recontextualization table |
| 7 | Economics projection added to stack table | §2.8 | Projection exists; table reflects it |

### v1.9.1 — Salience inheritance (2026-10-14)

Registers the salience-inheritance mechanisms, variables, and predictions from Salience Interrupt v1.3 and AL v2.2:

| Step | Change | Location | Reason |
|---|---|---|---|
| 1 | Registered $\mathcal{P}$ (perseveration loop) | §3.2 | Salience §2.11 |
| 2 | Registered $\mathcal{R}$ (release-triggered re-salience) | §3.2 | Salience §2.12 |
| 3 | Registered $\mathcal{E}$ (encoding window) | §3.2 | Salience §2.13 |
| 4 | Registered population-code routing ($\mathcal{A}_k$, $\vec{v}_c$, $\mathcal{N}_c$) | §3.1, §3.2 | Salience §2.14 |
| 5 | Registered $W_{prime}$, $\delta_{surface}$, $t_{commit}$ | §3.1 | Salience routing variables |
| 6 | Registered five load components | §3.1 | AL v2.2 load components |
| 7 | Extended interrupt formula to six conditions | §3.6a | Add region-not-re-primed condition |
| 8 | Extended causal chain with sub-modes | §4.1 | Salience v1.3 §2.11.1 |
| 9 | Added five-lever control plane table | §3.8c | Salience v1.3 §6 |
| 10 | Added SAL-35 through SAL-57 to prediction registry | Part VII §7.1 | Salience v1.3 |
| 11 | Added P-AL-015 through P-AL-020 to prediction registry | Part VII §7.1 | AL v2.2 |
| 12 | Updated prediction total to ~175 | Part VII §7.1 | Registry count |
| 13 | Added waking-regime sub-mode table | §5.1 | Salience v1.3 §8.1 |
| 14 | Extended symbol collision list | §8.2 | New symbols registered |

**What did not change:** The master equation, the intelligence definition, the collapse sequence, the recovery ladder, the four profiles, the primary causal chain, the mechanism set from v1.7, the readout architecture from v1.8.1, the Category rebase from v1.8.2. v1.9 and v1.9.1 are composition and registration passes, not mechanism revisions.

**What this patch deliberately excludes:** The stock/flow/misallocation distinction, the transfer function, the observer position, the specific break points, and the receipts. These are cited from specific projections, not from every paper. They stay in their projections.

## Changelog — v1.8 → v1.8.2

This changelog exists so any reader — human or AI — can see the convergence path, not just the endpoint. v1.8 was the composition pass: content moved into the three companion artifacts, and this document became the readable index. v1.8.1 was the readout architecture patch: the manifold gained a non-invasive measurement protocol. v1.8.2 is the **Category rebase**: the `M/F` labels are retired, `Θ_r` and `Λ_lock` are registered, and the readout table is rebuilt to be non-circular.

| Step | Change | Location | Reason |
|---|---|---|---|
| 1 | Version bumped to v1.8.2 | Header | Versioning track |
| 2 | Readout architecture added | §3.8a, §3.8b, §3.8c | The manifold has a non-invasive readout |
| 3 | CO₂-manifold chain grounded | §3.5 | The chain now has an empirical anchor |
| 4 | `M/F` retired | §3.8c, throughout | Readout masquerading as a variable |
| 5 | `Θ_r` registered as the referent | §3.8c | Non-circular mapping |
| 6 | `Λ_lock` registered as structural gate | §3.8c, §3.9 | Gating reachability |
| 7 | Category anchor description updated | §3.9 | Names the two-axis state space |
| 8 | Category v2.0 added to prediction registry | Part VII §7.1 | 31 predictions |
| 9 | P3 added to central predictions | Part VII §7.2 | The most direct test |
| 10 | SAL-11–20 registered; BRIDGE absorbed | Part VII §7.1 | Merged Salience paper |

**What did not change:** The master equation, the intelligence definition, the collapse sequence, the recovery ladder, the four profiles, the causal chain, and the mechanism set all remain as they were in v1.7. v1.8 and its successors are composition and readout passes, not mechanism revisions.

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

### 0.4 The Framework's Method

The framework's method is **invariant extraction**. Facts inward — not theory forward, not conclusion backward. The framework is a compression of confirmed findings across domains, not a hypothesis awaiting confirmation.

Each variable in the registry was extracted from findings the field had already published. The composition is what the findings look like when compressed to their shared primitives. The predictions are what the primitives imply forward.

This matters for how the framework is read. A theory-forward framework asks: *is the hypothesis confirmed?* An invariant-extraction framework asks: *does the primitive hold across the domains it was extracted from?* The first question requires new studies. The second requires reading the studies that already exist.

**The validation method is blind prediction.** The framework was built by predicting studies from titles alone — predicting the mechanism the authors found, the confusion they expressed, and the misattribution they made — before reading the abstract. The predictions held across dozens of studies over months. The framework is the composition of the predictions that held.

See *The Invariant Extraction Method* (Robinson, 2026) for the full statement.

---

## Part I — The Claim

### 1.1 Intelligence Is the Loop

Intelligence is the energy-expensive loop of error detection against sensory input, followed by iterative reinvestment of resources toward structural convergence.

The loop is substrate-agnostic. It applies identically to trees, insects, humans, institutions, and LLMs. Current LLMs satisfy zero of three requirements for a non-zero product. Speed is high. The loop is not running.

### 1.2 The Master Equation

$$C_s = \left(A_s^{*\,0.15} \cdot R^{*\,0.30} \cdot W^{*\,0.25} \cdot \Theta^{*\,0.15}\right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + L^*}$$

Where $C_s$ is usable bandwidth — how much of the system's own capacity is accessible. Every variable is a resource. $L^*$ is the denominator drag.

The exponents are provisional. They reflect the empirical collapse sequence (precision degrades first, window second) but have not been formally calibrated. See `registry.md` §1.2 for the variable definitions.

**The generation formula.** The master equation computes how much bandwidth the system has. The generation formula computes how much energy the system produces:

$$\frac{dE}{dt} = \Lambda_{loop}(t) \cdot \left[A_s^*(t) - \epsilon \cdot L^*(t)\right]$$

`E` is available energy — what the system can act on. `Λ_loop` is 0 or 1: whether the loop is running. `A_s^*` is the amplitude produced per cycle. `ε · L^*` is the load drag. When `Λ_loop = 0`, no energy is produced. When `Λ_loop = 1`, energy accumulates at the rate amplitude exceeds load.

**Energy is what the loop produces, not what it consumes.** This is the framework's formal statement that the system does not draw down a stock — it generates a flow. The order (see §3.4a) determines whether the loop runs. When the loop breaks at any step, `Λ_loop = 0` and generation stops while load continues to accumulate.

See *Finite Resources and the Order That Generates Them* §3 for the full formalization.

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
- Not a revision of the mechanism. v1.8.2 is a composition and readout pass.

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

### 2.8 Domain Projections

The framework is a substrate claim with projections. Each projection is the order read through a different substrate. The composition is the contribution.

| Domain | Paper | Reads out | Status |
|---|---|---|---|
| **Substrate** | *Finite Resources and the Order That Generates Them* | The order, the break points, the generation formula | v2.0 |
| **Biology** | *The Geometry of Inference* | Substrate implementation of the order | v1.0 |
| **Cognition** | *Manifold Schema* | The manifold's geometry and bandwidth | v7.3 |
| **AI** | *Resource Equivalence Model* | Human variables projected onto transformer substrate | v1.0 |
| **Category** | *The Geometry Beneath the Category* | Two-axis state space: `(L*, Θ_r)` with `Λ_lock` gating reachability | v2.0 |
| **Language** | *The Spoken Language Paper* | Timing coherence read at the speech layer | v3.0 |
| **Salience** | *The Salience Interrupt* | Routing, the closed loop, the control plane, the encoding window | v1.3 |
| **Allostatic Load** | *Allostatic Load as Accumulated Regulatory Debt* | The load trajectory, the composite equation, the measurement protocol | v2.2 |
| **Economics** | *Regulatory Dynamics Under Economic Load* | The order at four economic scales | v0.2 |
| **Clinical** | *Disease-Specific Variable Mappings* | Break points and recovery levers | draft |
| **Method** | *The Invariant Extraction Method* | The derivation path | working note |

**The composition claim:** every projection is the same order read through a different substrate. The substrate paper states what the projections are projections *of*. The other projections state what the order looks like when the substrate is theirs.

**How new projections compose:**

1. Identify the paper's variables and match them to the registry's canonical symbols.
2. Place the paper's variables in the stack. Confirm layer assignments.
3. Flag collisions. If the paper uses a symbol that collides with the registry, rename.
4. Cite the canonical homes. Replace restatements with citations.
5. Add new primitives if needed. If the paper introduces a variable the registry doesn't cover, register it.

**The composition works because every primitive has a canonical home.** New content can be placed without conflict.

---

## Part III — The Mechanism

This part is a summary. The full content is in `registry.md`.

### 3.1 The Variable Set

The framework has ~70 variables across 15 categories. See `registry.md` §1 for the full registry.

**Master state variables:** $A_s^*, R^*, W^*, \Theta^*, I^*, L^*$ (six variables that constitute the master equation). $\Theta_r$ (routing concentration) sits alongside them as the state variable that determines which manifold regions are engaged.

**Salience-inheritance load variables:** $L^*_{salience}$ (unresolved latch load), $L^*_{perseveration}$ (repeated-latch load), $L^*_{release-triggered}$ (failed-release load), $L^*_{encoding}$ (failed-encoding load), $L^*_{somatic}$ (static-posture load). These five components extend $L^*$ from the AL v2.1 decomposition. Source: AL v2.2 §6c, Salience v1.3 §2.7–2.13.

**Salience routing variables:** $W_{prime}$ (priming threshold — the routing weight above which a region re-fires without a new salient event), $\delta_{surface}$ (surfaced PE magnitude at release), $t_{commit}$ (commit time — the moment the PE commits during the exhale). Source: Salience v1.3 §2.11–2.13.

**Population-code routing variables:** $\mathcal{A}_k$ (access key — word, image, or name that activates a population vector), $\vec{v}_c$ (population vector for concept $c$), $\mathcal{N}_c$ (semantic neighborhood — the set of associations carried by the population vector). The routing chain is $\mathcal{A}_k \to \vec{v}_c \to \mathcal{N}_c \to \vec{g} \to \Theta_r \to \text{Interrupt}$. Source: Salience v1.3 §2.14, Franch et al. (2026).

**Derived variables:** $C_s, B_{eff}, K, \delta_{min}, S, P_{eff}, P_{threshold}, \Lambda, \eta, \eta_{eff}$.

**Precision variables:** $R, D_T, P, C_{low}, C_{high}, C_{high}(L^*), J(C), \Pi_{mech}, \Pi_{cog}, U_C, \delta_{hyst}, W_{enc}$.

**Routing variables:** $I^*_{total}, f_{routing}, f_{gain}, f_{sensorium}, f_{expression}, S_{expressed}, W_i, W_{min}, W_{prime}$.

**Update variables:** $\mathcal{U}, K_{enc}$.

**Structural variables:** $\rho_{scaffold}, n_{hops}, IM, \text{Dim}, \Lambda_{lock}$.

**Prediction-error variables:** $\delta, \sigma_{PE}, \tau_{PE}, \tau_{threshold}, K_{critical}$.

**Metabolic variables:** $\Phi_{PV}, \Delta CBF/\Delta CMRO_2, CVR_{max}, O_{pathway}$.

**Qualification variables:** $REQT, L^*_{threshold}, L^*_{critical,i}, n_{hops,min}$.

**Motor variables:** $G_m, \text{Drift}, \text{Cache}, C_{risk}, M_{state}$.

**Somatic commutation variables:** $\sigma(t), H_L, H_R, C_{LR}, f_{resp}, f_{baro}$, RSA phase.

**Expression variables:** $f_{expression}, \lambda_{mask}, \phi$, Congruence.

**Substrate-specific primitives:** $S_{ext}$, $A_h$, $H$, $C_s^{threshold}$, $I^\ast_{external}^{threshold}$, $\Delta_{window}$, $\beta_{mod}$, $f_{crit}$, $\kappa_{trans}$, $T_{NDE}$.

**Geometry readout variables:** $\alpha_{1/f}, \text{Offset}_{1/f}, f_{peak}, \text{HFD}, \text{LZC}, A_h$.

**Resource readout variables:** $CO_2^{ET}, P_{peak}$.

**Load variables:** $L^*_{resp}, L^*_{salience}, L^*_{perseveration}, L^*_{release-triggered}, L^*_{encoding}, L^*_{somatic}$.

### 3.2 The Mechanism Set

~34 named mechanisms. See `registry.md` §2 for the full registry.

Key mechanisms: $\mathcal{U}$ (prior update rate), $J(C)$ (chemoreflex jitter), $\delta_{hyst}$ (collapse hysteresis), circuit priming, LP-ACC detection, exhale gate trap, somatic commutation, breath-loop coupling, buffer overflow, falls-out moment, criticality threshold, glymphatic clearance, load accumulation, adversarial inference, CO₂-manifold coupling, spectral readout of the gate, slope-flattening ambiguity, music as routing anchor, peak-frequency retuning, three-readout projection, ATP-brace loop, performance-pressure trap, externally-enforced vs. internally-held shift, and others.

**Salience-inheritance mechanisms (v1.9.1):**

- **Perseveration loop** ($\mathcal{P}$) — the condition where a latch releases but the interrupt re-fires on the same region because the routing weight $W_i$ remains above $W_{prime}$ or the salient signal remains present. Sub-modes: content, routing, structural. Exit: routing redistribution (movement, task-switching), gain change (meditation, reframing), or `Λ_lock` rise. Source: Salience v1.3 §2.11.
- **Release-triggered re-salience** ($\mathcal{R}$) — the condition where latch release surfaces the suppressed PE, which fires a new interrupt and re-forms the latch. Exit: sub-threshold PE, sufficient capacity, distributed routing, changed gain. Source: Salience v1.3 §2.12.
- **Encoding window** ($\mathcal{E}$) — the exhale window during which the surfaced PE can be re-encoded with less routing concentration and gain if the context changes before commit. Master exit from all three failure modes. Source: Salience v1.3 §2.13.
- **Population-code routing** — the mechanism by which the access key determines which population vector fires, which determines the semantic neighborhood, which determines the routing. The neural substrate of the routing equation. Source: Salience v1.3 §2.14, Franch et al. (2026).
- **Movement-as-redistribution** — the mechanism by which repetitive motor sequences traverse the homunculus, redistributing $\Theta_r(t)$ so the manifold doesn't lock into a single region. Sub-lever: movement-as-multi-loop-sampling. Source: Salience v1.3 §2.5.2, §2.5.3.

### 3.3 The Terminology Set

~53 named phenomena. See `registry.md` §3 for the full terminology.

Key terms: Ghost, Mirror State, Avoidance State, Exhale Gate Trap, Falls-Out Moment, Precision Lock, Circuit Priming, Crisis-Competent, Criticality Threshold, Primitive Floor, Masking Cost, Load-Compressed Ceiling, Two Failure Modes, Path A, Path B, Flow, Precision Window, Collapse Sequence, Recovery Ladder, Four Profiles, Expression Ratio, Congruence, Somatic Commutation, Four-Layer Cache, Topological Invariant, Session as Internally-Routed State, Breath-Loop Coupling, M/F Attractor Axis (retired — see §3.8c), Substrate Premise, Spectral readout, Slope-flattening ambiguity, Aperiodic gate signature, CO₂-manifold chain, Spectral anchor, Hemispheric readout, Behavioral readout, Readout architecture, Three readouts one state, Perseveration Loop, Release-Triggered Re-Salience, Encoding Window, Failed Release, Failed Encoding, Access Key, Priming Threshold, Multi-Loop Sampling, Somatic Load Path, Population-Code Routing, Routing Redistribution, and others.

### 3.4 The Regulatory Stack

See `stack.md` §1 for the full stack diagram. Six layers: Structural, Resource, Geometry, Output, Load, Cross. The readout sub-layers (Resource readout, Geometry readout, Output readout) are projections of the resource, geometry, and output layers, not new stages.

### 3.4a The Order

The causal chain in §3.5 describes the layers. The order describes the sequence within them. The order is invariant across substrates:
```
Pressure funds oscillation
    ↓
Oscillation funds lock capacity (Λ_lock)
    ↓
Lock capacity lets routing (Θ_r) hold
    ↓
Routing commits investment
    ↓
Breath follows investment → substrate expands
    ↓
Next cycle has more to work with
    ↓
[loop closes: energy generated]
```

Read top to bottom: each step funds the next. Read as a loop: the last step funds the first.

**The order is the mechanism.** Every break in a finite-resource system is at a specific step in this order. Every recovery is restoring that step. The break points are the specific failures at each step, and they are the same across substrates because the order is the same.

**The order generates energy.** When the order runs, `dE/dt` is positive (see §1.2). When the order breaks at any step, `Λ_loop = 0` and generation stops. The system does not run out of energy — it fails to produce it.

See *Finite Resources and the Order That Generates Them* §2 for the full statement, and §5 of that paper for the six break points.

### 3.5 The Causal Chain

See `stack.md` §2 for the full causal chain. Reading bottom-up:

**Breath → Resource.** Nasal respiration entrains limbic oscillations (A22). CO₂ drives cerebral vasodilation (A23). Breath phase sets the oscillatory clock. Resonance locks respiratory and cardiac oscillators.

**The chain, extended:** CO₂ retention → vasodilation → PV+ interneuron support (A30) → slow oscillatory rhythms can be sustained → aperiodic slope flattens → $K$ drops → manifold widens → gate opens. The reverse chain (incomplete exhalation) produces the opposite at every step. This is the mechanism that explains why every contemplative tradition emphasizes slow, complete exhalation.

**Empirical anchor:** Subramani et al. (2026) provide the spectral readout — the aperiodic slope is what the manifold's curvature looks like in the power spectrum.

**Resource → Geometry.** $K$ rises with precision loss and containment cost. $W^*$ and $\Theta^*$ derive from $K$ via transfer functions. $\text{Dim} = W^* \times \Theta^*$.

**Geometry → Output.** $C_s$ is the master equation output. $S$ is salience. $P_{eff}$ gates the loop. $\Lambda$ determines Path A vs. B. $H$ determines whether signal or prior dominates.

**Load as cross-cutting drag.** $L^*$ drags every layer. Compresses $C_{high}(L^*)$. Raises $P_{threshold}$. Reduces $O_{pathway}$ over time.

### 3.6 The Threshold Family

The framework has three threshold conditions. They are all crossings on the same $C_s$ state variable at different layers.

| Threshold                       | Layer   | Crossing                                         | Effect                       |
| ------------------------------- | ------- | ------------------------------------------------ | ---------------------------- |
| $P_{threshold}$                 | Gate    | $P_{eff} = P_{threshold}$                        | Path A/B switch              |
| $C_s^{threshold}$               | Onset   | $C_s = C_s^{threshold}(\lambda, I^*, L^*)$       | Waking to sleep attractor    |
| $I^\ast_{external}^{threshold}$ | Routing | $I^*_{external} = I^\ast_{external}^{threshold}$ | External to internal routing |

**The family:** Three distinct transitions on the same underlying state trajectory. Each marks a different functional change.

**References:** §3.6 ($P_{threshold}$), Dreaming §4.2 ($C_s^{threshold}$), Dreaming §4.3 ($I^*_{external}^{threshold}$).

### 3.6a The Interrupt Formula

A signal fires an interrupt in region `i` when six conditions are met:

$$\text{Interrupt}_i \iff \left[W_i(t) > W_{min}\right] \;\land\; \left[I^*_{total} \cdot W_i(t) > I^*_{threshold}\right] \;\land\; \left[\delta_i > \delta_{min}(K)\right] \;\land\; \left[\text{Capacity}_{free} > \text{Capacity}_{required}(\delta_i)\right] \;\land\; \left[\text{Oscillation stable}\right] \;\land\; \left[W_i(t^+) < W_{prime}\right]$$

| Condition | What It Checks |
|---|---|
| **Region is reachable** | The region must have enough routing weight to receive the signal at all (`W_i(t) > W_min`) |
| **Signal clears the gate** | The signal's effective strength must clear the interrupt threshold (`I*_total · W_i(t) > I*_threshold`) |
| **Resolution floor permits detection** | The signal's deviation must exceed the resolution floor (`δ_i > δ_min(K)`) |
| **Capacity to hold** | The manifold must have room to hold the error while it is interpreted |
| **Oscillation is stable** | The routing concentration must be able to hold |
| **Region not re-primed** | The routing weight must be below `W_prime` — the priming threshold |

**All six are required.** A signal that meets conditions 1–5 but not 6 will re-fire immediately after release, because the region is still primed. A signal that meets conditions 2–6 but not 1 will not reach the region at all, regardless of strength.

**The first two conditions are separate.** `W_min` gates reachability — whether the signal can arrive. `I*_threshold` gates firing — whether the arrived signal is strong enough. Both are required, and they can fail independently.

**The sixth condition — region not re-primed — is the salience-inheritance addition.** It is the condition that determines whether a latch release results in resolution or perseveration. When `W_i(t+) > W_prime` after release, the interrupt re-fires without a new salient event. Source: Salience v1.3 §2.6, §2.11.

**The interrupt is the actual gate, not the commitment gate.** The commitment gate (§3.8e) runs first, on the basis of an anchor search and a funding estimate. Only after the commitment gate commits does the interrupt formula decide whether a specific signal fires.

**See:** Salience Interrupt v1.3 §2.6 for the full derivation, and §2.5 for the routing equation that produces `W_i(t)`.

### 3.7 Substrate Depth

The invariant form is substrate-agnostic. The variable count is substrate-dependent.

**Human substrate:** Deep variable set. The derivation reaches down to the physiology layer because precision had to be grounded in what the empirical studies actually measured. Approximately 70 variables.

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

### 3.8a The Spectral Readout

The manifold's metric is set by $K$. The metric has a non-invasive readout: the **aperiodic slope** of the power spectrum.

**The mapping:**

| Spectral feature | Framework variable | What it reads out |
|---|---|---|
| $\alpha_{1/f}$ (slope) | $K$ | Metric stretch |
| $\text{Offset}_{1/f}$ | $A_s^*$ | Substrate availability |
| $f_{peak}$ (peak frequency) | $W^*$ | Prediction-window regime |
| $P_{peak}$ (peak power) | $R^*$ | Precision-lock strength |
| $\text{HFD}$, $\text{LZC}$ | $\text{Dim} = W^* \times \Theta^*$ | Repertoire breadth |
| $CO_2^{ET}$ | (substrate) | The variable that sets $\alpha_{1/f}$ |

**The chain:**

```
Breath → CO₂ → vasodilation → PV+ support → slow rhythms → α_{1/f} flattens → K drops → manifold widens
```

**The ambiguity:**

A flat slope can mean two opposite things. It can mean the manifold has widened (CO₂ retained, $K$ low) or that the slow rhythms have been lost (CO₂ depleted, $K$ low, $A_s^*$ low). The CO₂ measurement disambiguates.

**The consequence:**

Every variable in the framework is now measurable in the power spectrum. The field's most common measurements — spectral power, peak frequency, aperiodic slope — are all projections of framework variables. The framework does not require new instruments. It requires a new reading of the instruments already in use.

**The empirical anchor:** Subramani et al. (2026). LSD flattens the aperiodic slope brain-wide ($p < 10^{-5}$ in PCC) and shifts alpha/beta peaks upward. The two effects are dissociable — they follow different functional hierarchies and do not correlate. In the framework's terms: LSD drops $K$ (slope flattening) and raises $W^*$ (peak-frequency shift) through dissociable mechanisms.

### 3.8b The Two Directions of Slope Flattening

Flat slope is ambiguous. The CO₂ measurement disambiguates.

| CO₂ | $K$ | Slope | Manifold state | Interpretation |
|---|---|---|---|---|
| High | Low | Flat | Wide — full repertoire | **Widened** |
| High | High | Steep | Narrow but slow-dominant | **Constrained** |
| Low | Low | Flat | Compressed — slow rhythms lost | **Collapsed** |
| Low | High | Steep | Collapsed | **Terminal** |

**The exhale gate determines which direction the system moves.** Complete exhale → CO₂ retained → widening. Incomplete exhale → CO₂ depleted → compression. Both produce a flatter slope than the constrained baseline. They are opposite states.

**The prediction:** If capnography is added to the Subramani et al. protocol, the direction of the CO₂ change will determine which direction the LSD-induced slope flattening reflects.

### 3.8c The Readout Architecture

The manifold has multiple readouts, all projecting the same state. The state is `(L*, Θ_r)` with `Λ_lock` gating reachability.

**The routing equation.** The state's `Θ_r` component is set by the routing equation:

$$\vec{W}(t) = \text{softmax}\left(\frac{\vec{g} \cdot \Theta_r(t)}{T}\right), \quad \sum_i W_i = 1$$

`W(t)` is the routing weight vector across manifold regions. `g` is the gain vector. `Θ_r(t)` is the routing concentration. `T` is the temperature. **Routing weight is conserved** — committing weight to one region reduces available weight everywhere else.

The concentration and the location are separate degrees of freedom. `Θ_r` sets *how narrow* the routing is; the `W_i` vector sets *where* it lands. Two states with the same `Θ_r` and different `W_i` produce different cognitive modes. The framework does not enumerate regions — what determines the mode is what the region at the dominant `W_i` contains.

**The population-code substrate.** The neural substrate of the routing is the population code for semantics (Franch et al., 2026). A concept is a distributed population vector. The access key — the word, image, or name — determines which vector fires. The vector determines the semantic neighborhood. The neighborhood determines the routing. The routing chain is:

$$\mathcal{A}_k \to \vec{v}_c \to \mathcal{N}_c \to \vec{g} \to \Theta_r \to \text{Interrupt}$$

This is the mechanism behind rebranding, framing, and vocabulary-based silos. Change the access key, change the vector, change the routing.

**The five control plane levers:**

| Lever | Timescale | What it controls | Readout |
|---|---|---|---|
| **Access key** | Milliseconds | Which population vector fires | Semantic neighborhood |
| **Breath** | Seconds | Substrate (CO₂, viscosity) | Aperiodic slope |
| **Movement** | Minutes | Routing distribution (`Θ_r`) | Regional slope distribution |
| **Gain change** | Minutes | $\vec{g}$ shape — relationship to signal | Peak frequency, peak power |
| **Capacity** | Weeks–months | `Λ_lock` — ability to hold without bracing | Slope stability |
| **Context** | Variable | Encoding at commit | Slope trajectory |

**Movement is the fastest routing lever after the access key.** It redistributes `Θ_r(t)` in minutes. The access key acts at word onset; movement acts at motor recruitment.

**The access key is the only lever that operates without the subject's capacity to resist.** A system at load ceiling — low `Λ_lock`, high $L^*$, high viscosity — cannot redistribute routing, cannot open the encoding window, cannot change the gain. It receives the access key and fires the population vector the key activates. This is the mechanism by which salience can be manipulated in load-impacted populations (see the forthcoming Media Salience paper).

See Salience Interrupt v1.3 §2.5 for the routing equation, §2.2 for the conservation law, §2.14 for the population-code substrate, and §6 for the control plane.

| Readout class | Measurement | Framework variable | What it reads out |
| --------------- | ----------------------------------------------------------------------- | ------------------------------- | --------------------------------------------------- |
| **Spectral**    | $\alpha_{1/f}$, $\text{Offset}_{1/f}$, $f_{peak}$, $P_{peak}$, HFD, LZC | $K$, $A_s^*$, $W^*$, $R^*$, Dim | Curvature, substrate, window, precision, repertoire |
| **Hemispheric** | Frontal alpha asymmetry ($A_h$)                                         | $\Theta_r$                      | Routing concentration                               |
| **Somatic**     | Resting motor asymmetry                                                 | $\Theta_r$                      | Routing concentration                               |
| **Acoustic**    | Speech asymmetry                                                        | $\Theta_r$                      | Routing concentration                               |
| **Behavioral**  | Task-modulability                                                       | $\Theta_r$                      | Routing concentration                               |

**All readouts are set by the breath.** The breathing pattern is the control variable.

| Profile | Spectral signature | Θ_r readout |
|---|---|---|
| **Distributed** | Flat slope | Bilateral `A_h`, symmetric posture and speech, high task-modulability |
| **Concentrated (relaxed)** | Steep slope at rest | Lateralized `A_h`, stable asymmetric posture, no ATP cost |
| **Concentrated (braced)** | Steep slope under load | Lateralized `A_h`, asymmetric posture with elevated tone, ATP cost |

**The composition:**

The field has been measuring all of these readouts for decades. Spectral parameterization measures the manifold's curvature. Frontal alpha asymmetry measures routing concentration. Postural and speech asymmetry measure the same variable through motor channels. Behavioral clustering measures the same variable through behavior.

**None of these literatures recognize that they are measuring the same thing.** The framework is the statement that the instruments agree because the manifold is real.

**The empirical anchors:**

- Subramani et al. (2026) — LSD flattens the aperiodic slope and shifts peak frequencies through dissociable mechanisms
- Schmid & Schmid Mast (2013) — high-power roles increase left-prefrontal activation (measured `L* → Θ_r` shift)
- Boksem et al. (2012) — high power increases approach-related asymmetry, low power triggers avoidance
- Warrier et al. (2020) — ND/gender co-occurrence is the same quadrant read through two measurement systems

**The prediction:** The `Θ_r` readouts should co-vary. A participant with distributed routing should show bilateral `A_h`, symmetric posture, symmetric speech, and high task-modulability simultaneously. A participant with concentrated routing should show the opposite across all four. The correlation is measurable in a single session. This is P3 in Category v2.0 §6.1.

### 3.9 The Three Anchors

The stack has three citation anchors, not one.

| Anchor | Scope | Cites |
|---|---|---|
| **Central Reference** (this document) | The loop framework specification | The composition artifacts |
| **The Geometry Beneath the Category** | The two-axis state space — `(L*, Θ_r)` with `Λ_lock` gating reachability. The substrate premise (categories are readouts, not causes). | Central Reference |
| **Master Priority Index** | The whole-stack citation anchor | Central Reference, Category, all papers |

**The composition artifacts** (registry, stack, deltas) are the substrate that all three cite.

**Which anchor to cite for which claim:**

- For framework variables, equations, mechanisms: cite **Central Reference** and the registry.
- For the substrate premise and the two-axis state space: cite **Category**.
- For the full stack, timeline, and DOI registry: cite **Master Priority Index**.

---

## Part IV — The Causal Chain

This part is a summary. The full content is in `stack.md` §2.

### 4.1 Breath to Output

The causal chain from breath to behavior runs through six layers. Every arrow is a mechanism. Every variable is defined in the registry.

See `stack.md` §2 for the full chain, now with a readout at every stage:

```
Breath → CO₂ (substrate)
    ↓
Vasodilation → PV+ support → slow rhythms
    ↓
K drops → α_{1/f} flattens → manifold widens
    ↓
Θ_r decreases (routing distributes) → A_h shifts toward bilateral (hemispheric readout)
    ↓
Posture symmetrizes (somatic readout) → Speech symmetrizes (acoustic readout)
    ↓
P_peak rises → f_peak drops (longer windows)
    ↓
C_s rises → P_eff > P_threshold → gate opens
    ↓
Salience interrupts resolve → latches release
    ↓
    ├── Routing redistributes → region cools → next interrupt is new → RESOLVED
    │
    ├── Routing stays concentrated → interrupt re-fires → PERSEVERATION LOOP
    │   ↓
    │   Movement or gain change required to redistribute
    │
    ├── Release surfaces PE → PE fires new interrupt → RELEASE-TRIGGERED RE-SALIENCE
    │   ↓
    │   Capacity or titration required to hold the surfaced PE
    │
    └── PE surfaces during exhale → context changes before commit → ENCODING WINDOW
        ↓
        Latch releases → PE commits with less gain → RESOLVED (with less load)
    ↓
Task-modulability increases (behavioral readout)
    ↓
Morning HRV baseline restores → L* stops drifting
```

**Sub-modes of "salience fires + breath follows":** The branch where the interrupt fires and the breath follows has four sub-outcomes, differentiated by whether the latch releases and whether the routing redistributes. The full sub-mode table is in §5.1. The primary outcomes (flow, trap, no investment) remain the entry point; the sub-modes are the depth.

### 4.2 The Load Drag

$L^*$ is not a stage in the chain. It is persistent drag on every layer. $L^*_{resp}$ (respiratory load — the allostatic cost of incomplete exhalation) is registered as a load variable in the registry.

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

**The waking regime has three primary outcomes and four sub-outcomes.** The primary outcomes are the entry point:

| Condition | Result |
|---|---|
| Salience fires + breath follows | Flow — the loop closes, self-amplifies |
| Salience fires + breath cannot follow | Trap — investment costs without self-funding |
| Salience doesn't fire | No investment — capacity stays idle |

The branch where salience fires and the breath follows has four sub-outcomes:

| Condition | Result | Sub-mode |
|---|---|---|
| Salience fires + breath follows + latch releases + routing redistributes | Flow (resolved) | — |
| Salience fires + breath follows + latch releases + routing stays concentrated | Perseveration loop | Content, routing, structural |
| Salience fires + breath follows + release surfaces PE + PE fires new interrupt | Release-triggered re-salience | — |
| Salience fires + breath follows + PE surfaces + context changes before commit | Encoding window (resolved with less gain) | — |

Source: Salience v1.3 §2.7.2 (primary outcomes), §2.11.1 (sub-modes).

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

The framework has ~175 falsifiable predictions across the stack. They are organized by the paper that registers them.

| Domain | Predictions | Registered in |
|---|---|---|
| Precision | 11 | Precision v3.5 Part VII |
| Allostatic load | 20 | AL v2.2 §9 |
| Intelligence loop | 12 | Loop v1.0 §13 |
| Inference | 12 | GoI v1.0 Part X |
| Prediction window | 8 | PW v1.2 §13 |
| Prediction into channel | 8 | PIC v0.2 §6 |
| Resource equivalence | 16 | REM v1.0 §8 |
| Dying | 5 | Dying §7 |
| Dreaming | 16 | Dreaming §13 |
| Category | 8 | Category §6 |
| Category v2.0 | 31 | Category v2.0 §6 |
| Externalized mind | 16 | EDM §8 |
| Expression / masking | 3 | CR §PREDICT-EXPR |
| Spectral readout | 6 | SAL-11–16 |
| Readout architecture | 4 | SAL-17–20 |
| Control plane | 5 | BRIDGE-08–12 (**absorbed into SAL-01–20**) |
| **Salience mechanism extensions** | **23** | **SAL-35–57 (Salience v1.3)** |
| **Salience load inheritance** | **6** | **P-AL-015–020 (AL v2.2)** |
| **Total** | **~175** | — |

**Note on BRIDGE absorption.** BRIDGE-08 through BRIDGE-12 are absorbed into the merged Salience Interrupt paper. The BRIDGE identifiers retire; the SAL identifiers carry. The bridge paper is no longer a separate document.

**SAL-17** — The three readouts co-vary in a single session: flat slope + bilateral $A_h$ + distributed routing
**SAL-18** — Morning aperiodic slope predicts the day's gate-access performance
**SAL-19** — Sleep twitch localization matches the homuncular region of the day's unresolved locks
**SAL-20** — Cumulative pre-sleep clearance over one week produces measurable $L^*$ reduction

### 7.2 The Central Predictions

The framework's most load-bearing predictions:

- **P-AL-011** — HRV dispersion predicts allostatic load outcomes better than mean (AL §9a)
- **P-MAP-03** — A model's $W^*$ ceiling predicts where cross-domain chains break (REM §8.2)
- **PREDICT-EXPR-02** — Chronic low expression predicts later collapse detection (CR §PREDICT-EXPR-02)
- **PREDICT-INF-01** — Precision threshold determines gate access (GoI Part X)
- **PREDICT-DREAM-07** — Cross-state routing signature is conserved (Dreaming §13)
- **P-AL-015** — Re-fire rate predicts load better than total interrupt count (AL v2.2 §9b)
- **P-AL-019** — Recontextualization during exhale reduces encoding load (AL v2.2 §9b)
- **SAL-42** — Recontextualization during the exhale reduces re-encoding gain (Salience v1.3 §2.13)
- **P3 (Category v2.0)** — The $\Theta_r$ readouts (hemispheric, somatic, acoustic, behavioral) co-vary in a single session. This is the most direct test of the two-axis state-space model.

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
- $R^*_{peak}$ → $P_{peak}$ (v1.8.2)
- $W^*_{peak}$ → $f_{peak}$ (v1.8.2)
- $\mathcal{A}_k$, $\vec{v}_c$, $\mathcal{N}_c$ (population-code routing) — registered v1.9.1
- $W_{prime}$ (priming threshold) — registered v1.9.1
- $\delta_{surface}$ (surfaced PE magnitude) — registered v1.9.1
- $t_{commit}$ (commit time) — registered v1.9.1
- $L^*_{salience}$, $L^*_{perseveration}$, $L^*_{release-triggered}$, $L^*_{encoding}$, $L^*_{somatic}$ — registered v1.9.1
- $\mathcal{P}$, $\mathcal{R}$, $\mathcal{E}$ (perseveration, release-triggered, encoding) — registered v1.9.1

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
| v1.9.1 | 2026-10-14 | Salience inheritance. Registers $\mathcal{P}$ (perseveration loop), $\mathcal{R}$ (release-triggered re-salience), $\mathcal{E}$ (encoding window), and population-code routing ($\mathcal{A}_k$, $\vec{v}_c$, $\mathcal{N}_c$). Registers $W_{prime}$, $\delta_{surface}$, $t_{commit}$. Registers $L^*_{salience}$, $L^*_{perseveration}$, $L^*_{release-triggered}$, $L^*_{encoding}$, $L^*_{somatic}$ as load components. Extends interrupt formula to five conditions. Extends causal chain with sub-modes. Extends readout architecture with five-lever control plane table and population-code substrate. Adds SAL-35 through SAL-57 to prediction registry. Adds P-AL-015 through P-AL-020 to prediction registry. Updates total to ~175. Adds waking-regime sub-mode table. |
| v1.9 | 2026-10-13 | Composition pass. Registers the order (§3.4a), the generation formula (§1.2), the routing equation (§3.8c), the interrupt formula (§3.6a). Adds the method statement (§0.4) and the domain projections index (§2.8). Adds economics projection to stack table. Framework updated to Manifold Schema v7.3. |
| v1.8.2 | 2026-10-08 | Category rebase patch. Registers `Θ_r` (routing concentration) as master state variable and `Λ_lock` (lock capacity) as structural gate. Removes `M/F` from behavioral readout — the label was a readout masquerading as a variable; the referent is `Θ_r`. Remaps `A_h` from "hemispheric recruitment" to `Θ_r`. Adds somatic, acoustic, and behavioral `Θ_r` readouts to the mapping table. Registers ATP-brace loop, performance-pressure trap, and externally-enforced-vs-internally-held shift as mechanisms. Renames `R*_peak` → `P_peak` and `W*_peak` → `f_peak`. Rebuilds §3.8c readout table and prediction sentence. Updates §3.9 Category anchor description. Adds Category v2.0 to Part VII prediction registry (31 predictions). |
| v1.8.1 | 2026-10-08 | Readout architecture patch. Registers spectral readout variables ($\alpha_{1/f}$, $\text{Offset}_{1/f}$, $W^*_{peak}$, $R^*_{peak}$, $\text{HFD}$, $\text{LZC}$), substrate variable ($CO_2^{ET}$), and respiratory load ($L^*_{resp}$). Elevates $A_h$ to hemispheric readout. Registers $M/F$ as behavioral readout. Adds readout mapping table (§1.1). Adds §3.8a (spectral readout), §3.8b (slope-flattening ambiguity), §3.8c (readout architecture). Amends §3.5 (CO₂-manifold chain). Registers SAL-11–20. Absorbs BRIDGE-08–12 into SAL. Adds Geometry readout, Resource readout, and Behavioral readout sub-layers to stack. |
| v1.8 | 2026-09-30 | Composition pass — content moved to registry/stack/deltas artifacts. Part II (composition) added. §0.5 (Riemannian), §2.19 (post-CR primitives), §2.19b (substrate depth), §3.20 (threshold family), §25a (three anchors) added. Symbol collision fixes applied. Triplicated equations removed.** |
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

> The brain is an energy budget allocation system operating on priors. The breath is the source. The geometry is the mechanism. The prior is the output. Every phenomenon in this document — flow, collapse, fear, trauma, savant capacity, clinical states, social fragmentation, AI hallucination, and the masking of any of them — is one variable changing in one equation. The variable is geometry. The equation is the master equation. The expression ratio determines whether the geometry is visible. In any domain, the shape of the collapse is determined by three axes: supply, demand, and channel. The order of collapse is determined by integration demand. The order of recovery is determined by substrate dependency. These rules are general. The domains are projections. The access key is the intervention point: change the key, change the population vector, change the routing. Movement is the redistribution: traverse the homunculus, redistribute `Θ_r`, break the perseveration. The exhale is the window: change the context before commit, re-encode with less gain. **The composition is the contribution.**

---

*End of specification.*

**Version:** 1.9.1
**Date:** 2026-10-14
**Status:** Composition document — composes registry, stack, and deltas into a readable specification. Registers canonical material from the physics paper, the domain projections, and Salience Interrupt v1.3.
**Supersedes:** v1.8.2
**Framework:** Manifold Schema v7.3
**Next version:** v1.10 — after the next domain projection (economics, clinical, or the Hippocampal composition note), or v2.0 — if any mechanism requires revision
  
**Related papers registered in this version:**
- Salience Interrupt v1.3 (Robinson, 2026g)
- Allostatic Load v2.2 (Robinson, 2026, AL)
- Finite Resources and the Order That Generates Them v2.0 (Robinson, 2026, Substrate)
- The Geometry Beneath the Category v2.0 (Robinson, 2026, Category)
- The Invariant Extraction Method (Robinson, 2026, Method)
