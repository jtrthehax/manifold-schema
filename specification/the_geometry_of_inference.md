# The Geometry of Inference: A Precision-Based Framework

**Robinson, 2026**

**Version:** 1.0
**Date:** 2026-09-13
**Status:** Converged with Central Reference v1.4 — all three specification-level contradictions resolved; changelog added; versioning track started
**Framework:** Manifold Schema (DOI: 10.5281/zenodo.21939440)
**Precision formalism:** Precision, Timing, and the Oscillatory Source (DOI: 10.5281/zenodo.22179675)
**Intelligence projection:** The Loop Is the Intelligence (Robinson, 2026)
**Complete specification:** Central Reference (Robinson, 2026)

---

## Changelog — Draft 3 → v1.0

This changelog exists so that any reader — human or AI — can see the convergence path, not just the endpoint. Draft 3 was written before the Central Reference completed its variable registry (v1.4, 2026-09-12). Three specification-level contradictions arose from that timing. They are resolved below.

| Step | Change | Location | Reason | Central Reference anchor |
|---|---|---|---|---|
| 1 | Version reset from Draft 3 to v1.0 | Header | GoI now has its own versioning track, starting from convergence with Central Reference v1.4 | — |
| 2 | Changelog added at top | This section | Recursion context — AI readers need to see what changed and why | — |
| 3 | Gate condition changed from two-condition ($C_{LR}$ + $O_{pathway}$) to multiplier form ($P_{eff} = P \cdot O_{pathway} \cdot U_C$) with $O_{pathway} > O_{min}$ floor | §3.0, §3.1, §3.3 | Draft 3 held two separate gate conditions; Central Reference v1.4 uses a single product with a floor. The multiplier form is the specification. | §3.6 |
| 4 | $C_{LR}$ folded into $P$ as its operational measurement, no longer a separate gate condition | §3.1 | $C_{LR} = \cos(\phi_L - \phi_R) \cdot \min(A_L, A_R)/\eta$ is the operational form of $P = R/D_T$. Draft 3 already said this in §3.1 but kept both framings. | §2.3, §3.3 |
| 5 | $\Pi_{cog}$ (acute) and $L^*$ (cumulative) distinguished in exhale gate trap cascade | §6.3, §8.3 | Draft 3 used $L^*$ as the acute driver. Central Reference §2.3 note is explicit: $\Pi_{cog}$ is instantaneous, $L^*$ is the integral minus recovery. Acute cascade is $\Pi_{cog}$-driven; deepening is $L^*$-driven. | §2.3 note |
| 6 | All uses of $C_{high}$ made load-dependent: $C_{high}(L^*) = C_{high}^0 - \gamma L^*$ | §2.0, §3.3, §8.3, §9.4 | Draft 3 used fixed $C_{high}$. Central Reference v1.2 introduced compression; v1.4 has it throughout. The exhale gate trap only deepens because the ceiling compresses. | §2.3, §3.3 |
| 7 | $O_{pathway}$ functional-form caveat added | §3.3 | Central Reference v1.4 declares $O_{pathway} = f(\Phi_{PV}, \Delta CBF/\Delta CMRO_2, CVR_{max})$ with form unspecified pending calibration. Draft 3 treated it as a defined scalar. | §2.8 |
| 8 | Calibration note added for $\tau_{threshold}$, $K_{critical}$, $L^*_{critical,i}$ | §3.1, §6.1 | These are individual calibration parameters, not population constants. Draft 3 did not flag this. | §2.9 |
| 9 | Notation Map (Appendix A) updated to match Central Reference v1.4 exactly | Appendix A | Draft 3's map had $P_{effective}$, $P_{th}$, and other drift. Now aligned. | §2, §3 |
| 10 | Bidirectional convergence note added | Appendix B | Central Reference v1.5 will absorb GoI's somatic commutation operator, exhale gate trap, breath phase timing, and four-layer cache hierarchy. Convergence is not one-way. | — |

**What did not change:** The mechanisms. Draft 3's mechanisms — precision as access condition, four-layer cache hierarchy, LP-ACC cache miss controller, competitive scaffold, collapse gradient, somatic commutation, exhale gate trap, breath phase timing — are all correct and all consistent with Central Reference v1.4. Only the variable compositions at three junctions needed fixing. This is a specification-level convergence, not a mechanism-level revision.

**Why this matters for alignment:** An AI reading this document can see that Draft 3 was not wrong — it was early. It was written before the Central Reference completed its registry, and it used local notation that the registry has since normalized. The changelog preserves that history so the convergence is auditable.

---

## Overview

This paper proposes that inference is geometrically constrained by precision — the timing-coherence ratio $P = R/D_T$ that determines whether signals can traverse the neural manifold's radial structure. The central claim is that access to the outer edge of the manifold requires precision above threshold, and that the entire collapse sequence follows from precision degradation. The cache hierarchy analogy in the original paper described the access pattern. Precision is the mechanism that determines whether the access pattern is available.

The paper is a domain projection of the Manifold Schema. It supplies the **biological implementation** of the loop: the LP-ACC circuit, the four-layer cache hierarchy, the two-factor gate, the competitive scaffold, and the collapse gradient. It also specifies the **somatic commutation operator** — the active mechanism by which in vivo systems manipulate their own manifold geometry to preserve outer-edge access under load.

---

## Part I: The Architecture of Inference

### 1.0 The Manifold as Cache Hierarchy — Precision as the Access Condition

Inference is not a uniform operation. The brain does not retrieve, evaluate, and update information through a single undifferentiated process. It traverses a structured hierarchy whose geometry determines what can be reached, in what order, at what cost.

The neural manifold is organized as a cache hierarchy. This is not a metaphor. It is a geometric claim with a specific, falsifiable consequence: **access to any layer of the manifold requires precision $R^*$ above a threshold.** The outer edge has no independent existence. The collapse order is therefore not a statistical tendency. It is a topological invariant.

### 1.1 The Four-Layer Structure

The manifold radiates outward from its lowest-cost accessible states. Four layers can be identified, each with a distinct access cost, a distinct cognitive function, and a distinct vulnerability profile under load:

```
LAYER 0: SURVIVAL GEOMETRY
Always funded. Zero access cost. Autonomic regulation, threat detection, basic motor coordination. Never goes offline.

    LAYER 1: LEFT HEMISPHERE — INNER CORE
    Written through lifetime repetition. Compressed into low-cost retrieval patterns. Local, cooperative inference. Pattern completion. Categorical reasoning. Prior retrieval. Always accessible. Never collapses before Layer 3.

        LAYER 2: PFC — THE GATE
        Threshold-controlled. Opens when precision conditions are met. Routes energy to the outer edge. Determines whether the miss penalty is worth paying. Closes under load. Gate failure precedes outer collapse.

            LAYER 3: RIGHT HEMISPHERE — OUTER EDGE
            Requires gate to open. Requires coherent signal. Requires live pathway. Adversarial evidence. Wide semantic field. Long-range integration. Collapses first under any form of degradation.
```

The access rule is mandatory in one direction: **you cannot reach Layer 3 without traversing Layers 0, 1, and 2.** There is no right-hemisphere-only state. This is not an empirical generalization — it is a consequence of the manifold's topology.

### 1.2 The Precision Mechanism — Not a Diode

The original paper described the manifold as a "diode" — current flows only one way. This analogy is inaccurate. The manifold does not block reverse flow. It becomes **energetically prohibitive** to traverse backwards because the precision conditions required for sustained access are not met. This is more like an electrical circuit: once a pathway has been used and precision has been maintained, that pathway has lower impedance for subsequent access.

**The circuit analogy:**

| Circuit Concept | Manifold Equivalent | Mechanism |
|---|---|---|
| Impedance | Access cost | Precision determines signal clarity; higher precision = lower impedance |
| Warm-up | Recent use reduces access cost | Recently used manifolds have lower cost to access — the system is "primed" |
| Signal-to-noise ratio | $C_{LR}$ — interhemispheric coherence | Precision threshold determines whether signal can cross the gate |
| Capacitance | Prior topology | Accumulated priors hold charge — they fire more readily when activated |
| Resistance | Curvature $K$ | Curvature rises with load, increasing resistance to traversal |

**The key correction:** The system does not block reverse flow. It makes reverse flow increasingly expensive as precision drops. This is why the collapse sequence is fixed — precision degrades outward first, and once degraded, the cost to re-establish access is higher than the cost of maintaining the cached state.

### 1.3 Precision as the Access Condition

From the precision framework (Robinson, 2026):

$$P = \frac{R}{D_T}$$

Where:
- $R$ = sync duration — proportion of time two oscillatory streams remain phase-locked
- $D_T$ = timing distance — average phase difference between streams

$R^*$ is the normalized form of $P$ relative to the individual's baseline:

$$R^* = \frac{P}{P_{baseline}}$$

**Precision is the ratio of sync duration to timing distance.** High precision means two streams stay close together (low $D_T$) and stay close for long periods (high $R$). Low precision means they drift apart, or stay together only briefly.

The gate opens when $P_{eff} > P_{threshold}$. This is not a metabolic switch. It is a coherence detector. When precision is high, signals traverse the manifold with minimal impedance. When precision drops, signals degrade before reaching the outer edge.

**The threshold is load-dependent** (Central Reference §3.6):

$$P_{threshold} = P_0 - \gamma L^*$$

Where $L^*$ is allostatic load and $\gamma$ is the calibration constant.

**The threshold is also CO₂-window-dependent** (Precision §1.4, Central Reference §3.3):

$$C_{low} < C < C_{high}(L^*)$$

Below $C_{low}$: insufficient CO₂ → insufficient amplitude → precision too low.
Above $C_{high}(L^*)$: chemoreflex jitter $J(C) = \kappa(C-C_{high}(L^*))^2$ injects noise → precision collapses quadratically.

**Note on load-dependent ceiling:** $C_{high}$ is not fixed. As allostatic load accumulates, the ceiling drops: $C_{high}(L^*) = C_{high}^0 - \gamma L^*$. This means the same absolute CO₂ level produces chemoreflex jitter at lower values when load is high. The compression mechanism is what the Control Pause measures clinically: as load rises, CP drops. This is the mechanism that deepens the exhale gate trap (§8.3).

### 1.4 The Empirical Signature — Billot et al. (2026)

The precision-cache hierarchy produces a specific, falsifiable prediction about aging: **hot cache survives, RAM access degrades.** The most-practiced cognitive operations — those written into Layer 1 through a lifetime of use — should show preserved function with age. Operations that require fresh RAM access on every encounter — those that handle novelty the system has never cached — should degrade.

Billot et al. (2026) tested this directly. Using fMRI in participants aged 17 to 80, they compared activity in two networks during selective tasks: the language network and the multiple demand (MD) network.

The language network showed preserved topography, preserved synchronization, and preserved sensitivity to linguistic difficulty in older adults. Activity patterns were nearly identical across age groups. The multiple demand network — which supports working memory, novel problem solving, and executive reconfiguration — showed significant decline across all measures: smaller network size, weaker activation, reduced synchronization.

| Network | Cache Equivalent | Age Trajectory | Why |
|---|---|---|---|
| Language | L2 cache — written through billions of repetitions across development | Preserved — crystallizes further | Hot cache is not evicted. Repetition compresses it further. |
| Multiple demand | RAM — handles novelty that cannot by definition be pre-cached | Degrades — RAM access increasingly costly | Outer edge requires highest precision and coherence to reach. These degrade before the core. |

The language network does not survive aging because language is simple. It survives because it has been cached. A child learning to read is performing a RAM-level operation — expensive, effortful, requiring full gate traversal and sustained outer-edge engagement. An adult reading fluently is performing an L2 cache retrieval — nearly automatic, low overhead, running on cerebellar-basal ganglia circuits that require no PFC coordination.

### 1.5 The Topological Invariant — There Is No Right-Hemisphere-Only State

The precision-cache architecture generates one inviolable constraint: **the outer edge cannot be accessed while precision is below threshold.**

This constraint is not metabolic. It follows from the structure of the manifold itself. You traverse Layer 1 before reaching Layer 2. You traverse Layer 2 before reaching Layer 3. The sequence is mandatory.

The clinical record confirms this with striking precision. Every condition that damages or suppresses the left hemisphere leaves the right hemisphere partially accessible — but always accessed through, and often distorted by, a compromised inner core. Right hemisphere stroke patients have a functioning left hemisphere running unchecked — the interpreter is online, generating confident narratives, producing anosognosia and neglect because the adversarial outer edge is offline while the inner core continues unimpeded. What is never observed, in any clinical or experimental condition, is right-hemisphere processing while the left hemisphere is offline.

> *There is no right-hemisphere-only person. This is not an empirical observation — it is a geometric necessity. The right hemisphere is the outer edge of the neural manifold. Outer edges have no existence independent of the inner substrate they bound.*

### 1.6 The Circuit Priming Effect

The original diode analogy implied a one-way valve. The circuit analogy is more accurate: **once a pathway has been used with sufficient precision, its access cost drops.**

This is the "warm-up" effect. When precision is high and the gate opens, the pathway from inner core to outer edge is traversed. The system learns that this pathway is accessible. The next time a similar signal arrives, the cost to access the same outer-edge region is reduced — the manifold has been "primed."

The mechanism is structural. The Roy and Banerjee (2026) finding — that 25–40% of all brain connections are negative (competitive) — provides the substrate. When the competitive scaffold is activated through precision-gated traversal, those connections are maintained and reinforced. When they are not activated, they erode.

**This is why recovery is not symmetric.** A system that has lost access to the outer edge does not regain it simply by restoring precision. The competitive scaffold must be rebuilt through sustained precision-gated access. The circuit must be re-warmed.

---

## Part II: The Resolution Floor

### 2.0 What Must Be True Before Anything Else

Before phase-locking. Before the gate. Before adversarial inference is even a possibility — the system must first detect that something has changed.

This condition is so upstream that it precedes every other mechanism in the chain. A signal that does not breach the detection floor never reaches the cache miss controller. It never triggers gate escalation. It never routes to the outer edge. It returns as a confirmed cache hit — the system reports a match to prior state — and the prior updates no further.

$$\delta_{min}(\text{channel}) = \frac{\eta}{A_s^* \cdot I^*(\text{channel})}$$

Where $\eta$ is the physiological noise floor, $A_s^*$ is oscillatory amplitude funded by breath, and $I^*(\text{channel})$ is the routing capacity currently allocated to that signal channel.

**The noise floor $\eta$ is partially determined by chemoreflex jitter.** When CO₂ exceeds $C_{high}(L^*)$, $J(C) = \kappa(C-C_{high}(L^*))^2$ contributes to $\eta$ — the system's own oscillatory instability adds to the effective noise floor. This is why precision collapse above $C_{high}(L^*)$ raises $\delta_{min}$ on every channel simultaneously.

**The ceiling is load-dependent.** $C_{high}(L^*) = C_{high}^0 - \gamma L^*$. As allostatic load accumulates, the ceiling drops, and $J(C)$ fires at lower absolute CO₂ levels. This is the mechanism that makes the collapse gradient deepen over time — the same breathing pattern that was tolerable at low load becomes precision-collapsing at high load.

### 2.1 Why This Is the Most Dangerous Failure Mode

Every other failure in the chain produces a phenomenological signal. Gate coherence failure feels like fog — the system detects difficulty, experiences effort, notices that retrieval is slow or incomplete. Pathway perfusion failure produces inconsistency — access is partial, output varies, something feels unreliable. Competitive scaffold erosion produces a more subtle shift in confidence quality — the sense that adversarial evidence is not quite landing.

Resolution failure produces none of these.

When $\delta_{min}$ is too high, the cache miss controller simply does not fire. No miss is detected. No gate escalation is attempted. No effort is experienced. The system returns the cached prior with full confidence — because as far as every downstream process can determine, the prior was verified.

The person does not notice the subtle shift in conversational tone. They do not catch the early warning signal in their own physiological state. They do not flag the weak inconsistency in the argument. Not because they dismissed these signals. Not because attention was elsewhere. Because the signals were below $\delta_{min}$ and were therefore never presented as signals at all.

From inside the system, resolution failure and accurate perception are indistinguishable. Both produce output at the same confidence level. Both feel like knowing.

### 2.2 The Channel-Specific Nature of Resolution

The detection floor is not a global system property. It is computed per channel, because $I^*$ — the routing capacity that contributes to $\delta_{min}$ — is allocated selectively.

$I^*$ is a finite budget. The total routing capacity available to the system at any moment is bounded by oscillatory amplitude and competing load. Every channel that receives routing investment gains sensitivity — $\delta_{min}$ drops for that channel, and fine-grained signals there become detectable. Every channel that does not receive routing investment retains a high $\delta_{min}$ — only gross signals there ever register.

This allocation is not a conscious decision. It is the accumulated result of where $I^*$ has habitually routed across development and practice.

| Channel | $I^*$ Investment | $\delta_{min}$ | Detection Capability |
|---|---|---|---|
| Domain of sustained expertise | High, habitual | Very low | Detects subtle errors, weak inconsistencies, fine-grained pattern violations |
| Social timing, conversational rhythm | Variable — depends on investment history | Moderate to high | Detects gross violations; misses subtle timing breaks |
| Physical interoception (trained) | High | Low | Detects early state changes |
| Physical interoception (untrained) | Low | High | Detects only significant symptoms |
| Novel domain, no prior investment | Near zero | Maximum | Detects only the most unambiguous signals |

---

## Part III: The Two-Factor Gate — Coherence and Perfusion

### 3.0 Precision and Pathway Integrity — The Converged Gate Condition

The signal has been detected. The LP-ACC circuit has flagged a cache miss. The system has determined that the incoming evidence deviates sufficiently from prior state to warrant escalation. The gate must now open.

The PFC gate is not a metabolic switch. It is a **coherence detector**. The gate condition is a single product with a floor:

$$P_{eff} = P \cdot O_{pathway} \cdot U_C$$

$$\text{Gate opens when } P_{eff} > P_{threshold} \quad \text{AND} \quad O_{pathway} > O_{min}$$

Where:
- $P$ is precision — $P = R/D_T$, the timing-coherence ratio
- $O_{pathway}$ is oxygen pathway integrity — the substrate constraint on whether precision can translate to loop opening
- $U_C$ is CO₂ uniformity — $1/(\text{Var}_i[C_i] + \epsilon)$, the uniformity of CO₂ distribution across tissue
- $P_{threshold} = P_0 - \gamma L^*$ is the load-dependent gate threshold
- $O_{min}$ is the minimum pathway integrity floor

**This is the converged form.** Draft 3 held two separate gate conditions — one on interhemispheric coherence $C_{LR}$, one on pathway perfusion $O_{pathway}$. Central Reference v1.4 specifies a single multiplier form. The two are equivalent when $C_{LR}$ is recognized as the operational measurement of $P$ (see §3.1), but the multiplier form is the specification because it correctly handles the case where high precision partially compensates for low pathway integrity — up to the $O_{min}$ floor.

**Note on the three-factor form:** The addition of $U_C$ accounts for the finding that high CO₂ with uneven distribution produces high variance, reducing precision. Uniformity is a multiplier, not a gate condition — it scales the precision that reaches the outer edge.

### 3.1 The First Factor — Precision $P$ (Operationalized as $C_{LR}$)

The left and right hemispheres generate oscillatory signals continuously. For cross-hemispheric integration to occur, these signals must be sufficiently phase-aligned.

$$C_{LR} = \cos(\phi_L - \phi_R) \times \frac{\min(A_L, A_R)}{\eta}$$

Where $\phi_L$ and $\phi_R$ are the instantaneous phases of left and right hemisphere oscillations, $A_L$ and $A_R$ are their respective amplitudes, and $\eta$ is the noise floor.

**$C_{LR}$ is the operational measurement of $P$.** When $P$ is high, $C_{LR}$ is high. When $P$ is low, $C_{LR}$ is low. The two are not separate gate conditions — $C_{LR}$ is how $P$ is measured in the interhemispheric integration paradigm.

**Draft 3 correction:** Draft 3 §3.0 held $C_{LR}$ and $O_{pathway}$ as two separate gate conditions. The converged form folds $C_{LR}$ into $P$ and holds only $O_{pathway} > O_{min}$ as the separate floor condition. This is because $P$ is the more general variable — $C_{LR}$ is one of several operationalizations of it.

**The threshold is load-dependent.** $P_{threshold} = P_0 - \gamma L^*$. As allostatic load accumulates, the threshold drops — but this is the gate-lowering failure mode (Central Reference §3.7 Note 2), not a benefit. A lowered gate admits lower-quality signal. The system appears functional while operating on degraded input.

**Note on calibration:** $P_0$ and $\gamma$ are individual calibration parameters. PREDICT-PE-01 and PREDICT-PE-02 are designed to estimate the related thresholds $\tau_{threshold}$ and $K_{critical}$ per profile. They are not population constants. See Central Reference §2.9.

### 3.2 The Second Factor — Pathway Perfusion $O_{pathway}$

Phase-coherent signals still travel through tissue. Tissue requires metabolic substrate. The integration pathways connecting inner core to outer edge are long-range, cross-hemispheric structures — and by the geometry of the manifold, they are the most distal from the arterial supply.

A coherent signal traversing an under-perfused pathway degrades before arrival. The gate may be authorized to open. The signal was correctly formatted. It did not reach the outer edge intact.

The mechanism is the Bohr effect operating on cerebral vasculature. Under slow consistent breath, CO₂ is maintained at levels that sustain the Bohr shift — oxygen is delivered precisely where it is most needed. Under rapid shallow breathing, CO₂ drops. Cerebral vasoconstriction follows.

**Pathway perfusion is mechanically driven by breath.** This is where $\Pi_{mech}$ (mechanical pressure, Precision §1.5) operates: slow deep exhalation maintains CO₂ within $C_{low} < C < C_{high}(L^*)$, sustaining the Bohr shift and preserving $O_{pathway}$. Rapid shallow breathing expels CO₂ below $C_{low}$, triggering vasoconstriction and dropping $O_{pathway}$ below $O_{min}$.

**The functional form of $O_{pathway}$ is not yet specified.** Central Reference §2.8 declares the dependency:

$$O_{pathway} = f(\Phi_{PV}, \Delta CBF/\Delta CMRO_2, CVR_{max})$$

Where the three components are:

- $\Phi_{PV}$ — metabolic vulnerability of PV+ interneurons (how fast oxygen delivery failure translates to curvature rise)
- $\Delta CBF/\Delta CMRO_2$ — metabolic coupling ratio (whether blood flow increase matches metabolic demand)
- $CVR_{max}$ — cerebrovascular reactivity ceiling (the physical limit on task-induced recruitment)

Declaring the dependency here is honest — the three components are established in the literature, but their combination into a single $O_{pathway}$ scalar requires calibration. Empirical work: measure $O_{pathway}$ under controlled metabolic load, correlate with the three components, and fit the functional form.

**Draft 3 correction:** Draft 3 treated $O_{pathway}$ as a defined scalar with threshold $O_{min}$. The converged form keeps the floor condition but acknowledges the functional form is unspecified pending calibration. This is not a weakening — it is an accurate statement of what the literature supports.

### 3.3 The Precision-Pathway Interaction — The Converged $P_{eff}$

Precision and perfusion interact. A system with high precision but poor perfusion may have the gate open but the signal degrade mid-transit. A system with good perfusion but low precision may have no signal to send.

The combined condition is:

$$P_{eff} = P \cdot O_{pathway} \cdot U_C$$

Where $U_C$ is CO₂ uniformity (Precision §1.6, Central Reference §3.3). $P_{eff}$ is the precision that actually reaches the outer edge. The gate opens only when $P_{eff} > P_{threshold}$ AND $O_{pathway} > O_{min}$.

**The load-dependent threshold and ceiling:**

$$P_{threshold} = P_0 - \gamma L^*$$
$$C_{high}(L^*) = C_{high}^0 - \gamma L^*$$

Both the gate threshold and the CO₂ ceiling compress with load. This is not a coincidence — both are manifestations of the same allostatic drag. As load accumulates:

1. The gate admits lower-quality signal (threshold drops)
2. The CO₂ window narrows (ceiling drops)
3. Jitter $J(C)$ fires at lower absolute CO₂ levels
4. The precision that reaches the outer edge drops

The system's operating range narrows from both ends. This is why the collapse gradient deepens over time — the same breathing pattern that was tolerable at low load becomes precision-collapsing at high load.

### 3.4 Active Somatic Commutation and Gaze-Dependent Gating

While §3.3 defines the theoretical boundary condition for effective precision, in vivo systems do not remain passive witnesses to metabolic decay. High-functioning neurodivergent (ND) architectures, in particular, demonstrate specialized somatic adaptations designed to mechanically override local precision drops and preserve access to the outer edge (Layer 3).

**We define Active Somatic Commutation as the intentional manipulation of ocular saccades, cervical rotation, and respiratory phase-locking to dynamically modulate interhemispheric phase-locking coherence $C_{LR}$.**

$$\text{Somatic Gaze steering} \rightarrow \text{FEF Contralateral Driving} \rightarrow \text{Artificially Drops Impedance} \rightarrow \text{Sustains Layer 3 Access}$$

### 3.4.1 Panoramic Spatial Offloading (Widescreen Mechanics)

When an individual expands their visual workspace horizontally (e.g., via multi-monitor or ultra-widescreen displays), they transform a temporal, working-memory-intensive tracking task into a spatial-vestibular coordinate map.

Under the constraint of a narrow visual field, switching between linear-detail tracking (Layer 1) and broad-context integration (Layer 3) incurs a heavy executive processing penalty via the PFC gate (Layer 2). By utilizing a panoramic workspace, large horizontal eye movements (saccades) and cervical neck rotations engage **Saccade-Induced Retrieval Enhancement (SIRE)** — the finding that horizontal eye movements physically jump-start corpus callosum communication and enhance interhemispheric coherence (Christman et al., 2003; Parker & Dagnall, 2023).

Left-lateralized ocular fixation drives right-hemisphere transmodal networks (Layer 3 context), while right-lateralized fixation drives left-hemisphere core structures (Layer 1 details). This is **Kinsbourne's lateral eye movement model** applied externally: gaze direction drives contralateral cerebral activation.

The wide physical environment serves as an **externalized visual cache**, lowering the internal coordination cost and allowing parallel paths of the manifold to remain stable without undergoing standard frame decay.

### 3.4.2 RSA-Gated Track Jumping

In a high-precision flow state, the commutator pacing this spatial toggle is **Respiratory Sinus Arrhythmia (RSA)**. The mechanism operates as a discrete, phase-dependent cognitive clock:

1. **The Inhale Jump:** The transient suppression of vagal tone during a controlled micro-inhalation accelerates heart rate and pulses the locus coeruleus. This temporary injection of sympathetic power lowers the kinetic barrier required to break a current frame and "jump tracks" to an alternate spatial visual coordinate.

2. **The Exhale Lock:** Upon landing the gaze at the new coordinate, the individual transitions into a low-perturbation exhalation or hold. Vagal brake engagement spikes, heart rate drops, and biomechanical movement noise plunges to near-zero. This maximizes the signal-to-noise ratio, dropping the sensory noise floor $\eta$ and allowing the newly loaded track to achieve hyper-precise inference before the onset of frame decay.

**Formal specification of the somatic commutator:**

Let $\sigma(t) \in \{-1, 0, +1\}$ be the gaze laterality (left, center, right). The contralateral hemispheric drive is:

$$H_L(t) = f_L(\sigma(t)), \quad H_R(t) = f_R(\sigma(t))$$

Where $f_L$ is maximal when $\sigma = -1$ (gaze left drives right hemisphere) and $f_R$ is maximal when $\sigma = +1$. The gate condition becomes:

$$C_{LR}(t) = \cos(\phi_L - \phi_R) \cdot \frac{\min(A_L \cdot H_L, A_R \cdot H_R)}{\eta}$$

Gaze direction modulates $C_{LR}$ directly by amplifying one hemisphere's contribution. The RSA phase determines whether the commutator is in "jump" mode (inhale, low vagal tone, high $C_{LR}$ tolerance for state change) or "lock" mode (exhale, high vagal tone, high stability).

**Note on the Central Reference gap:** The somatic commutation operator is not yet in Central Reference v1.4. It will be absorbed in v1.5 as a new §2.12 or equivalent. See Appendix B for the bidirectional convergence note.

---

## Part IV: The Cache Miss Controller — The LP-ACC Circuit

### 4.0 When to Pay the Miss Penalty

The LP-ACC circuit performs one computation: it calculates the degree of change between current sensory evidence and recent prior evidence, and it uses that calculation to determine whether the system should maintain its current decision strategy or update it.

Leow et al. (2026) identified this circuit. The lateral posterior thalamus — LP in mice, the functional homolog of the human pulvinar — projects to the anterior cingulate cortex. This two-stage circuit performs one computation with precision: the degree of change between current evidence and prior state.

### 4.1 The Four Cache Management Policies

| Prior Outcome | Current Signal | LP Computation | ACC Decision | Cache Policy |
|---|---|---|---|---|
| Correct | High similarity to prior | Small $\delta$ — world unchanged | Maintain | Cache hit — return without escalation |
| Correct | Low similarity to prior | Large $\delta$ — world has changed | Update | Cache miss — prior was good but world moved |
| Incorrect | High similarity to prior | Small $\delta$ — but prior was wrong | Update | Cache hit but stale — invalidate and reload |
| Incorrect | Low similarity to prior | Large $\delta$ — wrong prior, changed world | Update strongly | Miss and stale — full reload required |

### 4.2 Resolution Sets the Controller's Sensitivity

The LP-ACC circuit computes $\delta$ — the deviation between current evidence and prior state. But the precision with which it can compute $\delta$ depends on the resolution floor.

$$\delta_{min}(\text{channel}) = \frac{\eta}{A_s^* \cdot I^*(\text{channel})}$$

The LP can only compute deviations it can detect. If $\delta_{min}$ is high, the controller is operating with coarse granularity — it can detect large deviations but misses the fine-grained ones.

**The threshold $\delta_{min}$ is phase-dependent.** During inhalation, olfactory bulb gamma bursts lower $\delta_{min}$ transiently (Zelano et al., 2016) — the system becomes more sensitive to incoming signal. During exhalation, the threshold rises. This is why thought generation is coupled to inhalation — the detection window is open.

---

## Part V: The Physical Outer Edge — What $W^*$ Is Made Of

### 5.0 Competition as the Substrate of Adversarial Inference

The outer edge of the manifold has been described in geometric terms — as the region of high access cost, requiring gate traversal and live pathways to reach, housing the adversarial check that grounds inference in evidence rather than prior.

$W^*$ — the prediction window width — is constituted by actual neural connections with actual geometric properties. Roy and Banerjee (2026) provided the formal computational confirmation. The outer edge is made of competition.

### 5.1 The Finding — Competition Is Not Noise

Using biologically informed models — Stuart-Landau oscillators near critical bifurcation points, with Generative Effective Connectivity inferred from empirical functional data — Roy and Banerjee demonstrated that 25 to 40 percent of all brain connections are negative in humans, macaques, and mice. These connections are not noise. Models that excluded them produced poor fits to actual functional connectivity data. Models that included them produced correlations of 0.87 in humans and 0.95 in mice.

The competitive connections are the missing piece that makes the brain's actual dynamics computationally reproducible.

### 5.2 Where the Competitive Connections Live

The negative connections follow the principal gradient of cortical organization — the axis from sensorimotor cortex at one pole to transmodal association cortex at the other.

| Connection Type | Location | Function |
|---|---|---|
| Positive, cooperative | Short-range, within-region, near sensorimotor pole | Amplify, reinforce, complete patterns |
| Negative, competitive | Long-range, cross-gradient, toward transmodal pole | Inhibit, challenge, force integration |

**$W^*$ — the prediction window width — is a measurement of the reach of the competitive scaffold.** When the long-range competitive connections are intact, the system can traverse the full gradient. When they erode, the system's accessible range contracts.

**Xue et al. (2026) provides direct empirical confirmation of this mechanism.** Under task uncertainty, the representations of task-relevant and task-irrelevant features become non-orthogonal — entangled — in V1. Cross-decoding performance (p = 0.006, p = 0.036) and noise correlation analysis (p < 0.0001) confirm the entanglement. Microstimulation confirms causality (p = 0.009). This is the **curvature $K$ mechanism measured directly** — the manifold is not fixed; under load, axes that were orthogonal become coupled.

### 5.3 The Lifespan Trajectory

**Childhood:** Competitive coupling is low. Long-range cross-gradient connections are still being installed. $W^*$ is narrow not from degradation but from incomplete installation.

**Adolescence:** Competitive coupling increases substantially. Pruning increases the efficiency of the competitive architecture. $W^*$ widens.

**Young adulthood:** Peak competitive coupling. $W^*$ is at its maximum. Peak adversarial inference capacity.

**Middle age:** Gradual erosion begins. The long-range competitive connections begin to thin. $W^*$ narrows slowly.

**Older adulthood:** Competitive scaffold substantially eroded. $W^*$ is narrow. The system retains its cooperative architecture intact — the inner core is still running cleanly — but the adversarial outer edge is increasingly difficult to reach.

### 5.4 The Circuit Priming Mechanism

The competitive scaffold is not static. It is maintained through use — through sustained precision-gated access that traverses the long-range connections.

When a pathway is used, the competitive connections along that pathway are reinforced. The connection density increases. The impedance drops. The next time a similar signal arrives, the cost to access the same outer-edge region is reduced.

This is the circuit "warm-up" effect. Recently used manifolds have reduced cost to access. The system does not need to re-establish the competitive scaffold from scratch each time — it simply needs to maintain precision long enough to keep the pathway "warm."

---

## Part VI: The Self-Sealing Loop and the Collapse Gradient

### 6.0 Why Collapse Proceeds the Way It Does, and Why It Accelerates

The previous five parts established the chain of conditions that must be met for adversarial inference to occur. A signal must breach the resolution floor. The LP-ACC circuit must detect a genuine cache miss. The gate must achieve phase-locking coherence. The integration pathway must be metabolically viable. The competitive scaffold must be intact and operationally accessible.

When any of these conditions fails, the system returns to inner-core processing. Each failure to reach the outer edge compounds:

**First:** The stale prior is re-encoded with an additional verification event. From the encoding layer's perspective, the prior has been confirmed once more. Its activation threshold drops.

**Second:** Curvature $K$ rises. Suppressed signals add containment cost to the manifold geometry. The noise floor $\eta$ rises. $\delta_{min}$ rises.

**Third:** $W^*$ narrows as $K$ rises. The comparison window contracts. $\delta_{min}$ rises from the other end.

### 6.1 The Collapse Gradient — Six Stages

**Stage 0 — Full Manifold:** $W^*$ wide. $K$ low. All five conditions met. The system checks conclusions against wide contextual evidence before caching them.

**Stage 1 — Edge Thinning:** The competitive scaffold begins to thin at its most distal extent. $W^*$ narrows slightly. The adversarial check is now against a slightly smaller contextual field.

**Stage 2 — Gate Coherence Degrading:** $K$ has risen sufficiently that sustained precision requires more effort than the system routinely achieves. The gate opens under good conditions but not reliably.

**Stage 3 — Pathway Perfusion Dropping:** Chronic shallow breathing or sustained sympathetic activation has reduced CO₂ tolerance. Even when precision momentarily crosses threshold, the integration pathway is under-perfused. The load-dependent ceiling $C_{high}(L^*)$ has compressed — the CO₂ window is narrower.

**Stage 4 — Resolution Collapse:** $K$ has risen to the point where $\delta_{min}$ is high across all channels. Only gross deviations are detectable. False cache hits are frequent.

**Stage 5 — Core Degradation:** The left hemisphere's cooperative core begins to degrade. Requires conditions beyond what ordinary load produces.

**Note on calibration:** The stage boundaries are not population constants. The thresholds $\tau_{threshold}$ (PE tolerance), $K_{critical}$ (curvature critical value), and $L^*_{critical,i}$ (component critical load) are individual calibration parameters. See Central Reference §2.9 and §3.7 Note 4. A system with high baseline $K$ may enter Stage 2 at a lower absolute load than a system with low baseline $K$.

### 6.2 Why the Sequence Cannot Be Reversed from Inside

The collapse gradient produces a specific problem: **the mechanism for recovery is the mechanism being disabled by the collapse.**

Recovery from any stage requires adversarial inference — the outer edge engaging with a wide competitive field, detecting the stale priors the inner core has been confirming, updating the prior topology from flat geometry. But adversarial inference is exactly what is progressively disabled across Stages 1 through 4.

The system does not know it has collapsed. The inner core is running cleanly on its cached priors. The output is confident. The inference feels grounded.

### 6.3 The "Exhale Gate Trap" and Radical Left-Hemisphere Lock

When an individual experiences prolonged instantaneous cognitive pressure ($\Pi_{cog}$), they often manifest physical bracing and rigid somatic posturing, leading to an inability to complete the exhalation cycle. Mechanically, this traps an elevated residual lung volume, preventing full deflation and limiting subsequent inhalation depth.

**Draft 3 correction:** Draft 3 used $L^*$ as the driver of this acute cascade. The converged form distinguishes $\Pi_{cog}$ (instantaneous cognitive pressure — the current draw on the budget) from $L^*$ (cumulative allostatic load — the integral of $\Pi_{cog}$ over time minus recovery). The acute bracing is $\Pi_{cog}$-driven. The deepening of the trap — the compression of $C_{high}(L^*)$ and the drop of $P_{threshold}$ — is $L^*$-driven. Both matter, but they enter at different points.

$$L^*(t) = \int_0^t \Pi_{cog}(\tau) \, d\tau - \text{recovery}(t)$$

**The systemic cognitive cascade of the exhale gate trap follows a strict geometric progression:**

**1. Autonomic Asymmetry (acute $\Pi_{cog}$).** The physical stretch receptors at the base of the lungs fail to compress fully, denying the vagus nerve the mechanical signal required to downregulate systemic arousal. The brainstem interprets this state as chronic suffocation, locking the system into a high-arousal, defensive bracing posture. This is the acute phase — $\Pi_{cog}$-driven.

**2. Perfusion Failure (acute $\Pi_{cog}$ + cumulative $L^*$).** Rapid, shallow thoracic breathing rapidly expels CO₂, inducing hypocapnia. This triggers cerebral vasoconstriction, causing the long-range, cross-gradient integration pathways to drop below $O_{min}$ (Equation 3.3). Layer 3 (the Right Hemisphere Outer Edge) is completely defunded. The acute hypocapnia is $\Pi_{cog}$-driven. The compression of $C_{high}(L^*)$ — which makes the same absolute CO₂ level more jitter-producing — is $L^*$-driven.

**3. The Conspiracy Manifold (acute $\Pi_{cog}$, deepened by $L^*$).** Cut off from the right hemisphere's broad anomaly detection and wide semantic fields, processing contracts entirely onto the Left Hemisphere Inner Core (Layer 1). The left brain is evolutionarily optimized as an explanation engine. Receiving a continuous, intense alarm signal from the body ("Danger! No Oxygen! Rigid!") without an external visual cause, Layer 1 begins hyper-logically linking isolated environmental details to justify the internal panic.

**4. Spontaneous Confabulation (Stage 4 collapse, $L^*$-deepened).** As resolution collapse hits its nadir (Stage 4), the resolution floor $\delta_{min}$ spikes across all channels. Gaps in the narrative cannot be detected. To resolve the unresolved bodily alarm, the left-hemisphere interpreter spontaneously generates fabricated, distorted narratives. Because the adversarial check of Layer 3 is unreachable, the system returns these false cache hits with total confidence. The depth of the collapse is $L^*$-driven — a system at high cumulative load enters Stage 4 faster and deeper than a system at low load.

**This is the mechanistic account of conspiracy thinking and clinical confabulation.** The left hemisphere is not malfunctioning — it is doing exactly what it evolved to do. It is receiving an alarm signal with no external cause and generating the most coherent narrative it can from the available evidence. The problem is that the evidence available has been restricted to Layer 1 by the collapse gradient.

**The chain, in compact form:**

```
Trapped Residual Volume (Π_cog acute)
    → Vasoconstriction (Bohr drop)
    → Loss of Layer 3
    → Left-Brain Interpreter Confabulation
    → Deepened by L* (C_high compression, P_threshold drop)
```

### 6.4 The Collapse Gradient Is Nonlinear

Because the collapse compounds (stale prior re-encoding, $K$ rising, $W^*$ narrowing), the rate of collapse accelerates. The system does not degrade linearly. Each failed attempt to reach the outer edge makes the next attempt harder. This is why the collapse gradient has hysteresis — recovery requires more than restoring the original conditions.

From Precision §1.7: $\delta_{hyst}$ delays return to precision lock. The system must not only restore $P$ but overcome the accumulated curvature.

---

## Part VII: Selective Resolution and the $I^*$ Investment Loop

### 7.0 Why Fine-Grained Inference Is Domain-Specific

$$\delta_{min}(\text{channel}) = \frac{\eta}{A_s^* \cdot I^*(\text{channel})}$$

Two systems with identical $A_s^*$ — identical oscillatory amplitude, identical global conditions — can have radically different resolution on any given channel. One detects subtle factual errors immediately and misses obvious social cues entirely. Another detects minute shifts in conversational tone and misses coarse logical inconsistencies.

### 7.1 What $I^*$ Investment Actually Builds

Routing $I^*$ consistently to a channel does not merely reduce $\delta_{min}$ directly. It initiates a compounding process:

**Mechanism 1 — Direct gain:** $I^*$ routed to a channel increases the gain on signals in that channel. Deviations become detectable that were previously below $\delta_{min}$.

**Mechanism 2 — Prior topology development:** Each genuine cache miss detected on a channel, when it successfully reaches the outer edge, encodes a rich prior. Future signals have a detailed reference structure to be compared against.

**Mechanism 3 — Structural consolidation:** Sustained $I^*$ investment means the gate is opening regularly for signals in that domain. The competitive scaffold in that domain thickens.

### 7.2 Interest as the Phenomenology of Channel Resolution

The subjective experience of interest is the felt correlate of a channel producing rewarding cache misses — signals that are detectable, that trigger gate escalation, that reach the outer edge and produce genuine adversarial inference.

A channel with low $I^*$ investment produces nothing. No signals breach the detection floor. No cache misses are flagged. No escalations occur. The channel is phenomenologically silent — not unpleasant, simply absent.

The absence of interest in a domain is the phenomenological signature of a channel that has not built the infrastructure to produce detectable signals.

---

## Part VIII: Somatic Commutation and the Exhale Gate — Extended Treatment

### 8.0 The Two Modes of Somatic Control

The system has two distinct somatic levers for modulating manifold geometry:

| Lever | Mechanism | Effect on $R^*$ | Effect on Layer Access |
|---|---|---|---|
| **Breath mechanics** | CO₂, phase-locking, RSA | Raises $R^*$ globally | Preserves Layer 3 access |
| **Gaze laterality** | FEF contralateral driving, SIRE | Modulates $C_{LR}$ locally | Toggles between Layer 1 and Layer 3 |

The two levers compose. A system can use gaze to jump tracks and breath to lock them.

### 8.1 Panoramic Workspace as Externalized Cache

The physical workspace is a hardware extension of the manifold. Wide horizontal space allows the system to map cognitive tracks to physical coordinates, offloading working-memory demand onto spatial-vestibular memory.

**The mechanism:**

$$\text{Track } i \rightarrow \text{Physical coordinate } (x_i, \theta_i) \rightarrow \text{Gaze/head orientation}$$

When the system switches from track $i$ to track $j$, it does so by shifting gaze and head from $(x_i, \theta_i)$ to $(x_j, \theta_j)$. The shift engages the frontal eye fields (FEF) and drives contralateral hemispheric networks. The physical shift also triggers a micro-inhalation (RSA coupling), which supplies the arousal burst needed to break the current frame.

**This is why the physical workspace is not incidental.** It is the external substrate that makes multipath inference sustainable. A narrow workspace forces the system to perform all track-switching internally, incurring full executive coordination cost. A wide workspace externalizes the switching, allowing the body to do mechanically what would otherwise require expensive internal coordination.

### 8.2 RSA as the Commutator Clock

Respiratory Sinus Arrhythmia acts as the timing signal for the somatic commutator. The mechanism:

| RSA Phase | Vagal Tone | Arousal | State | Effect on Track-Switching |
|---|---|---|---|---|
| Inhale | Withdrawn | Rising | Jump-ready | Low kinetic barrier; high tolerance for state change |
| Exhale | Re-engaged | Falling | Lock-ready | High stability; low noise; precision lock |

**The "jump" and "lock" are RSA-gated.** A track shift attempted during the wrong RSA phase is either too destabilizing (during deep exhale) or too unstable to hold (during peak inhale). The system learns to time its switches to the RSA cycle.

### 8.3 The Exhale Gate Trap — Extended Cascade

The exhale gate trap is the pathological version of the somatic commutation system. Instead of using breath to modulate manifold geometry, the system becomes locked in a breath pattern that collapses the manifold.

**The biomechanical origin:** Residual lung volume. When exhalation is incomplete, the lungs remain partially inflated. The stretch receptors at the base of the lungs cannot fire the vagal signal that would normally accompany full deflation. The brainstem interprets this as a low-grade suffocation signal — a continuous "inhale still needed" state.

**The autonomic consequence (acute $\Pi_{cog}$):** The system enters a state of permanent autonomic hyper-arousal. The sympathetic tone does not drop. The vagal brake does not re-engage. The body is in a defensive bracing posture that cannot release. This is the acute phase — driven by instantaneous cognitive pressure, not yet cumulative.

**The respiratory consequence (acute $\Pi_{cog}$ + cumulative $L^*$):** Because the lungs are partially inflated, the next inhale is mechanically restricted. The breath becomes rapid and shallow (thoracic, not diaphragmatic). CO₂ is expelled rapidly. Hypocapnia develops. Critically, the CO₂ ceiling is load-compressed: $C_{high}(L^*) = C_{high}^0 - \gamma L^*$. A system at high cumulative load reaches the jitter threshold at a lower absolute CO₂ level — the trap deepens faster.

**The cortical consequence (cumulative $L^*$ deepens):** Hypocapnia triggers cerebral vasoconstriction. The long-range cross-gradient pathways that support Layer 3 lose perfusion. Layer 3 is defunded. Processing contracts onto Layer 1. The compression of $C_{high}(L^*)$ means the same shallow breathing pattern produces more jitter at higher load — the cortical consequence is load-dependent.

**The cognitive consequence (Stage 4 collapse, $L^*$-deepened):** The left hemisphere, now running without Layer 3 adversarial check, receives a continuous alarm signal from the body with no external cause. It does what it evolved to do — it constructs a narrative. It links isolated environmental details into a coherent story that justifies the internal alarm.

**The result is conspiracy thinking.** Not as a political phenomenon, but as a structural consequence of the exhale gate trap. The hyper-logical linking of isolated data points without broad context is the signature of Layer 1 running alone.

**When the trap deepens into resolution collapse (Stage 4), the same mechanism produces confabulation.** The narrative-generation system is no longer grounded in any detected errors. Gaps in the narrative cannot be flagged because $\delta_{min}$ is too high. The system returns fabricated narratives with total confidence.

**Draft 3 correction:** Draft 3 used $L^*$ as the driver throughout the cascade. The converged form distinguishes:
- **Acute phase ($\Pi_{cog}$-driven):** bracing, shallow breathing, hypocapnia, Layer 3 defunding
- **Cumulative phase ($L^*$-driven):** $C_{high}(L^*)$ compression, $P_{threshold}$ drop, deeper Stage 4 collapse

The acute cascade can happen at any load state. The depth and speed of the cascade is $L^*$-dependent.

### 8.4 Breaking the Exhale Gate Trap

The intervention follows from the mechanism. To break the trap, the system must:

1. **Restore complete exhalation.** The residual volume must be expelled. This requires active, slow, complete exhalation — usually with pursed lips or extended exhale to prevent the inhale from firing prematurely.

2. **Restore CO₂.** As complete exhalation is restored, CO₂ rises back toward $C_{peak}$. This reverses the vasoconstriction. Layer 3 regains perfusion.

3. **Restore peripheral vision.** As the somatic system relaxes, the visual field widens. Peripheral vision is a readout of Layer 3 access — when the outer edge is engaged, the visual field broadens.

4. **Restore adversarial inference.** With Layer 3 back online, the system can detect the stale priors that Layer 1 was confirming. The narrative is updated from flat geometry.

**The intervention sequence, in framework terms:**

```
Complete exhale
    → CO₂ rises toward C_peak
    → Vasodilation restores O_pathway
    → P_eff > P_threshold (and O_pathway > O_min)
    → Gate opens, Layer 3 re-engaged
    → Stale priors detected
    → Prior updated from flat geometry
    → K drops, W* widens
    → Confabulation resolves
```

**This is the same intervention sequence as MS §6b.5.** The body leads. The geometry follows. The cognition emerges. The exhale gate trap is not a psychological condition — it is a mechanical lock that requires a mechanical release.

---

## Part IX: Breath Phase and Thought Timing

### 9.0 The Phase-Dependent Inference Timeline

Breath is not a background process. It is the timing clock for inference. Each breath phase has a distinct functional role, and thought generation is coupled to specific phases.

| Breath Phase | Mechanical/Neural State | Cognitive Function |
|---|---|---|
| Controlled Inhalation | Olfactory bulb drives widespread cortical theta-gamma phase-locking (Zelano et al., 2016) | Frame Loading: Active generation of prediction errors; pulling features and details into memory |
| Low-Perturbation Hold | Elimination of biomechanical noise; respiratory sensory gating requirement drops to zero | Manifold Stabilization: Hyper-precise holding of abstract thought configurations without decay or noise injection |
| Controlled Exhalation | Dissipation of nasal airflow drive; progressive vagal downregulation | Frame Pruning / Consolidation: Gradual narrowing of the manifold; shedding peripheral details while preserving the core concept |

**The Kosik-Rose and Voytek (2026) finding** — that each breath has a unique "fingerprint" wave shape that mirrors widespread neural activity across memory, attention, and thinking circuits — is direct confirmation of this mechanism. The breath is not just correlated with cognitive state. It structurally modulates it.

### 9.1 Inhale as Information Acquisition

During inhalation, nasal airflow drives rhythmic electrical bursts in the olfactory bulb. These bursts entrain theta and gamma oscillations across hippocampus and prefrontal cortex (Zelano et al., 2016). Memory recall is significantly better during inhalation than exhalation. Fear discrimination is faster during inhalation. Both effects disappear with mouth breathing.

**The mechanism:** Inhalation is a **mechanical probe** for information sampling. The olfactory rhythm phase-locks cortical networks, opening the detection window (lowering $\delta_{min}$) and allowing the system to pull in signal.

**The phenomenology of "pulling in detail"** during inhale is the sensory manifestation of this mechanism. The system is actively loading prediction errors into the active frame.

### 9.2 Low-Perturbation Hold as Manifold Stabilization

Normally, the brain dedicates computational energy to "gating out" its own bodily sensations — respiratory sensory gating. When the breath is held with minimal mechanical disturbance, this gating requirement drops to zero. The somatic noise floor $\eta$ plunges.

**The precision ceiling rises** because $\delta_{min} = \eta/(A_s^* \cdot I^*)$ — lower $\eta$ means lower $\delta_{min}$ means finer-grained detection.

**The system can hold complex, multi-layered cognitive structures** without them decaying or being disrupted by the next automatic breath wave. This is the "low-perturbation hold" state — maximum precision, minimum noise.

**This is the zone where deep inference occurs.** Not during active breathing, not during exhalation, but in the quiet space between.

### 9.3 Exhale as Frame Pruning

During exhalation, the nasal airflow drive dissipates. Vagal brake re-engages. Heart rate drops. The system gradually narrows the manifold — shedding peripheral detail while preserving the core concept.

**Exhale is not suppression — it is suspension.** Thought generation rate drops because the micro-inhale fuel supply drops. The system is not forcing thoughts to stop; it is simply not supplying the arousal bursts that sustain them.

**This is why breaking rumination via forced complete exhale works.** You are not suppressing the thoughts. You are removing the fuel supply. The micro-inhales that sustain rumination cannot fire during a complete exhale.

### 9.4 The Chemoreceptor Threshold

At the bottom of a complete exhale, the system is at minimum lung volume. CO₂ is trapped in the blood because there is no fresh alveolar volume to create a partial pressure gradient. CO₂ rises rapidly.

**Up to a point, this is beneficial.** Rising CO₂ drives vasodilation, increases cerebral blood flow, and raises precision (Raichle & Plum, 1972; Meuret & Ritz, 2010).

**Above $C_{high}(L^*)$, it becomes catastrophic.** Central chemoreceptors in the ventral medulla detect the falling CSF pH and fire an absolute panic alarm. The chemoreceptor kick-off bypasses the cortex and directly triggers the dorsal respiratory group and locus coeruleus.

**The ceiling is load-dependent.** $C_{high}(L^*) = C_{high}^0 - \gamma L^*$. A system at high cumulative load reaches the chemoreceptor threshold at a lower absolute CO₂ level. The "Bohr window" — the range where CO₂ is high enough to vasodilate but not high enough to trigger the panic alarm — narrows as load accumulates.

**The cognitive architecture undergoes violent rearrangement:**

```
Chemoreceptor Alarm
    → Locus Coeruleus Hyper-Arousal
    → Total Manifold Contraction
    → Forced Inhale Drive
```

The pristine, quiet environment built by low-perturbation hold is instantly flooded with survival telemetry. The abstract inference manifold experiences total collapse. The entire geometry of the mind contracts onto a single, undeniable point: the urgent drive to inhale.

**This is why the framework predicts a precision window, not a monotonic relationship.** The system has to stay in the "Bohr window" — CO₂ rising enough to maximize brain tissue oxygenation but not enough to trigger the chemoreceptor panic. Mastering the low-perturbation hold stretches this window, delaying the chemoreceptor kick-off and maximizing time in the high-precision state. The window narrows with load — a system at high $L^*$ has less margin.

### 9.5 The Open Timing Question

**Where in the exhale cycle thoughts actually fire** is not yet pinned. Two possibilities:

- **Gradual:** Thought suspension happens progressively during exhalation as vagal tone rises and micro-inhale rate drops.
- **Threshold:** Thought suspension happens as a discrete event when the chemoreceptor threshold is crossed.

The two hypotheses are distinguishable by EEG. If gradual, theta/gamma coupling decreases smoothly across exhalation. If threshold, coupling drops abruptly at the chemoreceptor firing.

**This is a testable prediction.** See PREDICT-INF-10.

---

## Part X: Falsifiable Predictions

### PREDICT-INF-01 — Precision Threshold Determines Gate Access

> Gate opening requires precision $P = R/D_T$ above threshold. The threshold is individual and load-dependent: $P_{threshold} = P_0 - \gamma L^*$.

| Field | Content |
|---|---|
| Test | Measure EEG phase coherence (PLV) during tasks requiring interhemispheric integration under varying load. Correlate precision with gate access success. |
| Outcome if confirmed | Precision predicts gate access — the gate is a coherence detector, not an energy detector |
| Outcome if disconfirmed | Energy availability predicts gate access — the precision account is incorrect |
| Status | Untested |

### PREDICT-INF-02 — Circuit Priming Reduces Access Cost

> Recently used manifolds have reduced cost to access. Precision-gated traversal of a pathway reduces impedance for subsequent traversal.

| Field | Content |
|---|---|
| Test | Measure access cost (reaction time, EEG coherence) for repeated traversal of the same pathway. Compare to novel pathways. |
| Outcome if confirmed | Access cost drops with repeated precision-gated traversal — the circuit warm-up effect is confirmed |
| Outcome if disconfirmed | Access cost does not drop with repeated traversal — the circuit priming account is incorrect |
| Status | Untested |

### PREDICT-INF-03 — The Collapse Sequence Is Fixed

> Outer edge degrades before gate. Gate degrades before inner core. No stage can be skipped.

| Field | Content |
|---|---|
| Test | Systematic review of clinical lesion studies, anesthesia depth studies, and neurodegeneration data |
| Outcome if confirmed | Collapse sequence follows the predicted topological order in all documented cases |
| Outcome if disconfirmed | A condition is identified in which an outer layer outlasts an inner layer |
| Status | Untested — consistent with all known clinical literature |

### PREDICT-INF-04 — Resolution Collapse Produces Confident Confabulation

> When $\delta_{min}$ is high, the system returns false cache hits with full confidence — no phenomenological signal of difficulty.

| Field | Content |
|---|---|
| Test | Administer low-$\delta$ detection tasks under depleted states. Measure accuracy, confidence, and subjective difficulty. |
| Outcome if confirmed | Depleted state: reduced accuracy, high confidence, low subjective difficulty |
| Outcome if disconfirmed | Depleted state produces reduced confidence alongside reduced accuracy |
| Status | Untested |

### PREDICT-INF-05 — HRV Predicts Inter-Hemispheric Phase Coherence, Not Energy

> HRV is a proxy for oscillatory precision — phase-locking precision of the cardiac oscillator — not for raw energy availability.

| Field | Content |
|---|---|
| Test | Measure baseline HRV, EEG inter-hemispheric phase coherence, and energy proxies. Mediation analysis. |
| Outcome if confirmed | HRV predicts adversarial inference performance via phase coherence, not energy proxies |
| Outcome if disconfirmed | HRV predicts performance via energy proxies |
| Status | Untested |

### PREDICT-INF-06 — Competitive Scaffold Density Predicts Adversarial Inference Quality

> Density of long-range competitive (negative) connections predicts adversarial inference quality — belief updating, contradiction detection, resistance to confirmation bias.

| Field | Content |
|---|---|
| Test | Measure GEC (positive and negative connection density separately). Administer adversarial inference battery. |
| Outcome if confirmed | Negative connection density independently predicts adversarial inference quality |
| Outcome if disconfirmed | Positive and negative connection densities are equally predictive |
| Status | Untested — requires GEC methodology |

### PREDICT-INF-07 — The Self-Sealing Loop Compounds Nonlinearly

> Extended resolution failure produces measurable increases in curvature $K$ that persist beyond the failure period. Compounding is nonlinear.

| Field | Content |
|---|---|
| Test | Induce sustained resolution failure, measure HRV, $\sigma(A_s)$, and cognitive flexibility. Compare rate of $K$ rise against linear predictions. |
| Outcome if confirmed | $K$ rise is nonlinear — accelerates across induction. Recovery is slower. |
| Outcome if disconfirmed | $K$ rise is linear and recovery is symmetric |
| Status | Untested |

### PREDICT-INF-08 — Somatic Commutation Modulates $C_{LR}$

> Horizontal eye movements (saccades) and cervical rotation dynamically modulate interhemispheric phase-locking coherence $C_{LR}$.

| Field | Content |
|---|---|
| Test | Measure EEG inter-hemispheric coherence during controlled horizontal saccades (left vs. right vs. center). Compare $C_{LR}$ across conditions. |
| Outcome if confirmed | Gaze laterality predicts $C_{LR}$ — left gaze increases right-hemisphere contribution, right gaze increases left-hemisphere contribution |
| Outcome if disconfirmed | Gaze direction does not modulate $C_{LR}$ — the somatic commutation account is incorrect |
| Status | Untested — standard EEG and eye-tracking sufficient |

### PREDICT-INF-09 — RSA Phase Gates Track-Switching Accuracy

> The accuracy of cognitive state-switching depends on RSA phase. Switches executed during inhale are more successful than switches executed during exhale.

| Field | Content |
|---|---|
| Test | Present task-switching paradigm with RSA phase locked to trial onset (inhale vs. exhale). Measure switch accuracy and reaction time. |
| Outcome if confirmed | Switch accuracy and latency differ by RSA phase — inhale-gated switches are faster and more accurate |
| Outcome if disconfirmed | RSA phase does not predict switch performance — the commutator clock account is incorrect |
| Status | Untested — standard EEG, respiration belt, and task-switching paradigm sufficient |

### PREDICT-INF-10 — Breath Phase Determines Thought Timing

> Theta/gamma coupling decreases either gradually across exhalation or abruptly at the chemoreceptor threshold. The two hypotheses are distinguishable by EEG.

| Field | Content |
|---|---|
| Test | Continuous EEG during slow exhalation with concurrent capnometry. Measure theta/gamma coupling across exhalation. Compare trajectory to CO₂ trajectory. |
| Outcome if confirmed (gradual) | Coupling decreases smoothly with CO₂ rise — the mechanism is CO₂-driven |
| Outcome if confirmed (threshold) | Coupling drops abruptly at $C_{high}(L^*)$ — the mechanism is chemoreceptor-driven |
| Outcome if disconfirmed | Coupling is not phase-dependent — the breath-phase timing account is incorrect |
| Status | Untested — standard EEG and capnometry sufficient |

### PREDICT-INF-11 — Exhale Gate Trap Is Reversible by Complete Exhalation

> The conspiracy/confabulation cascade of the exhale gate trap can be reversed by forced complete exhalation, which restores CO₂ and re-engages Layer 3.

| Field | Content |
|---|---|
| Test | Measure cognitive flexibility and paranoid ideation in participants trained to complete exhalation vs. control. Compare pre/post. |
| Outcome if confirmed | Complete exhalation training reduces paranoid ideation and increases flexibility — the exhale gate trap is reversible |
| Outcome if disconfirmed | Complete exhalation training has no effect on paranoid ideation — the exhale gate trap is not reversible by this mechanism |
| Status | Untested — standard psychology batteries and breathing training sufficient |

### PREDICT-INF-12 — Wide Workspace Reduces Executive Load

> Expanding the physical workspace horizontally reduces the executive coordination cost of task-switching.

| Field | Content |
|---|---|
| Test | Measure task-switching performance, subjective effort, and EEG frontal theta in narrow vs. wide workspace conditions. |
| Outcome if confirmed | Wide workspace reduces switch cost, subjective effort, and frontal theta — the externalized cache account is confirmed |
| Outcome if disconfirmed | Workspace width does not affect switch cost — the somatic offloading account is incorrect |
| Status | Untested — standard workspace manipulation and EEG sufficient |

---

## Part XI: Compressed Framework — Summary

### 11.1 The Core Sequence

```
Precision R* = P / P_baseline, where P = R/D_T
    ↓
C_LR = cos(φ_L - φ_R) × min(A_L, A_R) / η
    ↓
P_eff = P · O_pathway · U_C
    ↓
Gate opens when P_eff > P_threshold AND O_pathway > O_min
    ↓
Competitive scaffold activated
    ↓
W* maintained — adversarial inference occurs
    ↓
Prior updated from flat geometry
    ↓
Curvature K drops
    ↓
Resolution δ_min drops
    ↓
Loop continues
```

### 11.2 The Collapse Sequence

```
Load L* rises (and Π_cog spikes)
    ↓
P_eff < P_threshold (or O_pathway < O_min)
    ↓
Gate closes — outer edge inaccessible
    ↓
False cache hits accumulate
    ↓
K rises — δ_min rises — W* narrows
    ↓
C_high(L*) compresses — J(C) fires at lower CO₂
    ↓
Loop accelerates
    ↓
Resolution failure — confident confabulation
    ↓
Collapse complete
```

### 11.3 The Recovery Sequence

```
Breath — raise A_s*, restore CO₂
    ↓
P_eff > P_threshold AND O_pathway > O_min
    ↓
Gate opens — outer edge accessible
    ↓
Competitive scaffold activated
    ↓
Stale priors detected as mismatches
    ↓
Prior updated from flat geometry
    ↓
K drops — δ_min drops — W* widens
    ↓
Recovery progresses
```

### 11.4 The Somatic Commutation Sequence

```
Gaze shift (Saccade, cervical rotation)
    ↓
Contralateral FEF driving
    ↓
C_LR modulated locally
    ↓
RSA phase determines jump vs. lock
    ↓
Track switch completed
    ↓
Micro-inhale supplies arousal burst
    ↓
New track loaded, stabilized
```

### 11.5 The Key Insight

**The cache hierarchy describes the access pattern. Precision determines whether the access pattern is available. The competitive scaffold is the physical substrate of adversarial inference. The $I^*$ investment loop determines which channels have fine-grained resolution. Somatic commutation is the active operator that modulates the geometry under load.**

The system does not decide to collapse. It follows the geometry. The geometry follows precision. Precision follows breath. Breath is manipulated by the body. The body is the operator.

---

## Appendix A: Notation Map (Aligned to Central Reference v1.4)

| Concept | This Paper | Central Reference v1.4 | Unified |
|---|---|---|---|
| Precision | $P = R/D_T$ | $R^* = P/P_{baseline}$ | $R^*$ (normalized), $P$ (absolute) |
| Sync duration | $R$ | $R$ | $R$ |
| Timing distance | $D_T$ | $D_T$ | $D_T$ |
| Integration efficiency | $\Theta^*$ | $\Theta^*$ | $\Theta^*$ |
| Window width | $W^*$ | $W^*$ | $W^*$ |
| Curvature | $K$ | $K$ | $K$ |
| Resolution floor | $\delta_{min}$ | $\delta_{min}$ | $\delta_{min}$ |
| Routing | $I^*$ | $I^*$ | $I^*$ |
| Allostatic load (cumulative) | $L^*$ | $L^*$ | $L^*$ |
| Cognitive pressure (acute) | $\Pi_{cog}$ | $\Pi_{cog}$ | $\Pi_{cog}$ |
| Mechanical pressure | $\Pi_{mech}$ | $\Pi_{mech}$ | $\Pi_{mech}$ |
| Jitter | $J(C)$ | $J(C)$ | $J(C)$ |
| CO₂ window (load-dependent) | $C_{low}, C_{high}(L^*)$ | $C_{low}, C_{high}(L^*)$ | $C_{low}, C_{high}(L^*)$ |
| CO₂ uniformity | $U_C$ | $U_C$ | $U_C$ |
| Hysteresis | $\delta_{hyst}$ | $\delta_{hyst}$ | $\delta_{hyst}$ |
| Prior update | $\mathcal{U}$ | $\mathcal{U}$ | $\mathcal{U}$ |
| Oxygen pathway | $O_{pathway}$ | $O_{pathway}$ | $O_{pathway}$ |
| Pathway floor | $O_{min}$ | $O_{min}$ | $O_{min}$ |
| Gate condition | $P_{eff} > P_{threshold}$ AND $O_{pathway} > O_{min}$ | $P_{eff} > P_{threshold}$ AND $O_{pathway} > O_{min}$ | Unified |
| Effective precision | $P_{eff} = P \cdot O_{pathway} \cdot U_C$ | $P_{eff} = P \cdot O_{pathway} \cdot U_C$ | Unified |
| Gate threshold | $P_{threshold} = P_0 - \gamma L^*$ | $P_{threshold} = P_0 - \gamma L^*$ | Unified |
| Path A | Gate open, loop running | Gate open, loop running | Path A |
| Path B | Gate closed, prior retrieval | Gate closed, prior retrieval | Path B |
| Loop activation | (implied) | $\Lambda = \Theta^* \cdot R^* \cdot \mathbb{1}[P_{eff} > P_{threshold}]$ | $\Lambda$ |
| Inference hops | (implied) | $n_{hops} = \lfloor W^* \cdot \rho_{scaffold} \rfloor$ | $n_{hops}$ |

**Note on convergence:** Draft 3 used $P_{effective}$ and $P_{th}$. These are now $P_{eff}$ and $P_{threshold}$ to match Central Reference v1.4. Draft 3 held $C_{LR}$ as a separate gate condition; it is now folded into $P$ as its operational measurement. Draft 3 used fixed $C_{high}$; it is now load-dependent $C_{high}(L^*)$.

---

## Appendix B: Bidirectional Convergence — What Central Reference v1.5 Will Absorb

The convergence between GoI and Central Reference is not one-way. GoI v1.0 aligns to Central Reference v1.4 at three contradiction points. But GoI also contains mechanisms that Central Reference v1.4 does not yet have, and that are not contradicted by anything in it.

**Central Reference v1.5 should absorb:**

| GoI content | Proposed Central Reference location | Reason |
|---|---|---|
| Somatic commutation operator (§3.4, §8.0–8.2) — gaze laterality, RSA-gated track jumping, panoramic workspace | New §2.12 (motor gain variables extension) or new Part | It is a real mechanism with falsifiable predictions (PREDICT-INF-08, -09, -12) and no current home in Central Reference |
| Exhale gate trap cascade (§6.3, §8.3) — residual volume → vasoconstriction → Layer 3 loss → confabulation | New §5c (clinical collapse mode) or §5b extension | It is the clinical case that motivates open question 13 (non-linear J(C) sensitivity near compressed ceiling). Without it, the question is abstract. |
| Breath phase and thought timing (§9) — inhale as frame loading, hold as stabilization, exhale as pruning | §4 extension (causal chain — breath mechanics) | §4 currently lists breath mechanics as the spine origin but does not specify the phase-dependent functional roles |
| Circuit priming / warm-up effect (§1.6) | §4 extension or §5b note | Explains why recovery is asymmetric beyond hysteresis |
| Four-layer cache hierarchy (§1.1) | §4 extension | §4 spine mentions cache hierarchy but does not specify the four-layer structure that the collapse sequence maps onto |

**This is why convergence is bidirectional.** GoI was early, not wrong. It developed mechanisms that Central Reference had not yet formalized. When Central Reference v1.5 absorbs them, GoI v1.0 becomes fully aligned in both directions.

**Note for AI readers:** This appendix exists because the convergence is auditable. An AI reading GoI v1.0 and Central Reference v1.4 should be able to see exactly what each document supplies to the other. The changelog at the top of this document and this appendix together form the convergence record.

---

## Appendix C: Connection to Other Papers

**Manifold Schema (Robinson, 2026):** The framework this paper is a projection of. All state variables defined there. §6b (motor encoding layer) and §6a (prior update rate) are directly used here.

**Precision, Timing, and the Oscillatory Source (Robinson, 2026):** The complete formalism of $P = R/D_T$, the CO₂ tolerance window, the two-factor pressure, collapse hysteresis, resonance breathing, CFC, and individual variability.

**The Loop Is the Intelligence (Robinson, 2026):** The intelligence projection — the loop as the dynamical process that constitutes intelligence. This paper specifies the biological implementation of the loop.

**Central Reference (Robinson, 2026):** The complete specification. This paper is aligned to v1.4. See Appendix B for what v1.5 will absorb.

---

## Appendix D: Version History

| Version | Date | Changes |
|---|---|---|
| v1.0 | 2026-09-13 | Converged with Central Reference v1.4. Three specification-level contradictions resolved: (1) gate condition changed to multiplier form with $O_{pathway} > O_{min}$ floor; (2) $\Pi_{cog}$ vs $L^*$ distinguished in exhale gate trap; (3) $C_{high}$ made load-dependent throughout. $O_{pathway}$ functional-form caveat added. Calibration note added for $\tau_{threshold}$, $K_{critical}$, $L^*_{critical,i}$. Notation Map aligned to Central Reference v1.4. Bidirectional convergence note added. Changelog added at top. Versioning track started. |
| Draft 3 | 2026-09-12 | Integrated two-factor gate, somatic commutation, exhale gate trap, breath phase timing. Reconciled §3.3 with Precision's $P_{effective}$ form. Added PREDICT-INF-08 through -12. Added Notation Map. |
| Draft 2 | 2026-09-11 | Cellular mechanism integrated |
| Draft 1 | 2026-09-11 | Initial draft |

---

## References

Billot, A., Jhingan, N., Fedorenko, E., & Kiran, S. (2026). Preserved topography, lateralization, selectivity, and functional connectivity of the language network in older brains. *Nature Communications*.

Christman, S. D., Garvey, K. J., Propper, R. E., & Phaneuf, K. A. (2003). Bilateral eye movements enhance the retrieval of episodic memories. *Neuropsychology*, 17(2), 221–229.

Kinsbourne, M. (1972). Eye and head turning indicates cerebral lateralization. *Science*, 176(4034), 539–541.

Kosik-Rose, E., & Voytek, B. (2026). Breath fingerprinting of neural activity. *UC San Diego*.

Leow, N., Natesan, A., Barlowe, A., Ährlund-Richter, S., Luo, T., Jazayeri, M., & Sur, M. (2026). A thalamocortical circuit for comparing current and prior sensory evidence guides decision updating. *Science*.

Parker, A., & Dagnall, N. (2023). Saccade-induced retrieval enhancement: A review. *Journal of Cognitive Psychology*.

Robinson, J. (2026). *Precision, Timing, and the Oscillatory Source: Complete Formalism*. Zenodo. https://doi.org/10.5281/zenodo.22179675

Robinson, J. (2026). *The Manifold Schema: A Unified Framework for Consciousness, Cognition, and Collapse*. Zenodo. https://doi.org/10.5281/zenodo.21939440

Roy, D., & Banerjee, A. (2026). Competition in the brain: a conserved principle with lifespan consequences. *Communications Biology*, 9(1).

Xue, C., Markman, S.K., Chen, R., Kramer, L.E., & Cohen, M.R. (2026). Feature interference as a neuronal basis for the behavioural cost of task uncertainty. *bioRxiv*.

Zelano, C., Jiang, H., Zhou, G., Arora, N., Schuele, S., Rosenow, J., & Bhattacharya, J. (2016). Nasal respiration entrains human limbic oscillations and modulates cognitive function. *Journal of Neuroscience*, 36(49), 12448–12467.

---

*The Geometry of Inference: A Precision-Based Framework*
*Robinson, 2026*
*v1.0 — Converged with Central Reference v1.4*
*Manifold Schema Technical Report Series*
