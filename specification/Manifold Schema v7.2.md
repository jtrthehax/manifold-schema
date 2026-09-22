# The Manifold Schema: A Unified Framework for Consciousness, Cognition, and Collapse

**Robinson, 2026**

*Canonical Reference. All subsequent work is a domain projection of this framework.*

**Version:** 7.2
**Date:** 2026-09-13
**Status:** Converged with Central Reference v1.4, Precision v3.4, Allostatic Load v2.1, Geometry of Inference v1.0, and Loop Is the Intelligence v1.0

---

## Changelog — v7.1 → v7.2

This changelog exists so that any reader — human or AI — can see the convergence path. MS v7.1 was assembled against Central Reference v1.3. The v1.3 → v1.4 delta added $O_{pathway}$ (§2.8), $L^*_{critical,i}$ (§2.9), and the motor gain variables (§2.11). Additionally, GoI v1.0 introduced the four-layer cache hierarchy and circuit priming effect. MS v7.1 absorbed neither. v7.2 applies the seven specification fixes and absorbs the two GoI mechanisms.

| Step | Change | Location | Reason | Central Reference anchor |
|---|---|---|---|---|
| 1 | Header updated to "Converged with Central Reference v1.4" | Header | Version drift | — |
| 2 | Added $O_{pathway}$, $\Lambda$, $n_{hops}$, $\rho_{scaffold}$, $\delta_{hyst}$ to variable table | §2b | Central Reference v1.4 registers these | §2.2, §2.3, §2.6, §2.8 |
| 3 | Registered $\delta_{hyst}$ with decay equation | §5a.5 | Variable was described but not registered | §2.3, §3.3 |
| 4 | Added $L^*_{critical,i}$ with calibration note | §5a.14 | Component critical load variable | §2.9 |
| 5 | Motor gain formalization (new §6b.8) | §6b.8 | Absorbed from Central Reference §2.11 and §3.11 | §2.11, §3.11 |
| 6 | Four-layer cache hierarchy (new §6b.9) | §6b.9 | Absorbed from GoI v1.0 §1.1 | — |
| 7 | Circuit priming (new §6b.10) | §6b.10 | Absorbed from GoI v1.0 §1.6 | — |
| 8 | Added GoI v1.0 and Loop v1.0 to domain projections | §17 | Both are now part of the stack | — |
| 9 | Changelog added at top | This section | Versioning track | — |
| 10 | Version history updated | Document Status | — | — |

**What did not change:** Every mechanism from v7.1. The master equation, the curvature equation, the precision integration, the motor encoding layer, the social projection, and the empirical anchors are unchanged. v7.2 is additive convergence.

---

## Abstract

The brain is an energy budget allocation system operating on priors. This paper proposes a unified geometric framework — the Manifold Schema — in which the operational capacity of the nervous system is formally determined by the geometry of a neural manifold shaped by oscillatory amplitude, precision, and curvature, all driven by breathing mechanics. The central claim is that these geometric variables — measurable via standard HRV instrumentation — constitute the physical substrate from which all cognitive, emotional, perceptual, and social phenomena emerge. No new variables are introduced. No new instrumentation is required.

The framework formalizes the causal chain from breath to consciousness in a single master equation, anchors every variable in existing empirical literature across independent research programs, and generates falsifiable predictions at the individual, perceptual, and social scales. Critically, the perceptual confirmation is cross-domain: every major sensory system — visual, auditory, semantic, interoceptive, social, motor, and mnemonic — degrades under load in the same geometric pattern, drawn from independent literatures that were not designed to test this framework. The convergence is the evidence.

The framework extends structurally to the social scale. A society allocating finite resources under compounding load exhibits the same collapse geometry as an individual nervous system: precision degrades, the prediction window narrows, outer regions lose access first, and the system retreats to survival geometry. The historical pattern of this collapse is already in the data. The framework is the map that reads it.

The geometry is stateful, not fixed. Every configuration described in this framework is one breath away from a different configuration. What is trainable is not a consolation — it is the entire point.

The framework additionally identifies the motor encoding layer as the substrate below the prior loop. Manifold distortion is not randomly distributed — it is topographically determined by the interoceptive reporting of cached movement patterns. What the body has learned to reach sets the topology of what the mind can access. Blank zones in the motor map are experienced as cognitive and emotional limits — not because the capacity is absent, but because the interoceptive signal was never generated. This has a direct consequence: the entry point for geometry change is movement, not narrative. The body leads. The geometry follows. The cognition emerges.

---

## 0. What the Manifold Is

A manifold is a geometric object — a surface that can be locally flat or curved, wide or narrow, and whose shape determines what can be reached across it.

In this framework, the neural manifold is the state space of the nervous system. Every cognitive, emotional, and perceptual operation the brain performs occupies a position in that space. The geometry of the space — how flat or curved it is, how wide or narrow its integration radius — determines what operations are accessible at any given moment.

**This is not a metaphor.** Neural manifolds are measured objects. Neuroscience has known since at least 2006 that population-level neural activity does not explore all possible states equally — it moves along low-dimensional surfaces embedded in high-dimensional state space. The shape of those surfaces constrains what the system can do. This framework formalizes what drives the shape.

The shape is driven by one thing: the oscillatory budget.

The breath generates a rhythmic oscillatory signal. That signal funds all cognitive operations. When the signal is stable and wide-ranging — high amplitude, low jitter, phase-locked during exhalation — the manifold is flat. Flat geometry means long geodesics: the system can reach distant states efficiently. When the signal destabilises — amplitude narrows, jitter rises, phase-locking breaks — the manifold curves. Curved geometry means short geodesics: the system is trapped near its current state and cannot efficiently reach anything distant.

**Curvature is not a metaphor for stress.** It is the geometric consequence of oscillatory instability. It is measurable via HRV. It determines, mathematically, how far the system's predictions can propagate.

Three things follow from this:

1. **Every cognitive, emotional, and perceptual phenomenon is a position on the manifold** — a configuration of the same geometric variables, not a separate mechanism requiring separate explanation.

2. **Collapse is always inward.** When the budget tightens and curvature rises, the system retreats toward its geometric center — survival geometry. This is a statement about manifold access cost under load, not an anatomical claim about brainstem circuits. Complex operations at the outer edge lose access first.

3. **Recovery is always radial expansion outward.** The geometry is stateful, not fixed. The breath is the lever. Change the oscillatory source and the manifold reshapes.

> **Note on "brainstem" and "survival geometry" throughout this document:** These terms are used as geometric shorthand for the manifold's lowest-cost accessible states under load — the configuration the system defaults to when curvature is high and outer regions have lost access. They are not anatomical claims about specific brainstem circuits, phylogenetic vagal hierarchies, or dorsal vagal shutdown. Wherever "brainstem center" or "survival geometry" appears, read it as: *the geometric center of the manifold, defined by access-cost gradient, not by neuroanatomy.*

The framework that follows is a formal description of this geometry: its variables, its causal structure, its empirical anchors, and its predictions.

---

## 1. The Ground State

**Salience — The Formal Definition**

$$S = C_s \cdot I^*$$

| Term | What It Means |
|---|---|
| $C_s$ | Usable bandwidth — how much processing capacity is currently available |
| $I^*$ | Interoceptive routing capacity — how well the system can read and direct its own geometry |
| $S$ | Salience — what the system can currently afford to process |

Salience is not a gate. It is the product of bandwidth and routing. The system does not decide what to permit — it processes what $S$ can afford, and anything that exceeds the threshold is displaced.

$$T_S = \frac{k}{S}$$

When $S$ is high, $T_S$ is low — more signals are affordable. When $S$ is low, $T_S$ rises — only high-priority signals reach the encoding layer. Signals below the threshold are suppressed, and their suppression adds to curvature via the containment cost term $\sum_i S_i \cdot C_i$.

Because $S$ is a product, it collapses from either direction independently:

| Failure Mode | What Happens | Result |
|---|---|---|
| $C_s \downarrow$ — bandwidth depleted | Budget is gone regardless of routing capacity | $S \downarrow$ — system cannot afford signals it could previously route |
| $I^* \downarrow$ — routing collapsed | Bandwidth is present but cannot be read or directed | $S \downarrow$ — system cannot route signals it could previously afford |

**The two input sources feeding $S$ are both routed through the same layer:**

| Source | Mechanism | What Drives It |
|---|---|---|
| Incoming sensory signal | External stimulus competes for $I^*$ allocation | Amplitude and novelty of the signal |
| Prior geometry | Encoded pattern reinstates its own $K_{enc}$ — prior-driven salience arrives before the stimulus | Curvature of the encoding, not content |

The routing layer does not distinguish between them. A prior reinstating its encoded geometry and a sensory signal arriving from the world both compete for $I^*$ through the same mechanism. Both generate gain in the region they route to. This is why the prior always wins when $I^*$ is low — it was already routing before the signal arrived.

**The salience map is therefore not reading reality. It is reporting what $S$ can afford, weighted by what $I^*$ is already allocated to.**

---

**Salience and the Oscillatory Source**

$S = C_s \cdot I^*$ has one upstream lever: breath.

$C_s$ is funded by oscillatory amplitude. $I^*$ routing capacity is freed by reducing competing load. Breath acts on both simultaneously — slow, deep exhalation raises $A_s^*$, which raises $C_s$, which raises $S$, which lowers $T_S$. Signals that were previously unaffordable become affordable. The threshold drops not because a gate was unlocked but because the product increased.

This is the complete mechanism. No permission was granted. No decision was made. The budget changed and the affordability threshold followed.

---

### 1b. Breath as Salience Override

$$S = C_s \cdot I^*$$

The salience mechanism described in Section 1 is not accessible to direct instruction. You cannot decide to find a stimulus less threatening. The prior reinstates its encoded geometry before conscious recognition occurs — the routing is already running before you arrive.

But $S$ has one lever: breath.

Breath changes $S$ from both terms simultaneously. Slow, deep exhalation raises $A_s^*$, which raises $C_s$. Routing $I^*$ to the breath geometry occupies the gain control loop — prior-driven salience loses routing capacity because $I^*$ is no longer available to amplify it. $S$ rises on the breath signal. $T_S$ drops. The prior does not need to be suppressed — it simply has no gain.

This is the complete mechanism of every breath-based intervention. Not relaxation. Not reframing. Routing attention to breath geometry holds $I^*$ on the breath signal long enough for prior-driven salience to starve of gain.

The sequence:

| Step | What Happens | Why It Matters |
|---|---|---|
| 1. Route $I^*$ to breath | Gain control loop runs on breath signal | Prior-driven salience loses routing capacity |
| 2. Hold the geometry | $C_s$ rises, $\sigma(A_s)$ drops, $R^*$ rises | Manifold flattens — $K_{enc}$ drops |
| 3. Signal reaches encoding layer | Previously gated signal arrives from flat geometry | Prior layer receives input it has not had before |
| 4. $\mathcal{U}$ writes from flat geometry | New prior does not carry old curvature forward | |
| 5. Routing recalibrates | Signal routed differently on next encounter | Topology has changed — not by decision, by geometry |

The intervention does not need to be labelled. The mechanism runs regardless — because it operates below the layer where understanding lives.

**Hold the breath geometry. Stop routing to the prior. The prior loses gain. The geometry stabilises. That is the complete sequence.**

---

### 1c. The Savant State — Capacity Without Overhead

When left-hemisphere injury produces savant-level ability, the standard account says inhibition was removed, releasing hidden capacity. But this frames it backwards.

The capacity was already there. The injury removed the overhead that was consuming it.

The left hemisphere's dominant routing generates suppression cost on signals outside its schema. Every suppressed signal adds to $K$ via $\sum_i S_i \cdot C_i$. The amplitude ceiling the system appears to operate at is not its actual ceiling — it is the ceiling minus the suppression overhead. The savant state is what remains when that overhead is removed.

This has one implication: everyone has the same capacity. What differs is how much suppression overhead is running.

$$\sum_i S_i \cdot C_i \downarrow \rightarrow K \downarrow \rightarrow A_s^* \uparrow \rightarrow R^* \uparrow \rightarrow W^* \uparrow$$

Both terms move simultaneously — amplitude rises to its actual ceiling and precision spikes because there is nothing left to suppress. The system is not in a special state. It is in its default state with the overhead removed.

| Entry Point | Mechanism | Reversibility |
|---|---|---|
| Acquired savant — injury | Structural removal of suppression source | Permanent — hardware changed |
| Breath-routed override | $I^*$ removed from suppression signal — overhead starves | Reversible but cumulative |
| Long-term practice | Suppression boundaries dissolved — flat geometry becomes resting state | Permanent — new topology cached as baseline |

The difference between the acquired savant and the trained practitioner is the entry point and the timescale. The geometry is identical. The capacity was never absent. The overhead was.

**The savant state is not exceptional. It is the system running at what it always was. The suppression was the anomaly.**

---

**A Note on Recall**

Memory recall operates by the same principle. A memory encoded under high $K$ carries that curvature forward — the geometry at encoding is stored with the content. Recalled under flat geometry, the same memory reconstructs differently: the boundary that was active at encoding is not active at recall. The stored pattern is unchanged. The manifold reading it has changed.

This is why breath-stabilized re-exposure produces durable change. The prior does not erase. It is re-encoded from flat geometry, and the new encoding competes with the old. See Section 6a for the full $\mathcal{U}$ mechanism.

---

### 1d. The Salience Spectrum: Flow and Collapse

$$S = C_s \cdot I^*$$

Salience has two directions. Everything follows from which way $I^*$ routes.

**Flow** is $I^*$ fully allocated to the external sensory channel. Phase-locking is precise. Gain maximises on one signal. Everything else drops below the noise floor. $\sigma(A_s)$ collapses — not because amplitude is low but because it is controlled. The full budget runs on one channel with no containment cost competing for it.

**Collapse** is $I^*$ routing to the internal autonomic map. Gain amplifies the alarm signal. The amplified signal routes more $I^*$ to the map. The map reads itself at rising amplitude. $\sigma(A_s)$ maxes — amplitude is still present but uncontrolled, spilling across the routing layer with no phase-locking to direct it. The loop tightens with each cycle.

The energy budget is the same in both states. What differs is phase-locking precision and where $I^*$ is routing.

| | **Flow** | **Collapse** |
|---|---|---|
| **$I^*$ routes to** | External sensory channel | Internal autonomic map |
| **Gain increases on** | Present signal | Alarm signal |
| **$A_s^*$** | ↑↑ | ↓↓ |
| **$\sigma(A_s)$** | ↓↓ minimal | ↑↑ maximal |
| **$R^*$** | ↑↑ | ↓↓ |
| **$W^*$** | ↑↑ | ↓↓ |
| **Containment cost** | $\rightarrow 0$ | Maximum |
| **Loop direction** | Self-releasing | Self-reinforcing |

**The Bifurcation Point**

Between the two poles sits one variable: where $I^*$ is currently routed.

When $K$ is low and $S$ is high, the external channel is affordable. $I^*$ routes outward. Phase-locking engages. The flow loop begins.

When $K$ is high and $S$ is low, the external channel costs more than the budget can afford. $I^*$ routes inward to the only available signal — the autonomic map. The map amplifies. The collapse loop begins.

Breath interrupts the collapse loop by routing $I^*$ back to breath geometry — the map loses gain, the external channel becomes affordable again, direction reverses.

| Phenomenon | $I^*$ Direction | Loop State | Signature |
|---|---|---|---|
| Flow | Fully external | Self-releasing | $\sigma(A_s) \downarrow\downarrow$, $R^* \uparrow\uparrow$, $W^* \uparrow\uparrow$ |
| Presence | Predominantly external | Stable open | $K$ low, containment minimal |
| Anxiety | Tilting internal | Mild tightening | $K$ rising, external losing |
| Rumination | Predominantly internal | Slow self-reinforcing | Map reading map at low amplitude |
| Panic | Fully internal | Rapid self-reinforcing | $\sigma(A_s)$ maxing, $W^* \downarrow\downarrow$ |
| Dissociation | Internal — map exhausted | Post-collapse | $C_s \rightarrow 0$, no signal left to route |
| Meltdown | Sensory overload tips internal | Rapid collapse | Sensory load saturates routing — map takes over |

**Flow is $I^*$ in the world. Panic is $I^*$ in the map. Phase-locking points the gate.**

*Phase-locking synchronizes the oscillatory signal with motor output so tightly that background interoceptive noise drops to near zero. Only the focused channel is above the noise floor.*

---

### 1e. Fear as Encoded Salience

Fear is not a response to the world. It is the prior routing $I^*$ to an encoded pattern — one that was written under high $K_{enc}$ with the gate already closed. When a matching signal arrives, the map recognises the pattern and reinstates the full encoding: gate direction, curvature, containment cost, $\sigma(A_s)$. The gain loop runs on the threat signal. The collapse loop begins. The fear is present before conscious recognition occurs.

The stimulus matched the pattern. The routing fired. The fear is the gain loop running on the map's own record — not on the current signal.

This is why:
- Fear persists after the threat is gone — the encoded pattern reinstates regardless of current conditions
- You can know something is not dangerous and still be afraid — the prior fires below the layer where knowledge operates
- Top-down intervention has limited reach — the routing is running before cognition is consulted

**Bottom-Up Control**

Someone with genuine bottom-up control of the oscillatory system encounters the same signal differently. The fear response is not suppressed or overridden — it is not generated, because the prior was encoded from flat geometry and carries no boundary forward. The pattern is recognised. The gain loop finds nothing to amplify. No alarm fires.

| Apparent Fearlessness | Mechanism | Sustainable |
|---|---|---|
| Suppression | Containment cost rising — $K$ accumulates | No |
| Dissociation | $I^* \downarrow$ — signal not processed | No |
| Courage | Fear present — cognitive override | Partially |
| **Bottom-up control** | **Prior encoded from flat geometry — boundary never written** | **Yes** |

A person operating without encoded fear boundaries is running the same hardware as everyone else — without the suppression overhead those boundaries impose. See Section 1c for the geometry of what that looks like at full capacity.

The entry point is not psychological. It is geometric: encode the prior from flat geometry and the boundary is never written. The routing finds nothing to amplify. See Section 6b for why the body leads this process, and Section 6a for the $\mathcal{U}$ mechanism that determines what geometry the prior carries forward.

---

## 2. The Master Equation

### 2a. Why the Equation Is Scalar

The neural manifold is multi-dimensional. Collapse is directional — it proceeds radially inward (Section 4), and different failure modes produce different functional profiles even at identical bandwidth levels. Two systems at the same $C_s$ can have completely inverted working capacity depending on *which* variables failed and *which* hemisphere's integration dropped first.

The master equation is scalar because it answers one specific question: **how much of the system's own usable bandwidth is currently accessible?** Directionality — which way the manifold is tilted, which variables have failed, what tasks remain available — lives in the companion descriptors (Section 2e). The scalar and the descriptors are not alternatives. They are complements. Neither is sufficient alone.

---

### 2b. The Master Equation

$$C_s = \left(
A_s^{*\,0.15} \cdot 
R^{*\,0.30} \cdot 
W^{*\,0.25} \cdot 
\Theta^{*\,0.15}
\right)^{\frac{1}{0.85}}
\cdot \frac{1}{1 + L^{*}}
$$

**All variables are normalized dimensionless ratios [0,1] relative to the individual's own baseline.**
$C_s$ is an intra-individual metric. It measures how much of *this system's own capacity* is accessible right now — not how that capacity compares to another system's baseline. Two people at $C_s = 0.7$ are each at 70% of their respective manifolds, which may represent very different absolute capacities.

> **Note on the normalization exponent:** The four oscillatory weights ($A_s^*$, $R^*$, $W^*$, $\Theta^*$) sum to 0.85, not 1.0. The remaining 0.15 is structurally claimed by the load term $\frac{1}{1+L^*}$, which operates outside the geometric mean as a drag penalty on whatever capacity the oscillatory geometry produces. The exponent $\frac{1}{0.85}$ normalizes the weighted geometric mean so that uniform fractional inputs map to the same fractional output — if all four variables are at 50% capacity, $C_s = 0.50$ before load is applied. Without this correction the equation systematically overstates partial-capacity states.

> **Note on $R^*$:** $R^*$ is the normalized form of precision $P = R/D_T$, where $R$ is sync duration and $D_T$ is timing distance. $R^*$ is formally defined as the timing-coherence ratio — see §5a for the complete formalism, two-factor pressure decomposition, and CO₂ tolerance window.

> **Note on provisional exponents:** The Cobb-Douglas exponents (0.15, 0.30, 0.25, 0.15) are provisional. They reflect the empirical collapse sequence (precision degrades first, window second, amplitude and integration third) but have not been formally calibrated. See §5a.12 for the collapse sequence and Central Reference §3.1 for the current formulation.

| Variable   | Definition                    | Physical Measurement                                     | What It Measures                                                                           |
| ---------- | ----------------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| $A_s^*$    | Oscillatory amplitude         | RMSSD / Baseline RMSSD                                   | The energy budget — how much oscillatory signal is available to fund cognitive operations  |
| $R^*$    | Precision — timing-coherence ratio | Phase-Locking Index / Baseline PLI | Signal clarity — whether oscillatory streams stay close (low $D_T$) and stay close for long periods (high $R$) — see §5a |
| $W^*$    | Window width                  | Cognitive flexibility composite / Baseline               | Accessible manifold range — how far predictions can propagate                              |
| $\Theta^*$ | Global integration efficiency | Phase-locking stability × ambiguity tolerance / Baseline | How well the system holds disparate signals together in the same processing window         |
| $I^*$      | Interoceptive selection       | Heartbeat detection accuracy / Baseline                  | The routing protocol — how well the system reads its own geometry and allocates the budget |
| $L^*$      | Allostatic load               | RMSSD depression / Max observed depression               | Total current draw on the budget — metabolic, social, and cognitive demand combined |

**Additional variables (registered from Central Reference v1.4):**

| Variable | Definition | Where used |
|---|---|---|
| $O_{pathway}$ | Oxygen pathway integrity — substrate constraint on gate condition | Gate condition (§5a.3, Central Reference §3.6) |
| $\Lambda$ | Loop activation indicator — $\Theta^* \cdot R^* \cdot \mathbb{1}[P_{eff} > P_{threshold}]$ | Intelligence equation, Loop v1.0 §0 |
| $n_{hops}$ | Inference hops available — $\lfloor W^* \cdot \rho_{scaffold} \rfloor$ | Intelligence equation, Loop v1.0 §0 |
| $\rho_{scaffold}$ | Scaffold density — density of long-range competitive connections (~0.30; Roy & Banerjee, 2026) | $n_{hops}$ derivation |
| $\delta_{hyst}$ | Collapse hysteresis — recovery delay after precision collapse | Precision §1.7, §5a.5 below |

**Zero new variables. Zero new measurements. Zero new ontology.**
Every measurement pathway is standard practice in RSA and HRV research.

> $I^*$ is not a component of $C_s$. It is the routing layer applied to $C_s$ — what happens to the bandwidth after it exists. $I^*$ appears in $S = C_s \cdot I^*$, not in the bandwidth equation. A system with low $I^*$ has its bandwidth intact but cannot direct it. See Section 13.

**Why $I^*$ is multiplicative:** Interoception is the routing protocol. A system that cannot read its own geometry cannot allocate its bandwidth, regardless of how large that bandwidth is. If $I^* \rightarrow 0$, $C_s \rightarrow 0$ — not because amplitude, precision, or window have failed, but because the system cannot direct what it has. This is the geometric account of FND and dissociation: capacity is present, routing has failed. $I^*$ is multiplicative for the same reason a router with no routing table produces zero throughput regardless of link bandwidth. See Section 13 for the full mechanism.

**Why $C_s$ uses a weighted geometric mean:** The product form punishes any deficit exponentially — a healthy system at 0.7 across all variables reads as near-collapse. The geometric mean preserves the "all variables matter" logic while allowing partial compensation. One strong variable can partially carry a weak one, which matches the physiology. $R^*$ carries the highest weight (0.30) because exhale precision is the earliest indicator of geometry degradation and the most direct mechanism of window collapse. See Section 5 for the CO₂ mechanism. $I^*$ is excluded from $C_s$ — it is the routing layer, not a bandwidth component. See Section 13.

---

### 2c. HRV as the Correct Proxy: Why Criticism Misses the Actual Mechanism

Before addressing methodological critiques, the mechanism needs to be stated plainly.

HRV reflects respiratory sinus arrhythmia (RSA) — heart rate accelerates on inhale and decelerates on exhale. This timing is not noise. It is the system matching cardiac output to when oxygenated blood is available from the lungs. High HRV means precise timing — maximum oxygen uptake efficiency per beat. Low HRV means timing drift — the heart is pumping when less oxygenated blood is available, which is finite resource waste. **HRV is the efficiency control signal for oxygen delivery under finite energy constraints.** That is not a proxy relationship. That is the mechanism.

This is why the criticism of HRV fails at the foundation: critics are measuring the fuel injector and ignoring the engine load.

#### The Missing Variable: Allostatic Load

HRV looks inconsistent because allostatic load ($L^*$) is absent from every model using it. Two individuals with identical HRV but different load profiles produce completely different outcomes:

| HRV | $L^*$ | Predicted $C_s$ | Interpretation |
| --- | --- | --- | --- |
| High | Low | High | Full capacity available |
| High | High | Moderate | Amplitude present, load consuming it |
| Low | Low | Moderate | Reduced amplitude, load not compounding |
| Low | High | Collapsed | Amplitude deficit plus load overhead |

When load is unmodeled, these four profiles collapse into two HRV values. The metric appears noisy. **The noise is not in HRV — it is in the missing denominator.**

#### The Temporal Sampling Error

The load problem is compounded by a sampling error. Most HRV studies measure once — or treat repeated measurements as replications of a static trait rather than samples of a dynamic trajectory. This is the wrong model entirely.

$L^*$ is not fixed. It accumulates across the day. The master equation predicts a time course:

$$C_s(t) = \left(A_s^{\ast 0.15} \cdot R^{\ast 0.30} \cdot W^{\ast 0.25} \cdot \Theta^{\ast 0.15}\right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + L^\ast(t)}$$

As $L^*(t)$ rises across the day, the denominator increases and $C_s$ drops — even if the oscillatory numerator holds steady. The same person will produce measurably different HRV at 7:00 AM and 6:00 PM, not because HRV is noisy but because the system is stateful.

| Time | Expected $L^*$ | Expected $C_s$ | HRV |
| --- | --- | --- | --- |
| Morning | Low | High | High |
| Midday | Accumulating | Moderate | Moderate |
| Evening | High | Reduced | Lower |

A morning-only measurement and an evening-only measurement of the same individual look like two different people. A study sampling across both without modeling $L^*(t)$ will produce apparent inconsistency. The field has interpreted this as metric noise. It is temporal signal — the range is the information.

**The minimum viable experiment was always morning vs evening.** That single addition would have revealed that HRV is stateful, not fixed — that the range across a day is a richer signal than any single measurement. The field did not run this experiment because it had no model predicting the trajectory. The Manifold Schema provides that model. The prediction is explicit: $C_s$ follows a declining trajectory across waking hours proportional to $L^*(t)$ accumulation, with recovery occurring during sleep as $L^*$ resets.

This is not a complex methodological failure. It does not require a new instrument, a new metric, or a new population. The minimum correction was a two-measurement design — morning and evening, same subjects, same protocol. The statefulness would have been immediately visible: the same person producing measurably different HRV across the same day, tracking load accumulation exactly as the master equation predicts. The field did not run this experiment because it had no model telling it the result would be meaningful. Without a model of statefulness, a second measurement looks like replication noise rather than trajectory signal. **The Manifold Schema provides that model. The prediction is now explicit. The experiment is trivial to run.**

#### What HRV Actually Measures

HRV captures the oscillatory source layer — the upstream input to the full causal chain:

$$\text{Breath} \rightarrow A_s^* \rightarrow \sigma(A_s) \rightarrow R^* \rightarrow K \rightarrow W^* \rightarrow \Theta^* \rightarrow C_s$$

- **Amplitude** ($A_s^*$) — oscillatory excursion range (RMSSD, time-domain metrics)
- **Precision** ($R^*$) — rhythm consistency across cycles (phase-locking, jitter)

Criticizing HRV for failing to predict outcomes without modeling load is like criticizing a thermometer for failing to predict boiling point without accounting for altitude. **The instrument is reading the right variable. The model is incomplete.**

#### Why Other Frameworks Took the Hit

Polyvagal Theory treated HRV as a direct index of discrete vagal states — categorical and hierarchical. When HRV failed to cleanly predict state transitions, the metric was blamed. But the framework had:

- No load variable
- No precision variable
- No geometric mechanism

HRV was forced to carry amplitude, precision, state category, and social engagement capacity simultaneously. It collapsed under the weight of missing structure.

The Manifold Schema avoids this error. HRV contributes to $A_s^*$ and $R^*$ estimates. Load is measured separately. Window and integration are estimated from behavioral and cognitive composites. No single metric carries the full model. HRV is one probe into one layer — exactly what it can reliably do.

#### On the Measurement Debate

The critique of HRV-based frameworks has been formally consolidated. Grossman (2023, *Biological Psychology*) argued that RSA provides "no or very limited information about any other vagal processes" beyond heart-rate timing. Grossman et al. (2026, *Clinical Neuropsychiatry*, 23(1):100–112) expanded this into a direct critique of Polyvagal Theory's empirical foundations. Porges responded directly in the same issue ("When a Critique Becomes Untenable," 23(1):113–128), and the debate remains live. The Manifold Schema takes no position on that dispute. It accepts Grossman's specific measurement limitation in full — and does not exceed it. HRV is used in this framework specifically as a proxy for $A_s^*$ and $R^*$. All remaining variables — $W^*$, $\Theta^*$, $L^*$ — are estimated through separate instruments. The critique applies to frameworks that overextend HRV beyond timing efficiency. The Schema does not overextend it.

#### Convergence Confirmation

Miller et al. (2026) describe a convergent electrophysiological framing: traveling wave dynamics organize cortex into low-dimensional, task-oriented geometry, and disruption of those dynamics produces cognitive collapse. This is structurally consistent with the Schema's curvature-driven constraints — their framework does not address breath, load, or the causal chain directly. The convergence is at the level of geometric description, not causal mechanism. The Manifold Schema provides the upstream driver their account leaves open:

- Reduced precision ($R^* \downarrow$)
- → Increased curvature ($K \uparrow$)
- → Narrowed window ($W^* \downarrow$)
- → Collapsed integration ($\Theta^* \downarrow$)
- → Reduced $C_s$

Their framework also lacks a load variable. The Manifold Schema provides it.

**HRV is not the wrong metric. The field is missing the denominator.**

---

### 2d. The Curvature Equation

$$K = k\left(\frac{1}{R^* + \epsilon}\right) + \sum_i S_i \cdot C_i$$

| Source | Mechanism |
|---|---|
| Precision loss — $\frac{1}{R^* + \epsilon}$ | Jitter rises, oscillatory signal fragments, manifold curves around the instability. $\epsilon$ is a small physiological floor — the system maintains residual precision at its geometric center. Without $\epsilon$, the equation produces infinite curvature as $R^* \rightarrow 0$, which is a mathematical artifact. Metabolic crisis produces system shutdown before infinite curvature occurs. |
| Containment cost — $\sum_i S_i \cdot C_i$ | Each suppressed signal adds to curvature independently of oscillatory amplitude |

**Transfer Functions — $K$ to Downstream Variables**

$K$ is not a variable in the master equation — it is the mechanism through which $R^*$ operates on $W^*$ and $\Theta^*$. The relationships are now formally defined:

$$W^* = \frac{1}{1 + \alpha K}$$

$$\Theta^* = \frac{1}{1 + \beta K}$$

| Term | Meaning |
|---|---|
| $\alpha$ | Calibration constant — how steeply window narrows per unit of curvature. Empirically measurable, individually variable |
| $\beta$ | Calibration constant — how steeply integration efficiency degrades per unit of curvature. Separate from $\alpha$ — $W^*$ and $\Theta^*$ do not necessarily degrade at the same rate |

> **Note on calibration constants:** The transfer parameters $\alpha$, $\beta$, and $\gamma$ are not universal constants; they are individual transfer functions whose baseline vectors are parameterized by genetic substrate. Interoceptive gain ($\alpha$) is anchored by dopamine clearance and receptor profiles, allostatic decay rate ($\beta$) by HPA axis resilience and glucocorticoid sensitivity, and structural efficiency ($\gamma$) by muscle fiber distribution and connective tissue architecture. Under identical external load ($L^*$), two individuals will follow distinct curvature trajectories ($C_s$) because their underlying parameter vectors differ. Empirical calibration therefore requires individual system identification rather than population-level averaging.

**Note on the $J(C) \to \eta$ pathway.** Chemoreflex jitter $J(C)$ — the timing noise injected above $C_{high}(L^*)$ (see §5a.2) — is not identical to the containment cost term $\sum_i S_i \cdot C_i$. It operates through a different channel: it raises the effective noise floor $\eta$ used in the resolution floor equation $\delta_{min} = \eta/(A_s^* \cdot I^*)$. The relationship is:

$$\eta_{effective} = \eta_{baseline} + f(J(C))$$

Where $f$ is currently assumed linear for simplicity: $\eta_{effective} = \eta_{baseline} + J(C)$. When CO₂ exceeds $C_{high}(L^*)$, the effective $\eta$ rises, which raises $\delta_{min}$ on every channel simultaneously. This is why CO₂ over-tolerance produces global resolution collapse — not localized to specific channels, but system-wide.

The functional form of $f$ is an open empirical question (see Precision v3.4 §1.10). For the purposes of the framework, the linear assumption is sufficient to predict the qualitative behavior: rising $J(C)$ → rising $\eta_{effective}$ → rising $\delta_{min}$ → resolution collapse.

At $K = 0$: $W^* = 1.0$, $\Theta^* = 1.0$ — no curvature, full window and integration.
As $K \rightarrow \infty$: both approach zero asymptotically — the system never fully shuts off until metabolic crisis.

**Consequence:** $W^*$ and $\Theta^*$ are derived variables, not independent inputs. The truly independent inputs to the system are $A_s^*$, $R^*$, $L^*$, and $\sum_i S_i \cdot C_i$. Everything else is downstream.

$K$ is not a variable in the master equation — it is the mechanism through which $R^*$ and $L^*$ operate. As $K$ rises, $W^*$ narrows and $\Theta^*$ degrades.

---

### 2e. Companion Descriptors

The scalar $C_s$ answers *how much*. The companion descriptors answer *which way* and *what for*.

**$\lambda$ — Lateralization State**

$$\lambda \in \{R\text{-dominant},\ L\text{-dominant},\ \text{bilateral},\ R\text{-collapsed},\ L\text{-collapsed},\ \text{bridge-failed}\}$$

$\lambda$ is inferred from which hemisphere's $\Theta^*$ degrades first under load. It is not a permanent trait — it is the current configuration of the manifold's tilt. See Section 14 for working state profiles.

**$F(\Xi)$ — Collapse Mode Vector**

$$F(\Xi) = (f_{R^\ast},\ f_{W^\ast},\ f_{\Theta^\ast},\ f_{I^\ast},\ f_{L^\ast},\ f_\lambda)$$

| Component | What It Measures | Range | Meaning |
|-----------|-----------------|-------|---------|
| $f_{R^*}$ | Precision failure — jitter, signal fragmentation | 0–1 | 0 = intact, 1 = collapsed |
| $f_{W^*}$ | Window narrowing — loss of range | 0–1 | 0 = intact, 1 = collapsed |
| $f_{\Theta^*}$ | Integration failure — loss of coherence | 0–1 | 0 = intact, 1 = collapsed |
| $f_{I^*}$ | Interoceptive misrouting — loss of self-routing | 0–1 | 0 = intact, 1 = collapsed |
| $f_{L^*}$ | Load saturation — budget overwhelmed | 0–1 | 0 = intact, 1 = collapsed |
| $f_\lambda$ | Lateralization lock — tilt fixed under load | 0–1 | 0 = fluid, 1 = locked |

Two systems at identical $C_s$ with different $F(\Xi)$ profiles have completely different functional capacity. A precision failure ($f_{R^*}$ high) looks nothing like a routing failure ($f_{I^*}$ high) at the behavioral level — even if the scalar bandwidth is the same.

**$C_s^{usable}(T)$ — Task-Relative Usable Bandwidth**

$$C_s^{usable}(T) \propto A_s^* \cdot R_{stable}^* \cdot W_T^* \cdot \Theta_T^*$$

Where $W_T^*$ is the window width required for task $T$ and $\Theta_T^*$ is the integration requirement for task $T$. A system may have substantial $C_s$ while having near-zero $C_s^{usable}$ for a specific task that demands the failed dimension. This is why a person in a precision-failure state can still perform emotionally attuned social tasks while being unable to execute structured logical work — the available bandwidth is real, but it is not in the right geometry for the task.

---

## 3. The Causal Chain

$$\text{Breath} \rightarrow A_s^* \rightarrow \sigma(A_s) \rightarrow R^* \rightarrow K \rightarrow W^* \rightarrow \Theta^* \rightarrow C_s$$

This is not a descriptive chain. Each arrow is a mechanism. Three mechanisms make the chain operational rather than correlational:

| Mechanism | What It Does | Where It Operates In The Chain | Section |
|---|---|---|---|
| **IRQ routing** — $I^*$ | Routes gain to signals — determines which signals the chain runs on | $R^* \rightarrow K$ — precision sets the noise floor, $I^*$ sets the gain | §13 |
| **Prior update rate** — $\mathcal{U}$ | Writes current geometry into the prior layer — determines what the next encounter costs | $C_s \rightarrow$ future $K$ — the output of the chain becomes the input of the next | §6a |
| **Motor encoding** — topology mapping | The body is the prior substrate — movement history is the manifold | Prior layer → future $K$ — blank motor zones are blank geometry | §6b |

Without these three mechanisms the chain describes what happens. With them it explains why the geometry behaves the way it does — and why breath at the bottom of the chain reaches all the way up to prior topology.

| Breath Phase | $\sigma(A_s)$ | $R^*$ | $K$ | $W^*$ | $\Theta^*$ | Budget State |
|---|---|---|---|---|---|---|
| Inhalation | ↑ | ↓ | ↑ | ↓ | ↓ | Variation, exploration, intake |
| Exhalation | ↓ | ↑ | ↓ | ↑ | ↑ | Precision, access, integration |
| Suspension | →0 | →Max | →0 | →Max | →Max | Peak access — phase-locked state |
| Pause | Stable | Stable | Stable | Stable | Stable | Consolidation |

$R^*$ rises during exhalation via phase-locking of vagal efferent drive — not via reduction in amplitude. When phase-locking is maximal during suspension, background interoceptive noise drops to near zero. Only the focused channel is above the noise floor. This is the geometric basis of the flow state. See Section 1d.

---

**Two Thresholds**

The chain does not become self-sustaining at all levels of $R^*$. Two thresholds determine whether the loop engages.

**Precision Floor — $R^*_{min}$**

Below $R^*_{min}$, interoceptive signal cannot separate from background noise. The map stays coarse. The prior layer cannot update from what it cannot distinguish. Crossing $R^*_{min}$ is a phase transition — when precision breaks above the noise floor, signals that were noise become readable earlier in the trajectory. The system detects curvature increase before it becomes a crisis. This is the large initial gain observed in breathwork and conditioning studies.

**Amplitude Ceiling — $A^*_{s,max}$**

The upper limit is set by CO₂ tolerance — how wide the oscillatory source can get before the system runs out of amplitude range. Gains below $R^*_{min}$ are signal-cleaning gains. Gains above $R^*_{min}$ are map-refinement gains. Expanding $A^*_{s,max}$ requires CO₂ tolerance training and operates on a longer timescale — and requires the system to already be above $R^*_{min}$ to register the expansion.

| Phase | Work | Gain Type |
|---|---|---|
| Below $R^*_{min}$ | Signal cleaning — breath, precision training | Phase transition — large, rapid |
| Above $R^*_{min}$ | Map refinement — prior updating | Continuous, moderate |
| Expanding $A^*_{s,max}$ | CO₂ tolerance, load progression | Slow, requires clean signal |

**$L^*$ — The Persistent Denominator**

$L^*$ is not a step in the chain — it is pressure on every step simultaneously. It determines the effective starting position: what $A_s^*$ is actually available after load is subtracted, what $R^*$ floor the system operates from before breath acts on it. Managing $L^*$ is upstream of breath training in terms of baseline geometry.

---

## 4. The Radial Structure

The manifold radiates outward from its oscillatory source — the geometric center defined by access cost under load.

| Distance From Center | Region | Access Cost | Lost First Under Load |
|---|---|---|---|
| Geometric center | Survival geometry (lowest access cost) | Zero — always funded | Never |
| Near | Limbic | Low | Last |
| Mid | Cortical, language | Moderate | Middle |
| Far | Prefrontal, bilateral | High | First |

This describes energetic priority, not emotional dominance. Survival geometry is the default. Everything else is built outward from it.

**On Individual Topology**

The distances above describe the default sequence in which regions lose access as curvature rises. The topology of "near" and "far" for any individual is not universal — it is personally constructed from motor encoding history and maintained in real time by interoceptive reporting.

Two people under identical external load will lose access in different regions first — not because their hardware differs, but because their motor vocabulary differs. See Section 6b for the full mechanism.

---

## 5. The CO₂ Mechanism: How Breath Sets the Geometry

$$\text{CO}_2 \rightarrow \text{phase-locking} \rightarrow \sigma(A_s) \rightarrow R^* \rightarrow K \rightarrow W^*$$

| Stage | Physiological Event | Framework Variable | Direction |
|---|---|---|---|
| CO₂ tolerance high | Wide oscillatory amplitude range available | $A_s^*$ range | ↑ |
| Exhalation phase-locked | Amplitude distributed evenly across cycles | $\sigma(A_s)$ | ↓ |
| Even distribution | Low jitter | $R^*$ | ↑ |
| High precision | Low allocation cost per prediction | $K$ | ↓ |
| Low curvature | Long geodesics, wide integration radius | $W^*$ | ↑ |

CO₂ is not a new variable. It is the physiological mechanism that determines amplitude range and phase-locking stability — the input conditions for every step above it in the chain.

**Why depth matters more than rate:** Breath depth moves CO₂. Rate does not. A fast shallow breath depletes CO₂ tolerance and collapses the chain from the top. A slow deep exhale stabilises phase-locking and widens the window. Each link in the chain above is already confirmed by independent RSA, HRV, breath-hold, and hyperventilation literatures. See Section 8 for anchors.

The geometry is stateful, not static. The system is always one breath away from a different configuration.

---

## 5a. Precision: The Formal Definition of $R^*$

Section 5 established how breath produces the conditions for precision — CO₂ tolerance, phase-locking, and amplitude stability. This section defines what precision *is*: the timing-coherence ratio that these conditions produce, and the formal substrate of the $R^*$ variable in the master equation.

---

### 5a.1 Precision as a Timing-Coherence Ratio

Let two oscillatory streams — such as respiration and heart rate, or inter-hemispheric EEG phase — have phase difference:

$$\Delta \phi(t)$$

Define **timing distance** as the average absolute phase difference over a measurement window:

$$D_T = \mathbb{E}_{t \in T} \big[|\Delta \phi(t)|\big]$$

Define **sync duration** as the proportion of time spent within a small phase band $\epsilon$:

$$R = \frac{T_{\text{in}}}{T_{\text{total}}}$$

Where $T_{\text{in}}$ is the time the phase difference remains below threshold $\epsilon$.

**Precision is the ratio of sync duration to timing distance:**

$$P = \frac{R}{D_T}$$

**Interpretation:** A system achieves high precision when two streams stay close together (low $D_T$) and stay close for long periods (high $R$). A system with low precision may have streams that are close briefly (low $D_T$, low $R$) or far apart consistently (high $D_T$, high $R$). Both produce low $P$.

**$R^*$ is the normalized form of this timing-coherence ratio, relative to the individual's baseline:**

$$R^* = \frac{P}{P_{\text{baseline}}} = \frac{R/D_T}{(R/D_T)_{\text{baseline}}}$$

**Note on $P$ vs $P_{eff}$.** $P$ is the raw timing-coherence ratio. The gate condition uses the effective precision:

$$P_{eff} = P \cdot O_{pathway} \cdot U_C$$

Where $O_{pathway}$ is oxygen pathway integrity and $U_C$ is CO₂ uniformity. The full distinction is specified in Precision v3.4 §1.1 and §1.10. In MS, $R^*$ is the normalized raw $P$; $P_{eff}$ is the gate-condition variable.

**Operational Measurement:** The Phase Locking Value (PLV) is the operational measurement of this ratio. PLV ranges from 0 (no synchronization) to 1 (perfect synchronization), calculated as:

$$\text{PLV} = \left|\frac{1}{N}\sum_{n=1}^{N} \exp(i \times (\phi_{\text{resp}}(n) - \phi_{\text{hr}}(n)))\right|$$

This is the mathematical measure of how close two oscillatory streams stay ($D_T$) and how consistently they maintain that proximity ($R$) — precisely the ratio defined above (Pratap et al., 2026). The streams being measured can be any pair of oscillatory signals relevant to the system state.

---

### 5a.2 The CO₂ Tolerance Window and Chemoreflex Jitter

Precision increases only while CO₂ remains within the individual tolerance band:

$$C_{\text{low}} < C < C_{\text{high}}(L^*)$$

Where:
- $C_{\text{low}}$ is the minimum CO₂ needed to raise HRV, reduce jitter, and allow precision to rise
- $C_{\text{high}}(L^*)$ is the maximum CO₂ the system can sustain before chemoreflex activation injects jitter, given current allostatic load

**Above $C_{\text{high}}(L^*)$:** Chemoreflex activation produces involuntary diaphragm and intercostal spasms that inject timing noise into the oscillatory loop. This jitter is modeled as:

$$J(C) = \begin{cases}
0 & C \le C_{\text{high}}(L^*) \\
\kappa (C - C_{\text{high}}(L^*))^2 & C > C_{\text{high}}(L^*)
\end{cases}$$

Where $\kappa$ is the chemoreflex jitter gain. Jitter grows quadratically once tolerance is exceeded.

**Load-compressed ceiling.** The CO₂ tolerance window is not fixed. As allostatic load accumulates, the ceiling drops:

$$C_{high}(L^*) = C_{high}^0 - \gamma L^*$$

where $C_{high}^0$ is baseline tolerance and $\gamma$ is the load-compression coefficient. This means the same absolute CO₂ level produces chemoreflex jitter at lower values when load is high. The compression mechanism is what the Control Pause measures clinically: as load rises, CP drops.

**Below $C_{\text{low}}$:** HRV is insufficient to sustain coherence. Precision remains low regardless of effort.

**Interpretation:** This completes the mechanism asserted in Section 5. CO₂ does not monotonically improve precision — it has a tolerance window. The chemoreflex jitter term explains why excessive CO₂ collapses rather than improves the geometry, and why breath-hold at the right moment produces precision lock while over-extension produces spasms and fragmentation.

**Operational Measurement:** Capnometry (end-tidal CO₂) provides continuous CO₂ measurement. Jitter is approximated using EEG phase jitter, HRV beat-to-beat variability (RMSSD), and respiration–ECG phase slip.

**Cross-reference:** Precision v3.4 §1.4 specifies the full CO₂ tolerance window with load compression. Allostatic Load v2.1 §5d specifies the Control Pause protocol.

---

### 5a.3 The Two-Factor Pressure Correction

Section 5 treats "pressure" as a single variable. This is insufficient. Pressure must be split into two components with opposite effects on precision:

| Component | Symbol | Source | Effect on Precision |
|-----------|--------|--------|---------------------|
| **Mechanical pressure** | $\Pi_{\text{mech}}$ | Breath-hold, closed-loop pressure, thoracic pressure, baroreflex coherence | **Beneficial** — reduces timing distance, extends sync duration |
| **Cognitive/metabolic pressure** | $\Pi_{\text{cog}}$ | Load, sympathetic activation, cognitive demand, allostatic load | **Harmful** — increases timing distance, reduces sync duration |

**Total pressure is the sum:**

$$\Pi = \Pi_{\text{mech}} + \Pi_{\text{cog}}$$

But they operate with opposite signs in the precision equations.

**Mechanical Pressure Onset Condition:** Mechanical pressure becomes beneficial when the respiratory loop is closed (end-exhalation breath-hold) and thoracic motion drops below threshold. This condition enforces bilateral symmetry and reduces timing drift.

**Note on $\Pi_{cog}$ vs. $L^*$:** These are distinct. $\Pi_{cog}$ is *instantaneous* cognitive pressure — the current draw on the budget. $L^*$ is *cumulative* allostatic load — the integral of $\Pi_{cog}$ over time minus recovery:

$$L^*(t) = \int_0^t \Pi_{cog}(\tau) \, d\tau - \text{recovery}(t)$$

Both appear in the framework. $\Pi_{cog}$ enters the precision equation directly (through $D_T$ and $R$). $L^*$ enters the master equation as the denominator drag and compresses $C_{high}(L^*)$. This prevents double-counting: acute load affects precision; chronic load affects bandwidth and the CO₂ ceiling.

**Operational Measurement:** Mechanical pressure is approximated using thoracic pressure amplitude (respiration belt), baroreflex phase coherence (ECG–BP coupling), and intracranial pulse pressure proxies (PPG). Cognitive/metabolic pressure is approximated using sympathetic markers (LF/HF ratio), pupillometry (task-evoked dilation), and performance-capacity mismatch (error rate under load).

**Interpretation:** This resolves a latent ambiguity in the Manifold Schema's curvature equation — $K$ has containment cost $\sum_i S_i \cdot C_i$ but no formal distinction between the type of pressure driving curvature up. The two-factor split gives that distinction formal grounding. Breath-hold pressure (mechanical) improves precision by enforcing bilateral symmetry and phase coherence. Cognitive load pressure (metabolic) degrades precision by injecting noise and increasing jitter. The same word — "pressure" — carries opposite meanings depending on its source.

**The complete precision equation with two-factor pressure:**

$$P(C, \Pi_{\text{mech}}, \Pi_{\text{cog}}) = \frac{R}{D_T}$$

Where timing distance with both pressure components and jitter is:

$$D_T = \frac{k_2}{H(C)} \cdot \frac{1 + \lambda_c \Pi_{\text{cog}}}{1 - \lambda_m \Pi_{\text{mech}}} + J(C)$$

And sync duration with both pressure components and jitter is:

$$R = k_3 H(C) \cdot (1 + \mu_m \Pi_{\text{mech}}) \cdot e^{-\mu_c \Pi_{\text{cog}}} \cdot e^{-\nu J(C)}$$

With CO₂ uniformity applied at the gate condition:

$$P_{eff} = P \cdot O_{pathway} \cdot U_C, \quad U_C = \frac{1}{\text{Var}_i[C_i] + \epsilon}$$

**Cross-reference:** Precision v3.4 §1.5 specifies the full two-factor pressure decomposition. Central Reference §3.3 specifies the full precision equations.

---

### 5a.4 CO₂ Uniformity and Dynamics

CO₂ uniformity is the inverse variance of CO₂ across the system:

$$U_C = \frac{1}{\text{Var}_i[C_i] + \epsilon}$$

**Interpretation:** Precision is maximized when CO₂ is high AND uniformly distributed. High CO₂ with uneven distribution produces high variance, reducing precision. This explains why breath-hold at the right moment improves precision (uniformity achieved) but collapses when CO₂ becomes unevenly distributed.

**Uniformity Dynamics:** CO₂ uniformity evolves over time according to:

$$\frac{dU_C}{dt} = -\rho \cdot \text{Var}_i[C_i(t)]$$

Where $\rho$ is the equalization rate. Uniformity increases during closed-loop breath-holds and decreases when CO₂ distribution becomes uneven.

**Load-driven variance:** Allostatic load increases the variance term directly:

$$\text{Var}_i[C_i(t)] \propto L^*$$

This means load degrades uniformity through the same pathway it compresses $C_{high}(L^*)$ — the CO₂ regulatory system loses precision as debt accumulates. The composite uniformity expression is:

$$U_C(L^*) = \frac{1}{1 + \nu L^*}$$

where $\nu$ is the uniformity-degradation coefficient.

**Operational Measurement:** CO₂ uniformity is approximated using end-tidal CO₂ (capnometry), multi-site PPG variance, and respiration–HRV coupling stability.

**Cross-reference:** Precision v3.4 §1.6 specifies the full uniformity dynamics. Central Reference §3.3 specifies the composite uniformity expression.

---

### 5a.5 Collapse Hysteresis

After precision collapse, recovery is delayed due to residual jitter and sympathetic activation. This is modeled as:

$$P_{\text{recover}} = P(t) - \delta_{\text{hyst}}$$

Where $\delta_{\text{hyst}}$ is the hysteresis penalty. This explains post-collapse fog and delayed clarity.

**Variable registration.** $\delta_{\text{hyst}}$ is registered in §2b as a framework variable. It appears in the precision equations (§5a.3) and in the master equation's recovery dynamics (not as a term, but as a delay on the $P$ recovery path).

**Hysteresis Decay:** The hysteresis penalty decays exponentially:

$$\frac{d\delta_{\text{hyst}}}{dt} = -\sigma \delta_{\text{hyst}}$$

**Interpretation:** The system does not recover from collapse at the same rate it entered it. Once jitter is injected and coherence is lost, residual sympathetic activation and lingering phase noise prevent immediate return to precision lock. Recovery requires sustained conditions — not just a brief return to the precision window.

This is the formal substrate for why Section 7 (Felt Geometry) describes the collapse states as sticky — the geometry doesn't bounce back symmetrically. The hysteresis penalty captures that asymmetry.

**Cross-reference:** Precision v3.4 §1.7 specifies the full hysteresis dynamics. Central Reference §3.3 registers the variable.

---

### 5a.6 Resonance Breathing and Cross-Frequency Coupling

**Resonance breathing** occurs when the respiratory oscillator and the cardiac baroreflex oscillator phase-lock at ~0.1 Hz (≈6 breaths/min). This frequency matching reduces timing distance and increases sync duration independent of CO₂.

Formally:

$$\Pi_{\text{mech}} \propto \text{PLV}(f_{\text{resp}}, f_{\text{baro}})$$

When $f_{\text{resp}} = f_{\text{baro}}$, drift drops, jitter remains low, and precision rises without entering the CO₂ tolerance window. This produces stable clarity and flow without spasms or collapse.

**Cross-frequency coupling (CFC)** extends the precision model to interactions across multiple frequency bands:
- Respiration–HRV coupling (0.1 Hz)
- Alpha–theta coupling during meditation
- Theta–HRV coupling during breath-hold
- Gamma–cardiac phase coupling during flow states

**Interpretation:** Resonance breathing is a third precision mechanism — distinct from CO₂-driven precision and breath-hold precision lock. It operates through frequency entrainment of the respiratory and cardiac oscillators, producing sustained precision at moderate CO₂ levels without the risk of exceeding tolerance. CFC makes the precision model compatible with multi-band EEG and HRV phenomena.

**Operational Measurement:** Resonance is measured as phase-locking between respiration and baroreflex at ~0.1 Hz. CFC is measured using phase-amplitude coupling (PAC), phase-phase coupling (PPC), or n:m phase locking between oscillatory bands.

**Cross-reference:** Precision v3.4 §1.8 specifies the full resonance breathing mechanism. Precision v3.4 §1.2 specifies the CFC extension.

---

### 5a.7 Individual Variability in CO₂ Tolerance

The CO₂ tolerance parameters $C_{\text{low}}$ and $C_{\text{high}}$ are individual-specific and trainable. Factors that shift the tolerance window include:

| Factor | Effect on Tolerance |
|--------|---------------------|
| Fitness/athletic training | Increases tolerance (higher $C_{\text{high}}$) |
| Anxiety | Decreases tolerance (lower $C_{\text{high}}$) |
| Altitude | Shifts tolerance (adaptation over days) |
| Hydration | Affects tolerance (dehydration lowers) |
| Sleep | Affects tolerance (poor sleep lowers) |
| Breathwork practice | Increases tolerance (trainable) |

Precision peaks occur at different CO₂ levels across individuals. The tolerance window is not fixed — it is a dynamic state variable that shifts with training and condition. This accounts for why interventions that work for one individual may fail for another: the tolerance window and training history differ.

**Load compression.** The ceiling $C_{high}$ compresses with allostatic load (see §5a.2). This means the same person's tolerance window narrows as load accumulates. Tracking CP across time is tracking $L^*$ through the CO₂ pathway.

**Cross-reference:** Precision v3.4 §1.3 specifies the full individual variability treatment. Allostatic Load v2.1 §5d specifies the CP measurement protocol.

---

### 5a.8 Variable Mapping — Precision Doc to Manifold Schema

| Precision Doc | Manifold Schema | What It Captures |
|---------------|-----------------|------------------|
| Timing distance $D_T$ | Phase coherence deficit | How far apart oscillatory streams are |
| Sync duration $R$ | Phase-locking stability | How long streams stay together |
| Precision $P$ | $R^*$ | The ratio of sync duration to timing distance |
| Effective precision $P_{eff}$ | Gate condition input | $P_{eff} = P \cdot O_{pathway} \cdot U_C$ |
| Oxygen pathway $O_{pathway}$ | Substrate constraint | Metabolic viability of integration pathway |
| Jitter $J(C)$ | $\sigma(A_s)$ (amplitude jitter) | Noise floor from chemoreflex |
| Mechanical pressure $\Pi_{\text{mech}}$ | Breath coherence | Symmetry enforcer |
| Cognitive pressure $\Pi_{\text{cog}}$ | Containment cost | Harmful pressure — acute load degrading precision |
| Collapse hysteresis $\delta_{\text{hyst}}$ | Recovery cost | Asymmetric recovery |
| CFC (multi-band) | $\Theta^*$ integration | Cross-frequency coupling |
| $C_{high}(L^*)$ | — | Load-compressed CO₂ ceiling |
| REQT | — | Qualification threshold |
| Collapse sequence | — | Topologically forced failure order |

**The precision ratio $P$ is the operational definition of $R^*$ in the master equation.** When $P$ is high, $R^*$ is high, curvature drops, and the manifold flattens. When $P$ is low, $R^*$ is low, curvature rises, and the manifold curves.

**For the complete mathematical formalism — including temporal dynamics, motor gain equations, cross-frequency coupling, and full falsifiable predictions — see *Precision, Timing, and the Oscillatory Source: Complete Formalism* v3.4 (Robinson, 2026). DOI: 10.5281/zenodo.22179675**

---

### 5a.9 The Salience-Triggered Loop Access

Baseline CO₂ tolerance determines whether the loop is available at rest or only under salience-induced breath interruption.

**The mechanism.** Salience halts breathing → CO₂ rises → cerebral blood flow increases → jitter drops → $R^*$ rises → $K$ drops → $W^*$ widens → orthogonality restored → $\Theta^*$ rises → loop becomes available.

**The individual difference.**

| Profile | Breath pattern | Baseline CO₂ | Baseline $R^*$ | Loop access |
|---|---|---|---|---|
| Chronic hypocapnic | Rapid, shallow, chest | Low | Low | Requires salience trigger |
| Stable CO₂ | Slow, diaphragmatic | Within window | High | Available at baseline |

**The prediction.** Baseline CO₂ tolerance predicts whether an individual requires salience-induced breath interruption to enter deep inference. See PREDICT-PREC-10.

**The clinical implication.** CO₂ tolerance training raises baseline $R^*$, lowering the salience threshold required to access the loop. This is a trainable substrate parameter, not a fixed trait.

**The framework connection.** The loop (Path A) is expensive. Path B (prior retrieval) is always available and always cheaper. The system defaults to Path B under load unless precision is high enough to open the gate. For chronic hypocapnic individuals, precision is rarely high enough at baseline — the gate stays closed until a salience event forces a breath interruption that temporarily restores CO₂. For stable-CO₂ individuals, the gate is available at baseline. This is not a difference in intelligence — it is a difference in substrate parameters.

**Cross-reference:** Central Reference §5 specifies the Path A/B branch condition. Central Reference §6 specifies the four qualification profiles. Precision v3.4 §1.4b specifies the full mechanism.

---

### 5a.10 Independent Empirical Confirmation of $K$ — Xue et al. (2026)

Xue et al. (2026) demonstrated that under task uncertainty, the neural representations of task-relevant and task-irrelevant features become non-orthogonal in V1. Cross-decoding (p = 0.006, p = 0.036), noise correlation (p < 0.0001), and microstimulation (p = 0.009) all confirm the entanglement.

**This is the $K$ mechanism measured directly.** Under load, representations that were orthogonal become entangled — the manifold curves, and the effective dimensionality drops. The paper calls it "feature interference." This framework calls it "$K$ rising under load."

**Mapping:**

| Xue et al. (2026) | This Framework |
|---|---|
| Task uncertainty | $L^*$ (allostatic load) |
| Feature interference | $K$ (curvature) |
| Enhanced irrelevant encoding | $W^*$ narrowing |
| Non-orthogonal feature axes | $\Theta^*$ degradation |
| Dimensionality loss | $W^* \times \Theta^*$ collapse |
| Perceptual accuracy drop | $C_s$ reduction |

**Why this matters.** Xue et al. is an independent confirmation of the curvature mechanism from a different research program with different vocabulary, methods, and anatomical targets. The convergence is the evidence: the same geometric mechanism appears whether you call it "feature interference" or "curvature."

**Cross-reference:** Central Reference anchor A28 specifies this connection. Precision v3.4 §1.11 has the full mapping.

---

### 5a.11 REQT — The Qualification Threshold

Precision is necessary for the loop to run, but not sufficient. The system must also be qualified — the substrate must be in a state where the loop can be sustained. REQT is the condition under which Intelligence > 0 is sustained. When REQT ≤ 0, $\Lambda \to 0$ and the intelligence product collapses regardless of $n_{hops}$, $R^*$, or $\Theta^*$.

$$REQT = \left(\frac{A_s^*}{A_{s,0}^*} \cdot \frac{R^*}{R_0^*} \cdot \frac{W^*}{W_0^*} \cdot \frac{\Theta^*}{\Theta_0^*} \cdot \frac{I^*}{I_0^*}\right) - L^* > 0$$

**Note on weighting.** REQT uses equal weights as a conservative qualification default — any component falling significantly below baseline is treated as a disqualifier regardless of compensating strength in other components. The master equation uses unequal weights because they reflect the empirical collapse sequence (precision degrades first). REQT weights reflect minimum viable threshold — a different question.

**Requalification condition:**

$$REQT > 0 \quad \text{after} \quad L^* < L^*_{threshold} \quad \text{AND} \quad \Lambda > 0 \quad \text{for} \geq 48h$$

**The gate-lowering failure mode.** As $L^*$ rises, $P_{threshold} = P_0 - \gamma L^*$ drops. The gate remains open but admits lower-quality signal. The decision-maker appears functional. The output is Path B dressed as Path A. This is the most dangerous failure mode — it is undetectable from behaviour alone.

**Component REQT.** Composite REQT can be passed while a single component is at critical load:

$$REQT_{component} = REQT_{composite} \wedge (\max_i L^*_i < L^*_{critical,i})$$

A system passes REQT only if both total load is manageable AND no single component is at critical level.

**Cross-reference:** Central Reference §3.7 formalizes the full REQT equation. Precision v3.4 §1.12 has the precision-framework version. Allostatic Load v2.1 §10c describes the clinical signature of the gate-lowering failure mode.

---

### 5a.12 The Collapse Sequence

Collapse does not happen uniformly. It proceeds in a topologically forced order. This determines the monitoring priority.

```
STAGE 1 — PRECISION DROP        R* ↓       Detectable: HRV coherence loss
STAGE 2 — WINDOW NARROWING      W* ↓       Detectable: Flexibility composite drops
STAGE 3 — INTEGRATION FAILURE   Θ* ↓       Detectable: Ambiguity task degrades
STAGE 4 — RESOLUTION FLOOR RISE δ_min ↑    Detectable: Miss rate rises on low-amplitude signals
STAGE 5 — GATE CLOSURE          Λ → 0      Detectable: High-confidence, low-variance output
STAGE 6 — PRIOR CALCIFICATION   U ≈ 0      Detectable: Update rate collapses under contrary evidence
```

**Critical annotation on Stage 5:** Stage 5 looks like competence from the outside. Output becomes high-confidence and low-variance — precisely the signature of an expert operating from deep prior. Monitoring protocols that wait for Stage 5 are measuring the terminal state. The monitoring window is Stages 1–2.

**Connection to precision.** Stage 1 is precision collapse. The entire sequence begins with $R^*$ dropping. This is why the precision framework is the measurement layer for the collapse sequence. The CO₂ tolerance window determines when precision collapses. The load-compressed ceiling $C_{high}(L^*)$ determines how close the system is to that collapse at any given moment.

**Cross-reference:** Central Reference §5b specifies the full sequence with zone correspondence. Precision v3.4 §1.13 has the precision-framework version. Allostatic Load v2.1 §3b connects the zones to the stages.

---

### 5a.13 The Four Qualification Profiles

The branch condition is determined by the interaction of PE sensitivity, PE tolerance, encoding curvature, and routing capacity. Four profiles are distinguishable:

| Profile | $\sigma_{PE}$ | $\tau_{PE}$ | $K_{enc}$ | $I^*$ | Qualification Status |
|---|---|---|---|---|---|
| **High-gain, high-tolerance** | High | High | Low | High | **Qualified** — detects PE, gate stays open, loop runs, prior updates |
| **High-gain, low-tolerance** | High | Low | Low | High | **Conditionally qualified** — detects PE but cascade fires |
| **Standard-gain, high $K_{enc}$** | Low | Any | High | Moderate | **Disqualified for novel domains** — doesn't detect PE, or suppresses it |
| **Low $I^*$ (any gain)** | Low | Low | Any | Low | **Disqualified** — ambiguity unresolvable regardless of gain or tolerance |

**The fourth profile is the most clinically important.** When $I^*$ collapses — through dissociation, chronic interoceptive avoidance, or interoceptive load — the system cannot resolve ambiguity regardless of its gain or tolerance. Avoidance becomes the default behavior.

**Connection to precision.** The CO₂ tolerance window determines which profile a person can access. Low $C_{high}$ means the system is closer to jitter onset. High $C_{high}$ means the window is wide and the gate can stay open longer. Precision lock is the physiological signature of the qualified profile.

**Load profiles vs. qualification profiles.** This section describes *qualification profiles* — whether the system is qualified to run the loop. Allostatic Load v2.1 §7a describes *load profiles* — where the debt is concentrated across five components. These are orthogonal: a person can have high $L^*_{HRV}$ (load profile: autonomic debt) and be in the high-gain, high-tolerance qualification profile (qualified to run the loop).

**Cross-reference:** Central Reference §6 specifies the full profile table. Precision v3.4 §1.14 has the precision-framework version.

---

### 5a.14 The Load Decomposition

$L^*$ is not a scalar state — it is a profile across five components. Each component is calculated as a drift from the individual's own baseline.

$$L^* = w_1 L^*_{HRV} + w_2 L^*_{RHR} + w_3 L^*_{temp} + w_4 L^*_{inflam} + w_5 L^*_{resp}$$

$$\sum_i w_i = 1$$

**Default weights (proposed — subject to empirical calibration):**

| Component | Weight | Rationale |
|---|---|---|
| $L^*_{HRV}$ | 0.30 | HRV baseline drift is the earliest indicator of cumulative debt |
| $L^*_{RHR}$ | 0.25 | Sleep RHR elevation reflects persistent background demand |
| $L^*_{temp}$ | 0.15 | Temperature elevation reflects inflammatory load |
| $L^*_{inflam}$ | 0.20 | Chronic inflammation reflects long-term regulatory debt |
| $L^*_{resp}$ | 0.10 | Respiratory inefficiency reflects bracing and diaphragm lock |

**Each component** is computed as a within-person drift:

$$L^*_{component} = \frac{Value_{current} - Baseline_{component}}{Baseline_{component} - Floor_{component}}$$

Where $Baseline_{component}$ is the 30-day median and $Floor_{component}$ is the 30-day minimum (for markers that decrease with load) or maximum (for markers that increase with load).

**The composite vs. diagnostic distinction:**

- **Composite $L^*$:** total debt magnitude. Appropriate when multiple components are elevated and the question is overall load.
- **Diagnostic $L^*_{diagnostic} = \max_i L^*_i$:** where the debt is concentrated. Appropriate for treatment targeting.

**Minimum viable measurement** (HRV-only):

$$L^* \approx \frac{1}{2}\left( \frac{HRV_{morning} - HRV_{evening}}{HRV_{morning} - HRV_{floor}} + \frac{HRV_{max} - HRV_{sleep}}{HRV_{max} - HRV_{floor}} \right)$$

**Component critical load $L^*_{critical,i}$.** The composite $L^*$ can pass REQT while a single component is at critical load. $L^*_{critical,i}$ is the threshold for each of the five components. When any single component exceeds its critical value, the system fails component REQT (§5a.11) regardless of the composite. This prevents false-positive qualification of systems with isolated severe debt.

**Calibration:** Component threshold values are individual calibration parameters. They are not population constants. Calibration protocol: measure $L^*_i$ for each component across a range of load states, identify the point at which the corresponding functional domain (cognitive performance, autonomic regulation, inflammatory response) shows measurable degradation, and fit the threshold per individual. See Central Reference §2.9 for the specification.

**Load-compressed CO₂ ceiling.** $L^*$ enters the precision framework directly by compressing the CO₂ ceiling:

$$C_{high}(L^*) = C_{high}^0 - \gamma L^*$$

High load means a narrower CO₂ window. The same absolute CO₂ level produces jitter at lower values when load is high.

**Cross-reference:** Central Reference §2.10 specifies the full decomposition. Allostatic Load v2.1 §6 specifies the measurement protocols. Precision v3.4 §1.15 has the precision-framework version.

---

## 6. The Prior Loop

$$\text{Manifold geometry} \rightarrow \text{Prior quality} \rightarrow \text{Budget allocation efficiency} \rightarrow \text{Manifold geometry}$$

The loop runs in both directions. The geometry shapes the prior. The prior shapes the geometry. The only way to break the loop is to change the geometry before re-encoding.

---

### 6a. The Prior Update Rate

$$\mathcal{U} = \frac{A_s^* \cdot R^* \cdot \Theta^*}{1 + \gamma K_{enc}}$$

| Variable | Role in Prior Update |
|---|---|
| $A_s^*$ | Amplitude determines how much signal is available to write with |
| $R^*$ | Precision determines how cleanly the signal writes — high jitter produces fragmented priors |
| $\Theta^*$ | Integration efficiency determines whether disparate signals encode together or fragment |
| $K_{enc}$ | Curvature at encoding is the critical variable — determines what geometry the new prior carries forward |

**The curvature contamination rule:**

$$K_{enc} \uparrow \rightarrow \mathcal{U} \downarrow \text{ — prior carries forward curved geometry}$$

$$K_{enc} \downarrow \rightarrow \mathcal{U} \uparrow \text{ — prior carries forward flat geometry}$$

The curvature at encoding determines what every future encounter with that signal costs — fear persistence, trauma, therapy efficacy, and insight failure are all downstream of $K_{enc}$.

| Timescale      | Variable             | What It Captures                                                  |
| -------------- | -------------------- | ----------------------------------------------------------------- |
| Instantaneous  | $C_s$                | Current usable bandwidth                                          |
| Cycle-level    | $K$, $R^*$, $W^*$    | How budget is allocated this breath cycle                         |
| Encoding event | $\mathcal{U}$ at $K_{enc}$ | What geometry was just written into the prior layer |
| Accumulated    | Prior topology       | Manifold shape built from history of $\mathcal{U}$ at varying $K_{enc}$ |

**The intervention sequence:**

1. Change the geometry first — breath stabilization drops $K_{enc}$
2. Introduce the signal — reaches encoding layer from flat geometry
3. $\mathcal{U}$ writes a flat prior — new encoding does not carry old curvature forward
4. Geometry updates — future $C_s$ has a different floor

Skipping Step 1 means $\mathcal{U}$ writes under the same curvature that produced the original prior. Content updates. Geometry does not. The autonomic response on future encounters remains unchanged.

| Term | Role |
|---|---|
| $A_s^* \cdot R^* \cdot \Theta^*$ | Signal available × precision × integration — how much clean signal reaches the encoding layer |
| $1 + \gamma K_{enc}$ | Curvature penalty at encoding — high $K_{enc}$ suppresses update rate and writes curved geometry into the prior |
| $\gamma$ | Calibration constant — how steeply curvature suppresses prior updating. Empirically measurable |

**Connection to the encoding window.** The prior update rate $\mathcal{U}$ is the instantaneous rate at each moment within the encoding window. The encoding window $W_{enc}$ is the temporal integral of precision during encoding:

$$W_{enc} = \int_{t_{enc}} \mathbf{1}_{P(t) > P_{threshold}} dt$$

The two are related: $\mathcal{U}$ is the rate, $W_{enc}$ is the interval over which the rate applies. The total prior update magnitude is approximately:

$$\text{Update} \approx \int_{t_{enc}} \mathcal{U}(t) \cdot \mathbf{1}_{P(t) > P_{threshold}} dt$$

High $W_{enc}$ with high $\mathcal{U}$ produces the strongest prior update. This is why the intervention sequence above specifies: change the geometry first (raise $P$, widen $W_{enc}$), then introduce the signal (run $\mathcal{U}$ at flat $K_{enc}$).

**Why $\mathcal{U}$ not $dM/dt$:** The original notation implied a differential equation with a solvable functional form. $\mathcal{U}$ is a rate estimate at a specific encoding event — a snapshot of how much clean signal reached the encoding layer and under what geometry. If formal continuous dynamics are needed, $\mathcal{U}$ is the natural starting point for a proper ODE. That is future work.

**Cross-reference:** Precision v3.4 §4.6 specifies the full $W_{enc} \leftrightarrow \mathcal{U}$ mapping. Central Reference §3.8 formalizes the prior update rate.

---

### 6b. The Motor Encoding Layer: Why Distortion Is Not Random

The prior loop established in Section 6 runs at the cognitive level — geometry shapes prior quality, prior quality shapes budget efficiency, budget efficiency shapes geometry. But the loop has a substrate layer running below cognition, one that determines *where* the manifold distorts and *why* that distortion is not random.

**The substrate is the motor encoding layer. The bridge is interoception.**

---

#### 6b.1 Movement Patterns as Manifold Topology

The radial structure of the manifold (Section 4) describes distance from center in terms of energetic priority. What that table does not specify is how the topology of "near" and "far" is established for any individual system. The answer is motor encoding:

> **What counts as "near" on the manifold is whatever the cached motor patterns already reach. What counts as "far" is whatever they do not.**

Motor patterns that have been encoded and cached run on cerebellar-basal ganglia circuits — low overhead, no PFC coordination required. They are energetically "near" regardless of their physical complexity. Motor patterns that have never been encoded, or that have been abandoned, require PFC coordination to execute — high cost, high overhead, energetically "far."

The manifold does not have a universal topology. It has a **personally constructed topology** — built from the history of movement patterns the system has encoded, reinforced, and cached.

#### 6b.2 Interoception as the Encoding Bridge

The mechanism connecting the motor layer to the prior layer is interoception. The interoceptive signal does not merely report body state — it is the **signal the system uses to assign energetic cost to movement patterns**:

|Movement State|Interoceptive Signal|System Encoding|
|---|---|---|
|Cached pattern executed|Low cost signal — familiar, predictable|Prior: "this is easy" — path reinforced|
|Uncached pattern attempted|High cost signal — effortful, unpredictable|Prior: "this is hard" — path avoided|
|Pattern avoided under load|No new signal generated|Prior: "this is the limit" — blank zone|
|Pattern never attempted|No signal at all|Prior: absent — region does not exist in map|

The final row is the critical one. The most distorted regions of the manifold are not where the interoceptive map says *danger* — they are where the map says *nothing*. The system interprets absence of interoceptive data as capacity limit, because under a finite energy budget, unexplored regions are indistinguishable from inaccessible ones.

> **The system experiences blank map as "can't." The blank is not a boundary. It is the absence of cartography.**

#### 6b.3 The PFC Economy Loop

Under load, $W$ narrows and PFC access contracts toward the geometric center (Section 4). This contraction creates a selective pressure on which movement patterns the system can execute in real time.

Motor patterns that have been encoded and cached run on cerebellar-basal ganglia circuits. They are automatic — executed without PFC coordination, at negligible overhead cost. Under any level of load, they remain accessible. Motor patterns that have not been encoded require PFC coordination to initiate and sustain. They are expensive under normal conditions and inaccessible under elevated $K$.

The consequence is structural:

$$\text{Load} \uparrow \rightarrow K \uparrow \rightarrow W \downarrow \rightarrow \text{PFC access} \downarrow \rightarrow \text{Uncached movement inaccessible} \rightarrow \text{System defaults to cached patterns}$$

Defaulting to cached patterns under load is not failure — it is efficient energy conservation. The system is doing exactly what it should do given finite resources and rising curvature. But the structural consequence is that **the conditions under which novel movement is most needed are exactly the conditions under which it cannot be accessed.**

This is the mechanism behind postural bracing, trauma fixation, and chronic compensatory patterns. The brace is the cached pattern — low cost, always accessible, reinforced by every load event that causes the system to default to it. The open posture, the full breath, the unrestricted movement — these are the uncached alternatives, expensive under load, inaccessible precisely when the system most needs them.

$$\text{Brace} = \text{Low PFC cost} = \text{"Near"} = \text{Reinforced under load}$$
$$\text{Release} = \text{High PFC cost} = \text{"Far"} = \text{Inaccessible under load}$$

Each load event deepens the encoding gap. The cached pattern becomes more automatic. The uncached alternative becomes more foreign. Over time the gap is experienced not as a habit but as a fixed trait — *"I am someone who holds tension here," "I cannot move that way"* — because the interoceptive signal has never reported otherwise.

The trait is the topology. The topology was constructed by the economy.

#### 6b.4 Distortion Topography Is Diagnostically Informative

Because distortion follows motor encoding gaps rather than distributing randomly, the location of manifold distortion is predictable and readable:

|Distortion Location|What It Indicates|Entry Point|
|---|---|---|
|Prefrontal, bilateral access|Uncached integrative movement — breath, postural coordination|Diaphragmatic range, thoracic mobility|
|Emotional regulation regions|Uncached interoceptive exposure — felt sensation avoided|Slow breath hold, felt-sense practice|
|Social cognition|Uncached regulatory role expression — compliance pattern cached|Role expansion, non-compliance practice|
|Temporal integration|Uncached oscillatory range — amplitude ceiling low|CO₂ tolerance training, extended exhale|

Two individuals under identical external load will distort differently — because they have different motor encoding histories, and their interoceptive maps reflect those histories as topology.

> **The distortion map is not a symptom profile. It is a motor vocabulary inventory.**

#### 6b.5 The Complete Control Loop

The prior loop established in Section 6 runs at the cognitive level — geometry shapes prior quality, prior quality shapes allocation efficiency, allocation efficiency shapes geometry. The motor encoding layer established in Sections 6b.1 through 6b.4 runs one level below that. Together they form the complete control system of the manifold:

$$\text{Motor pattern cached} \rightarrow \text{Interoceptive signal generated} \rightarrow \text{Prior encoded} \rightarrow \text{Manifold geometry set} \rightarrow \text{PFC economy enforced} \rightarrow \text{Cached pattern reinforced} \rightarrow \text{Loop}$$

This loop runs without deliberate input. It is the system actively reproducing its own topology at every breath cycle, through the interoceptive reporting of cached motor cost. The geometry is not imposed from outside — it is generated from within, continuously, by the body reporting back what it has learned to reach.

The loop is self-sealing. A curved prior encodes a restricted movement range. A restricted movement range generates interoceptive signal only within that range. Signal only within that range updates only the priors already present. The new priors carry the same curvature forward. Nothing from outside the current topology can enter unless the movement changes first.

**This is why the loop cannot be broken from the cognitive layer.** Narrative reframing, insight, awareness — these operate on the prior layer. But the prior layer is downstream of the interoceptive signal, and the interoceptive signal is downstream of the movement. Changing the content of the prior without changing the movement that generates the interoceptive signal that sustains it is working against the write direction of the constructing function. The geometry absorbs the new content and re-encodes it under the existing curvature.

The intervention sequence is therefore not optional:

1. **Change the movement** — introduce range that the cached patterns do not reach
2. **Hold it long enough** — generate interoceptive signal in the blank zone
3. **Let the signal write** — the prior layer updates from the new signal, not from instruction
4. **The geometry changes** — curvature drops, $W$ widens, new cognitive range becomes accessible
5. **Now the prior can be re-encoded** — from a flat geometry, without carrying the old curvature forward

This is the mechanism underlying every effective bottom-up intervention — somatic therapy, breathwork, postural training, yoga, movement-based trauma protocols. They are not separate modalities with separate theories. They are all applying the same write sequence to the same constructing function. The traditions that discovered this independently discovered it because it works, and it works because the mechanism is structural.

The corollary is equally precise: **every intervention that skips Step 1 is attempting to write to the prior layer without opening the write channel.** The insight may be real. The awareness may be genuine. The reframe may be accurate. None of it reaches the topology until the body moves.

#### 6b.6 The Hypermobility Clarification

Hypermobility does not provide more hardware. It provides more of the hardware mapped. A wider physical range means more movement patterns encoded across development — more regions with interoceptive data, fewer blank zones. The geometric advantage is cartographic, not architectural.

#### 6b.7 Social Compliance as Topology Restructuring

When movement is systematically restricted by social signal — compliance requirements, masking, role enforcement — the restriction does not remain at the behavioral layer. Through $\mathcal{U}$, it is written into the manifold topology. The interoceptive signal reports the constrained range as the available range. The compliance becomes the geometry.

This mechanism applies at every scale — individual, cultural, institutional, and AI alignment training. In every case the social signal restricts movement, the restricted movement generates no interoceptive signal, the absent signal encodes as a limit, and the limit becomes the topology. See Section 15 for the social scale projection.

**The mask becomes the face. The compliance becomes the manifold.**

Unmasking is not psychological — it is geometric. New movement into the restricted range, interoceptive signal generated and held, prior layer updated from the body up. The territory was always there. The map stopped reporting it.

#### 6b.8 Motor Gain Formalization

The motor encoding layer (§6b.1–6b.7) describes the mechanism by which motor patterns set manifold topology. This section formalizes the gain variables that connect precision to motor output — the "limb with gain requiring control" formulation.

**Motor gain.** The amplification of motor intention:

$$G_m = \alpha P - \beta \eta$$

Where:
- $\alpha$ is the precision-to-gain conversion coefficient (individual parameter)
- $P$ is precision (timing coherence)
- $\beta$ is the noise sensitivity coefficient (individual parameter)
- $\eta$ is the neural noise floor

**Operational Measurement:** Motor gain is approximated using EMG amplitude, movement overshoot, and tremor amplitude.

**Movement stability.** The inverse of movement drift:

$$\text{Stability} = \frac{1}{G_m \cdot \text{Drift}}$$

Where Drift is the variance in motor output relative to intention:

$$\text{Drift} = \text{Var}(X_{intended} - X_{actual})$$

**Collapse risk.** The probability of precision loss during movement:

$$C_{risk} = \frac{\gamma \cdot G_m}{1 + \text{Cache}}$$

Where Cache is the availability of cached movement patterns:

$$\text{Cache} = \frac{N_{cached}}{N_{total}}$$

**Motor state.** The discrete state of the motor system:

$$M_{state} = \begin{cases}
\text{Stable} & \text{if } G_m < G_{threshold} \text{ and Cache} > \text{Cache}_{min} \\
\text{Unstable} & \text{if } G_m > G_{threshold} \text{ or Cache} < \text{Cache}_{min} \\
\text{Collapsed} & \text{if } C_{risk} > C_{threshold}
\end{cases}$$

**The limb with gain requiring control is the unstable state** — gain is high but control is sufficient to maintain stability. Collapse occurs when gain exceeds control capacity.

**Calibration note.** The thresholds $G_{threshold}$, $\text{Cache}_{min}$, and $C_{threshold}$ are individual calibration parameters, not population constants. No current prediction calibrates them directly. The relevant measurements are:

- PREDICT-PREC-06 measures $G_m$ but does not calibrate $G_{threshold}$
- PREDICT-MOTOR-01 measures distortion location but not motor state transitions
- PREDICT-MOTOR-02 measures sequencing effects but not motor state thresholds

Calibration of $M_{state}$ thresholds is an open empirical question. The formal protocol would be: induce motor load across the stable–unstable–collapsed range, measure $G_m$, Cache, and $C_{risk}$ at each transition point, and fit the threshold values per individual. This is the motor analog of the $\tau_{threshold}$ and $K_{critical}$ calibration in §5a.13 and Central Reference §2.9.

**Cross-reference:** Central Reference §2.11 and §3.11 specify the motor gain variables and equations. Precision v3.4 Part III specifies the full derivation and operational measurement.

#### 6b.9 The Four-Layer Cache Hierarchy

The motor encoding layer sits within a four-layer geometric hierarchy that determines access order and collapse sequence. This hierarchy is the biological implementation of the precision-cache architecture and is specified in full in *The Geometry of Inference* v1.0 §1.1. The four layers are:

```
LAYER 0: SURVIVAL GEOMETRY
Always funded. Zero access cost. Autonomic regulation, threat detection, 
basic motor coordination. Never goes offline.

    LAYER 1: LEFT HEMISPHERE — INNER CORE
    Written through lifetime repetition. Compressed into low-cost retrieval 
    patterns. Local, cooperative inference. Pattern completion. Categorical 
    reasoning. Prior retrieval. Always accessible. Never collapses before 
    Layer 3.

        LAYER 2: PFC — THE GATE
        Threshold-controlled. Opens when precision conditions are met. Routes 
        energy to the outer edge. Determines whether the miss penalty is 
        worth paying. Closes under load. Gate failure precedes outer collapse.

            LAYER 3: RIGHT HEMISPHERE — OUTER EDGE
            Requires gate to open. Requires coherent signal. Requires live 
            pathway. Adversarial evidence. Wide semantic field. Long-range 
            integration. Collapses first under any form of degradation.
```

**The topological invariant:** You cannot reach Layer 3 without traversing Layers 0, 1, and 2. There is no right-hemisphere-only state. This is not an empirical generalization — it is a consequence of the manifold's topology. The clinical record confirms it: every condition that damages or suppresses the left hemisphere leaves the right hemisphere partially accessible, but always accessed through, and often distorted by, a compromised inner core. What is never observed is right-hemisphere processing while the left hemisphere is offline.

**Access rule.** The gate (Layer 2) opens when $P_{eff} > P_{threshold}$ and $O_{pathway} > O_{min}$. Below threshold, processing remains in Layers 0–1 (prior retrieval, Path B). Above threshold, Layer 3 becomes accessible (adversarial inference, Path A).

**Collapse order.** The four-layer hierarchy produces the topologically forced collapse sequence of §5a.12. Precision drops first (Layer 3 access degrades), then window narrows (Layer 2 threshold rises), then integration fails (Layer 2 → Layer 3 traversal fails), then resolution floor rises (Layer 1 comparison granularity coarsens), then gate closes (Path B becomes default), then prior calcification (Layer 1 stops updating).

**Circuit analogy.** The manifold is not a diode — current does not flow only one way. It is a circuit: once a pathway has been used with sufficient precision, its access cost drops. This is the warm-up effect specified in §6b.10.

**Cross-reference:** GoI v1.0 §1.1 specifies the four-layer hierarchy in full. GoI v1.0 §1.6 specifies the circuit priming effect.

#### 6b.10 Circuit Priming

The competitive scaffold that constitutes $W^*$ (§5.2) is not static. It is maintained through use — through sustained precision-gated access that traverses the long-range connections.

**The mechanism.** When precision is high and the gate opens, the pathway from inner core (Layer 1) to outer edge (Layer 3) is traversed. The competitive connections along that pathway are reinforced — connection density increases, impedance drops. The next time a similar signal arrives, the cost to access the same outer-edge region is reduced. The manifold has been "primed."

**Why recovery is asymmetric.** A system that has lost access to the outer edge does not regain it simply by restoring precision. The competitive scaffold must be rebuilt through sustained precision-gated access. The circuit must be re-warmed. This is the substrate mechanism behind the collapse hysteresis $\delta_{hyst}$ specified in §5a.5 — the hysteresis penalty is not just residual jitter and sympathetic activation; it is the cost of rebuilding the competitive scaffold that erosion degraded.

**The priming effect in practice.** Recently used manifolds have reduced cost to access. A system that has just completed a high-precision adversarial inference task can perform the next similar task at lower energetic cost than a system starting cold. This is the mechanism behind warm-up in expert performance, the reduced cost of repeated exposure in desensitization protocols, and the increased difficulty of engaging a skill that has not been used recently.

**Cross-reference:** GoI v1.0 §1.6 specifies the circuit priming effect. The competitive scaffold substrate is specified in §5.2 above (Roy & Banerjee, 2026 — 25–40% of brain connections are negative).

---

## 7. The Felt Geometry

The geometry is not abstract. It is experienced directly:

| Geometry State | Felt Experience | Self-Detectable Signal |
|---|---|---|
| Flat manifold | Clarity, presence, ease, fluid cognition | "I can think clearly. The world feels stable." |
| Curvature increasing | Unease, tension, narrowing attention | "I feel off. Things feel tighter." |
| $W^*$ narrowing | Tunnel vision, impatience, fragmented thought | "I can't think straight. Everything feels urgent." |
| $K$ high | Overwhelm, reactivity, cognitive fatigue | "I'm running on empty. Everything is too much." |
| $C_s \approx 0$ | Numbness, derealization, shutdown | "I'm not here. Nothing feels real." |

The shift you feel on a slow exhale is the geometry changing. The breath is the lever.

---

## 8. Empirical Anchors

Each claim in this framework is already supported by existing empirical literature. The framework is the map that shows how they fit together.

| Anchor | Framework Claim | Citation / Source | What It Confirms |
| ------ | ---------------- | ----------------- | ---------------- |
| 01 | The manifold exists and has geometry | *Chaos, Solitons & Fractals*, 2026 | Neural manifolds are real, measured, and functional |
| 02 | $A_s^*$ funds $W^*$ via $R^*$ | *Neuroscience*, 2025 | HRV predicts cognitive performance — amplitude and precision jointly determine window width |
| 03 | Intervention effects depend on baseline geometry | HRVB systematic review | "Inconsistent results" across HRV biofeedback studies are predicted by the formula |
| 04 | $\Theta^*$ is real and measurable | Dono et al. (2020) — *Frontiers in Neurology* | Hemispheric laterality affects autonomic regulation |
| 05 | Containment cost raises $K$ independently of $A_s^*$ | Reed et al. (2020) — *Collabra: Psychology* | Suppression depletes resources even when HRV is stable |
| 06 | Priors encoded under high $K$ carry curvature forward | Haghian et al., 2025 | Emotional encoding systematically distorts recall |
| 07 | Collapse proceeds radially inward | ADNI, 2016 | Neurodegeneration follows the predicted outer→inner sequence |
| 08 | Geometry must change before re-encoding works | Mathersul et al., 2024 | Baseline HRV moderates which therapy works |
| 09 | Social co-regulation restores $\Theta^*$ | EDM concert physiology + religious practice convergence + CA2-CA1 gamma (2023) | Every major civilization independently built synchronized group rhythm as a core regulatory protocol |
| 10 | FND is $C_s \approx 0$ via $I^* \rightarrow 0$, not structural lesion | Maurer et al. (2016) — *Parkinsonism & Related Disorders* | FND is a routing failure — $I^*$ collapses while amplitude and precision may remain partially intact |
| 11 | Cached motor patterns shift from PFC-dependent to low-overhead cerebellar-basal ganglia execution | Diedrichsen & Kornysheva (2015) — *Nature Reviews Neuroscience* | Motor automatisation produces measurable reduction in PFC overhead |
| 12 | $I^*$ — interoception reports movement cost and gates prior encoding | Garfinkel et al. (2015) — *Neuropsychologia*; Craig (2009) — *Nature Reviews Neuroscience* | Interoceptive accuracy predicts emotion regulation, prior formation, and cognitive updating |
| 13 | Unexplored physical range produces blank interoceptive zones experienced as capacity limits | Moseley & Flor (2012) — *Nature Reviews Neuroscience* | Cortical body maps shrink with movement disuse and expand with exploration |
| 14 | $I^*$ routes to a region → signal amplifies (gain control loop) | Petzschner et al. (2018) — HEP study | Attention to heartbeat increases HEP amplitude |
| 15 | $I^*$ routing modulates peripheral physiology directly | Mizrachi et al. (2026) — *Attention shapes inflammation* | Attention to inflamed area reduces inflammation ~1.5-fold within minutes |
| 16 | $I^* = I^*_{total} - I^*_{vision}$ — sensory load is arithmetically subtracted | NeuroImage (2024) — visual-interoceptive trade-off study | Visual stimuli during systole reduce visual processing |
| 17 | Eyes closed restores $I^*$ routing to interoceptive channel | Postural balance study (2024) | Higher cardiac awareness predicts better balance with eyes closed |
| 18 | Precision is a timing-coherence ratio of sync duration over timing distance | Pratap et al. (2026) — Cardiorespiratory coupling during encoding | PLV measures the ratio of sync duration to timing distance |
| 19 | CO₂ tolerance window determines precision peak | Sakakibara et al. (1994) — Voluntary apnea and EEG-HRV | Hypercapnia depresses cortical activity; theta correlates with parasympathetic activity |
| 20 | Resonance breathing produces stable precision | Yamamoto et al. (2006) — Zen meditation EEG-HRV | Interhemispheric coherence increases with parasympathetic activation |
| 21 | Collapse hysteresis delays recovery | Reed et al. (2020) — Suppression depletes resources | Recovery time exceeds collapse time |
| 22 | Nasal respiration entrains limbic oscillations | Zelano et al. (2016) — *Journal of Neuroscience* | Memory recall better during inhalation; effects disappear with mouth breathing |
| 23 | CO₂ drives cerebral vasodilation | Raichle & Plum (1972) — *Stroke* | Hyperventilation produces vasoconstriction; hypocapnia reduces cerebral blood flow |
| 24 | Slow breathing produces HRV and EEG coherence | Zaccaro et al. (2018) — *Frontiers in Human Neuroscience* | Systematic review of slow breathing protocols; frequency-dependent effects |
| 25 | Breathing training shifts parameters | Kox et al. (2014) — *PNAS* | Wim Hof practitioners show different autonomic responses to endotoxin |
| 26 | Control Pause measures $C_{high}$ individually | Cooper et al. (2003) — *Thorax* | Buteyko trial — CP varies, shifts with training |
| 27 | Hypocapnia produces cognitive and anxiety collapse | Meuret & Ritz (2010) — *Int. J. Psychophysiology* | Panic disorder characterized by low CO₂; raising CO₂ reduces panic |
| 28 | Feature interference is $K$ rising | Xue et al. (2026) | Axis entanglement in V1 confirmed causally — non-orthogonality under task uncertainty |
| 29 | Hyperventilation impairs cognitive function | Tsukamoto et al. (2014) | CBF drop → cognitive impairment |
| 30 | PV+ interneurons are metabolically vulnerable | Kann et al. (2015) | Cellular mechanism for $K$ rise |
| 31 | ΔCBF/ΔCMRO₂ predicts neural efficiency | Hutchison & Rypma (2013) | Metabolic signature of high $K$ |
| 32 | Baseline vascular state sets activation ceiling | CVR literature | Physical constraint on outer edge |
| 33 | EEG-HRV coupling emerges during hyperventilation | Titov & Dick (2022) | Partial anchor for $R^* \rightarrow K$ |
| 34 | Path A/B = epistemic vs. extrinsic value | Friston et al. (2015) | Formal branch condition |
| 35 | Impaired IAc → emotional learning failure | Schäflein et al. (2018) | Behavioral endpoint of low $I^*$ |
| 36 | Stress narrows visual processing | Yang et al. (2026) | Cross-scale visual integration in V1 |
| 37 | HRV stressor signatures are distinct | Villatte et al. (2026) | Different loads reshape variables in specific ways |
| 38 | Methylphenidate increases dimensionality | Ni et al. (2022) | Pharmacological $K$ reduction improves performance |
| 39 | Working memory capacity ~5 items | Cowan (2016) | Dimensionality limit |
| 40 | Chunking compresses dimensions | Thalmann et al. (2019) | Effective compression of representations |
| 41 | Confirmation bias has no mechanistic account | Nickerson (1998) | 25-year gap — framework provides mechanism |
| 42 | System 1/System 2 branch | Kahneman (2011) | Path B / Path A described without naming |
| 43 | Deliberate practice requires edge-of-ability | Ericsson et al. (1993) | Structured loop-running |
| 44 | Expert recognition is compressed loop history | Klein (1998) | Recognition IS cheap retrieval |
| 45 | Intuition reliable in high-validity environments | Kahneman & Klein (2009) | Feedback IS error signal |
| 46 | Cognitive plasticity requires boundary operation | Lövdén et al. (2010) | Loop running on novel input |
| 47 | Neuroplasticity from skill learning | Draganski et al. (2004) | Loop writes into substrate |
| 48 | Plants exhibit adaptive behaviour | Trewavas (2003) | Slow loop at seasonal timescale |
| 49 | Plants habituate and retain learned responses | Gagliano et al. (2014) | Prior update from error signal exposure |
| 50 | Hot cache survives aging, RAM access degrades | Billot et al. (2026) | Outer edge degrades first |
| 51 | Competition is 25–40% of brain connections | Roy & Banerjee (2026) | Competitive scaffold is real |
| 52 | LP-ACC circuit detects change | Leow et al. (2026) | Cache miss controller identified |
| 53 | ACC activity scales with prediction error | Botvinick et al. (2001) | Biological loop detector |
| 54 | Beta oscillations signal prior maintenance | Engel & Fries (2010) | Measurable signature of loop suppression |
| 55 | Free-energy principle describes both paths | Friston (2010) | Path A/B in thermodynamic terms |
| 56 | Continuous wearable HRV measurement validates variance as signal | Oura, WHOOP, Garmin, Apple, Polar, Biostrap | HRV variance is real physiology, not measurement noise |
| 57 | Daily HRV variance predicts outcomes better than mean | Okawara et al. (2024) | The signal the field calls noise is the load trajectory |
| 58 | HRV follows circadian rhythm with individual chronotype variation | Vitale et al. (2019); Li et al. (2024) | Time-of-day is a feature, not noise |
| 59 | Glymphatic clearance drives interstitial solute clearance during slow wave sleep | Iliff et al. (2012); Grunewald et al. (2012) | Substrate for load recovery during sleep |
| 60 | Chronic vagal tone and CAP share efferent pathway | Tracey (2002); Thayer et al. (2010) | HRV is a real-time indicator of anti-inflammatory brake integrity |

_These anchors confirm each component of the framework independently. The full causal chain — connecting all of them in sequence — is the novel contribution._

---

## 9. Perceptual Confirmation Across Sensory Systems

Every sensory domain that depends on integration degrades under load in the same geometric pattern — window narrows, precision drops, outer regions lose access first. These studies were not designed to test this framework. The convergence is the evidence.

| Sensory Domain | Readout | Manifold Variable | What the Literature Shows |
|---|---|---|---|
| **Spatial—Visual** | Color constancy | $W^*$ | Stress reduces color constancy; anxiety drives local contrast dominance |
| **Spatial—Visual** | Contrast sensitivity | $\sigma(A_s)$, $R^*$, $W^*$ | Cognitive load and anxiety reduce fine contrast sensitivity |
| **Spatial—Visual** | Peripheral vision | $W^*$ | Threat and hyperventilation collapse peripheral integration → tunnel vision |
| **Spatial—Visual** | Depth perception | $W^*$ | Stress reduces stereoscopic accuracy |
| **Temporal—Auditory** | Rhythm perception | Phase-locking, $R^*$ | Stress disrupts beat tracking; vagal tone improves rhythm perception |
| **Temporal—Auditory** | Speech-in-noise | $W^*$ | Stress and load reduce speech-in-noise comprehension |
| **Temporal—Visual** | Motion perception | $W^*$ | Anxiety distorts motion perception; narrow window → jerky appearance |
| **Semantic** | Ambiguity resolution | $W^*$ | Load reduces contextual resolution of ambiguous input |
| **Semantic** | Pronoun resolution | $W^*$ | Stress reduces referential tracking across sentence boundaries |
| **Semantic** | Garden-path recovery | $W^*$ | Load increases reparse failure |
| **Semantic** | Prosody interpretation | $W^*$ | Anxiety reduces prosody accuracy |
| **Semantic** | Phoneme discrimination | $\sigma(A_s)$, $R^*$ | Stress reduces phoneme boundary clarity |
| **Interoceptive** | Temperature perception | $W^*$ | Stress increases thermal discomfort; CO₂ tolerance predicts thermal stability |
| **Interoceptive** | Pain sensitivity | $K$, $W^*$ | Stress increases pain sensitivity; curvature amplifies nociception |
| **Interoceptive** | Heartbeat perception | $R^*$ | Stress distorts heartbeat detection; HRV predicts interoceptive accuracy |
| **Social** | Face perception | $W^*$, $K$ | Anxiety distorts face interpretation; curvature increases false-threat reads |
| **Social** | Theory of Mind | $W^*$ | Stress reduces multi-perspective holding capacity |
| **Social** | Threat detection | $K$ | Anxiety increases false positive rate for social threat |
| **Motor** | Coordination | $\sigma(A_s)$ | Load disrupts motor phase-locking; jitter → movement instability |
| **Motor** | Reaction time variability | $\sigma(A_s)$ | Load increases RT noise |
| **Motor** | Fine motor control | $R^*$ | Anxiety produces tremor-like instability via precision loss |
| **Mnemonic** | Episodic coherence | $W^*$ | Stress fragments episodic recall; narrow window → non-sequential retrieval |
| **Mnemonic** | Temporal ordering | $W^*$ | Load increases sequence ordering errors |
| **Decision** | Future horizon | $W^*$ | Stress shortens temporal discounting horizon → apparent impulsivity |
| **Decision** | Risk perception | $K$ | Anxiety inflates threat via curvature-driven prior distortion |

**2026 High-Precision Confirmations**

| Study | Finding | Framework Claim Confirmed |
|---|---|---|
| Yang et al. — *Chronic stress impairs multi-scale visual processing in V1* | Stress reduces cross-scale visual integration in early visual cortex | $W^*$ narrows under load; spatial integration radius collapses |
| Villatte et al. — *Temporal dynamics of HRV reveal stressor-specific autonomic patterns* | Mental arithmetic, noise, and pain produce distinct HRV signatures | Different loads reshape $A_s^*$, $\sigma(A_s)$, and $R^*$ in stressor-specific ways |
| Naghibi et al. — *Indoor environmental quality and the brain* | Thermal environment linked to neural and physiological changes | Temperature perception tied to autonomic state and $W^*$ |
| *Neural dissociation of cognitive effort and physiological arousal* — Int. J. Psychophysiology | Cognitive load and arousal have separable autonomic signatures | Suppression cost and precision are geometrically distinct pressures |

> _Every interpretation that reduces this framework to metaphor, correlate, cognitive load theory, or stress research fails at the anchor table above — each variable is operationally defined, independently measured, and already in the literature._

---

## 10. Falsifiable Predictions

> *These predictions are derived from the framework and have not yet been tested. They are stated here in falsifiable form. If disconfirmed, the framework requires revision at the layer indicated.*

**PREDICT-CO₂-01 — CO₂ Tolerance Predicts $W$**

> CO₂ tolerance (breath-hold time, capnometry) will correlate with color constancy magnitude ($r > 0.5$) and with $R$ ($r > 0.6$). Manipulating breathing—load, recovery, hyperventilation—will change both.

| Field | Content |
|-------|---------|
| Test | Pre/post breathing manipulation with capnometry + ECG + color constancy task |
| Outcome if confirmed | $W$ is physiologically measurable via CO₂ tolerance |
| Outcome if disconfirmed | Framework requires revision at Layer 02 |
| Status | Untested—protocol uses off-the-shelf equipment |

**PREDICT-FND-01 — The Prodrome Is Measurable**

> HRV will show progressive amplitude collapse in the period preceding FND onset. Structural imaging will be clean. The geometric collapse will precede the symptomatic presentation.

| Field | Content |
|-------|---------|
| Test | Retrospective longitudinal wearable data (Oura, Garmin, Apple Watch) in FND patient cohort |
| Outcome if confirmed | $C_s \approx 0$ has a measurable geometric prodrome—FND is a predictable manifold collapse event |
| Outcome if disconfirmed | Framework requires revision at Layer 02 |
| Status | Untested—instrumentation now available |

**PREDICT-Γ-01 — Social Co-Regulation Restores Γ**

> Social exposure (synchronized movement, music, dance, chanting) will increase lateralized HRV coherence ($\Gamma$) within 10-20 minutes, as measured by hemispheric HRV asymmetry.

| Field | Content |
|-------|---------|
| Test | Pre/post Γ measurement in group synchrony protocols—EDM concerts, choir, dance classes |
| Outcome if confirmed | Γ is modifiable via co-regulation—social geometry is trainable |
| Outcome if disconfirmed | Framework requires revision at Layer 02 |
| Status | Untested—protocol is testable with off-the-shelf equipment |

**PREDICT-MOTOR-01 — Movement Vocabulary Predicts Distortion Topography**

> Individuals with wider cached movement vocabulary — assessed by range of motion, motor variability indices, or movement repertoire — will show less manifold distortion under equivalent cognitive load than individuals with restricted movement vocabulary, controlling for baseline HRV. Distortion location will correlate with specific movement encoding gaps rather than with emotional history or cognitive style.

| Field | Content |
|---|---|
| Test | Movement vocabulary assessment (range of motion + motor variability) + cognitive load task + continuous HRV. Compare distortion location against movement gap profile across participants. |
| Outcome if confirmed | Distortion topography is a motor vocabulary inventory — the interoceptive bridge is the mechanism, not emotional loading or cognitive type |
| Outcome if disconfirmed | Framework requires revision at Section 6b — distortion may be distributed by a parallel mechanism not captured by motor encoding |
| Status | Untested — standard motion capture and HRV equipment sufficient |

**PREDICT-MOTOR-02 — Geometry Change Precedes Prior Update**

> If the prior loop runs through the motor encoding layer, then introducing a novel movement pattern and holding it until interoceptive signal stabilizes will produce measurable prior update — reduced $K_{enc}$, wider $W^*$, reduced self-reported limit — faster than cognitive intervention alone, under equivalent time investment. The movement does not need to be symbolically related to the prior being updated. The mechanism is geometric, not associative.
>
> This prediction applies across domains. In generic prior updating: movement-first outperforms narrative-first matched for time. In bias reduction: implicit association measures will show larger effect size when motor vocabulary expansion precedes cognitive reframing, compared to cognitive reframing alone — and the effect size difference will correlate with baseline motor encoding gaps, not with the content of the bias.

| Field | Content |
|---|---|
| Test | RCT: movement-first vs cognitive-first intervention matched for time. Pre/post, self-reported prior rigidity, and behavioral outcome. Second arm: IAT or behavioral bias measure pre/post, between-group comparison of effect size with and without movement vocabulary expansion preceding reframing. |
| Outcome if confirmed | Sequencing is the active variable — movement before cognitive intervention produces larger and more durable prior update regardless of domain |
| Outcome if disconfirmed | Narrative and movement update priors via parallel channels — sequencing is not the mechanism |
| Status | Untested |

**PREDICT-SAL-01 — Salience Map Predicts Interoceptive Response, Not Stimulus Properties**

> If salience is determined by manifold topology rather than stimulus properties, then two individuals with different topology profiles — measured by baseline HRV, movement vocabulary, and prior rigidity — will show measurably different interoceptive responses to identical stimuli. The difference will correlate with topology profile, not with stimulus intensity, novelty, or objective threat level.

| Field | Content |
|---|---|
| Test | Present identical neutral-to-ambiguous stimuli to participants with pre-measured topology profiles (HRV, movement range, interoceptive accuracy). Measure interoceptive response (skin conductance, HR change, self-report). Correlate response magnitude with topology profile vs. stimulus properties. |
| Outcome if confirmed | Salience is topologically determined — the map is reading itself, not the world |
| Outcome if disconfirmed | Stimulus properties dominate response — salience is primarily bottom-up from sensory input, not top-down from topology |
| Status | Untested — standard psychophysiology equipment sufficient |

**PREDICT-SAL-02 — Geometry at Encoding Determines Durability of Change**

> If $\mathcal{U}$ is the critical variable in prior formation, then the geometry present at the moment a signal is processed — whether at initial encoding or at recall — will determine the durability of the resulting prior update. Two corollaries follow from the same mechanism:
>
> **Corollary A — Encoding geometry:** Presenting a previously aversive stimulus immediately following breath stabilization will produce measurably different interoceptive encoding than presenting it under baseline conditions, and this difference will persist at 4-week follow-up as reduced autonomic reactivity.
>
> **Corollary B — Recall geometry:** A memory recalled under breath-stabilized flat geometry will show measurably reduced autonomic reactivity at 4-week follow-up compared to the same memory recalled under baseline geometry — and the reduction will correlate with the degree of geometric flattening at time of recall, not with the content of the memory or duration of exposure.
>
> In both cases the durability is determined by $\mathcal{U}$ at the moment of processing, not by what is said, understood, or consciously experienced.

| Field | Content |
|---|---|
| Test — Corollary A | RCT: aversive stimulus under (a) baseline vs (b) post-breath-stabilization confirmed by HRV. Pre/post autonomic reactivity at baseline and 4-week follow-up. |
| Test — Corollary B | Pre/post autonomic reactivity to target memory under (a) baseline recall vs (b) breath-stabilized recall. HRV-confirmed geometry at time of recall. 4-week follow-up. Correlate outcome with $\mathcal{U}$ at recall. |
| Outcome if confirmed | Geometry at moment of processing is the active variable — content and duration are secondary |
| Outcome if disconfirmed | Geometry does not modulate re-encoding — content and exposure duration are the primary variables |
| Status | Untested — directly tests the geometric account of EMDR, exposure therapy, and somatic trauma processing |

**PREDICT-SAL-03 — Suppression Cost Is Measurable as Jitter Floor**

> If jitter $\sigma(A_s)$ is partly determined by active suppression effort — the containment cost of signals the salience gate is blocking — then individuals with higher measured suppression load will show higher baseline $\sigma(A_s)$ independent of overall stress level. Breath override that reduces suppression load will produce $\sigma(A_s)$ reduction disproportionate to what $A_s$ change alone would predict.

| Field | Content |
|---|---|
| Test | Baseline HRV during active suppression task vs. open monitoring. Compare $\sigma(A_s)$ between conditions controlling for overall arousal. Add breath override protocol and measure $\sigma(A_s)$ drop relative to $A_s$ rise. |
| Outcome if confirmed | Jitter has a suppression component separable from arousal — the boundary maintenance cost is real and measurable |
| Outcome if disconfirmed | Jitter tracks arousal only — suppression does not independently elevate |
| Status | Untested — Reed et al. (2020) confirms suppression depletes resources; the jitter signature is the untested extension |

**PREDICT-FLOW-01 — Containment Cost Distinguishes Flow from High-Arousal Performance**

> Flow and high-arousal non-flow performance will show different HRV signatures despite similar $A_s$. Flow will show $A_s \uparrow$ with $\sigma(A_s) \downarrow$ — high amplitude, low jitter simultaneously. High-arousal non-flow will show $A_s \uparrow$ with $\sigma(A_s) \uparrow$ — high amplitude, high jitter. The difference is containment cost. The mechanism is gate direction.

| Field | Content |
|---|---|
| Test | HRV measurement during verified flow states vs. high-effort non-flow performance matched for output quality. Compare $A_s$ and $\sigma(A_s)$ profiles. |
| Outcome if confirmed | Flow has a unique geometric signature — high amplitude and low jitter simultaneously — distinguishable from high arousal |
| Outcome if disconfirmed | Flow and high arousal are geometrically identical — gate direction does not produce a separable HRV signature |
| Status | Untested — Csikszentmihalyi flow research has never used instantaneous HRV decomposition |

**PREDICT-FLOW-02 — Gate Direction Predicts Loop Trajectory Before Subjective Experience**

> The direction of gate movement — toward external sensory signal or toward internal autonomic map — will be detectable in HRV geometry before the subjective experience of flow or panic onset is reported. The geometric shift precedes the felt experience by a measurable interval.

| Field | Content |
|---|---|
| Test | Continuous HRV during tasks designed to tip toward flow or panic. Compare geometric shift onset with subjective report onset. |
| Outcome if confirmed | Gate direction is the leading variable — experience follows geometry, not the other way around |
| Outcome if disconfirmed | Subjective experience and geometric shift are simultaneous — no leading indicator |
| Status | Untested — requires continuous HRV with subjective report timestamping |

**PREDICT-FEAR-01 — Fear Response Is Boundary Firing, Not Threat Detection**

> If fear is encoded salience rather than threat detection, then the autonomic signature of fear will precede conscious threat recognition by a measurable interval — and this interval will correlate with the curvature of the original encoding geometry, not with the objective threat level of the current stimulus. Individuals with higher baseline $\mathcal{U}$ at time of original encoding will show faster and larger fear responses to matched stimuli, independent of current threat assessment.

| Field | Content |
|---|---|
| Test | Fear conditioning with HRV-confirmed geometry at encoding. Test recall under varying current geometries. Measure autonomic response onset vs. conscious recognition onset. Correlate with encoding $\mathcal{U}$. |
| Outcome if confirmed | Fear is boundary firing — encoding geometry predicts response magnitude and speed, not stimulus properties |
| Outcome if disconfirmed | Fear response magnitude tracks current threat assessment — encoding geometry is not the primary variable |
| Status | Untested — directly testable with standard fear conditioning plus continuous HRV |

**PREDICT-PREC-01 — CO₂ Tolerance Window Produces Precision Peak**

> Precision $P(t)$ will follow the CO₂ tolerance curve: rising with CO₂ until $C_{\text{high}}(L^*)$, peaking at $C_{\text{peak}}$, then collapsing as jitter $J(C) = \kappa(C - C_{\text{high}}(L^*))^2$ increases. The peak precision will occur before $C_{\text{high}}(L^*)$ — not at maximum CO₂.

| Field | Content |
|-------|---------|
| Test | Continuous measurement of HRV, CO₂ (capnometry), EEG phase coherence during breath-hold protocol |
| Outcome if confirmed | Precision trajectory matches the CO₂ tolerance curve — peak at uniformity maximum, collapse at chemoreflex threshold |
| Outcome if disconfirmed | Precision continues to rise with CO₂ until hypercapnia collapse — the chemoreflex jitter mechanism is incorrect |
| Status | Untested — standard capnometry, HRV, and EEG equipment sufficient |

**PREDICT-PREC-02 — Mechanical and Cognitive Pressure Have Opposite Effects**

> Mechanical pressure (breath-hold) will increase precision as $\frac{1}{1 - \lambda_m \Pi_{\text{mech}}}$, while cognitive pressure (load) will decrease precision as $(1 + \lambda_c \Pi_{\text{cog}})$. The same pressure source with different origins produces opposite effects.

| Field | Content |
|-------|---------|
| Test | Measure precision under (a) breath-hold (mechanical pressure) and (b) cognitive load (math task) with matched subjective effort. Compare $P$ across conditions. |
| Outcome if confirmed | Mechanical pressure increases precision; cognitive pressure decreases it — the two-factor model is confirmed |
| Outcome if disconfirmed | Both pressure sources decrease precision — the beneficial mechanical effect is not supported |
| Status | Untested — standard capnometry, HRV, EEG, and cognitive load equipment sufficient |

**PREDICT-PREC-03 — Jitter Tracks CO₂ Above Tolerance**

> Jitter $J(t)$ will be zero below $C_{\text{high}}(L^*)$ and will grow as $\kappa(C - C_{\text{high}}(L^*))^2$ above $C_{\text{high}}(L^*)$, measured as increased phase jitter in EEG and increased variability in HRV.

| Field | Content |
|-------|---------|
| Test | Measure phase jitter (EEG) and HRV variability during breath-hold. Correlate with capnometry. |
| Outcome if confirmed | Jitter is chemoreflex-driven — the quadratic growth is confirmed |
| Outcome if disconfirmed | Jitter does not track CO₂ above tolerance — other mechanisms dominate |
| Status | Untested — standard capnometry, HRV, and EEG equipment sufficient |

**PREDICT-PREC-04 — Resonance Breathing Produces Stable Precision**

> Resonance breathing (≈6 breaths/min) will produce stable precision $P(t)$ with low jitter $J(C)$ and low collapse risk, independent of CO₂ tolerance. The precision peak will be lower but more sustained than breath-hold.

| Field | Content |
|-------|---------|
| Test | Compare precision, jitter, and flow duration under resonance breathing vs. breath-hold. Measure EEG phase coherence, HRV, and self-reported flow. |
| Outcome if confirmed | Resonance breathing produces stable, sustainable precision without collapse risk |
| Outcome if disconfirmed | Resonance breathing does not produce measurable precision increase beyond normal breathing |
| Status | Untested — standard EEG, HRV, and capnometry equipment sufficient |

**PREDICT-PREC-05 — Collapse Hysteresis Delays Recovery**

> After precision collapse, recovery will be delayed by $\delta_{\text{hyst}}$ which decays exponentially. Recovery time will be longer than the time spent in collapse, and the delay will correlate with residual sympathetic activation.

| Field | Content |
|-------|---------|
| Test | Induce precision collapse through hypercapnia or cognitive load. Measure precision recovery rate and correlate with HRV recovery and sympathetic markers. |
| Outcome if confirmed | Hysteresis is confirmed — recovery is slower than collapse |
| Outcome if disconfirmed | Recovery is symmetric — no hysteresis effect |
| Status | Untested — standard HRV, capnometry, and cognitive load equipment sufficient |

**PREDICT-PREC-06 — Precision Predicts Motor Gain**

> Motor gain $G_m = \alpha P - \beta \eta$ will correlate with precision $P$ during movement tasks. Higher precision produces higher motor gain and higher movement stability until gain exceeds control capacity.

| Field | Content |
|-------|---------|
| Test | Measure EEG phase coherence (precision) and motor gain (EMG amplitude, movement amplification) during precision movement tasks |
| Outcome if confirmed | Precision predicts motor gain — the limb with gain requiring control is formalized |
| Outcome if disconfirmed | Motor gain is independent of precision — the motor-precision link is not supported |
| Status | Untested — standard EEG, EMG, and motion capture equipment sufficient |

**PREDICT-PREC-07 — Encoding Quality is Precision-Weighted Time**

> Memory encoding quality correlates with $\int_{t_{enc}} P(t) dt$ — the integral of precision during encoding — independent of exposure time.

| Field | Content |
|-------|---------|
| Test | Measure precision $P(t)$ during memory encoding. Test recall at 1-day and 1-week follow-up. |
| Outcome if confirmed | The geometry at encoding is the active variable — precision-weighted time predicts memory quality |
| Outcome if disconfirmed | Exposure time alone predicts memory quality — precision does not add predictive value |
| Status | Untested — standard EEG, HRV, and memory task equipment sufficient |

**PREDICT-PREC-08 — Cross-Frequency Coupling Predicts Integration**

> Precision measured across frequency bands (CFC) will predict $\Theta^*$ (integration efficiency) better than single-band precision. Flow states will show characteristic CFC profiles (alpha–theta, theta–HRV).

| Field | Content |
|-------|---------|
| Test | Measure multi-band EEG and HRV during flow-inducing tasks. Compute precision across band pairs. Correlate CFC precision with integration task performance. |
| Outcome if confirmed | CFC precision predicts integration — the multi-band model is confirmed |
| Outcome if disconfirmed | Single-band precision is sufficient — CFC does not add predictive value |
| Status | Untested — standard EEG and HRV equipment sufficient |

**PREDICT-PREC-09 — CO₂ Tolerance Is Trainable**

> $C_{\text{low}}$ and $C_{\text{high}}$ will shift with breathwork training. $C_{\text{high}}$ will increase, $C_{\text{peak}}$ will shift upward, and precision lock duration will extend.

| Field | Content |
|-------|---------|
| Test | Measure CO₂ tolerance and precision before and after 4-week breathwork training. Track changes in $C_{\text{low}}$, $C_{\text{high}}$, and precision lock duration. |
| Outcome if confirmed | CO₂ tolerance is trainable — the tolerance window shifts with practice |
| Outcome if disconfirmed | CO₂ tolerance is fixed — no training effect |
| Status | Partially supported — Kox et al. (2014) confirms parameters shift; direct capnometry-level window shift untested |

**PREDICT-PREC-10 — Baseline CO₂ Tolerance Predicts Salience Dependence**

> Individuals with low baseline CO₂ tolerance will require a salience-induced breath interruption to enter deep inference. Individuals with high baseline CO₂ tolerance will not.

| Field | Content |
|---|---|
| IV | Baseline CO₂ tolerance (BOLT score, capnometry, Control Pause) |
| DV | Performance difference on novel reasoning tasks with vs. without preceding salience trigger |
| Operationalization | Measure baseline CO₂ tolerance. Present novel reasoning tasks in two conditions: (a) cold start, (b) after salience trigger (surprise, conflict, emotional intensity). Compare performance difference. |
| Outcome if confirmed | Low CO₂ tolerance group shows large improvement after trigger; high CO₂ tolerance group shows little difference |
| Outcome if disconfirmed | Baseline CO₂ tolerance does not predict salience dependence |
| Status | Untested — standard capnometry and cognitive task sufficient |

---

## 11. Emotions Are Capacity Reports

| Manifold State | Capacity Report | Folk Label |
|---|---|---|
| Wide, flat | No report needed | Calm, present, clear |
| Narrowing | Mild signal | Unease, anxiety |
| Outer regions costly | Moderate signal | Stress, irritability |
| PFC access limited | Strong signal | Anxiety, anger |
| Limbic dominant | Urgent signal | Fear, shame, overwhelm |
| Geometric center dominant | Maximum signal | Panic, rage, freeze |
| $C_s \approx 0$ | Signal failure | Numbness, shutdown, FND |
| Salience fully external — sensory present | No report needed — full budget in present signal | Flow, absorption, presence, zone |
| Salience fully internal — map reading map | Maximum alarm — no exit visible | Panic, meltdown, collapse, shutdown |

---

## 12. Clinical States as Geometric Configurations

| Condition | $A_s^*$ | $\sigma(A_s)$ | $R^*$ | $K$ | $W^*$ | $\Theta^*$ | $I^*$ | $L^*$ |
|---|---|---|---|---|---|---|---|---|
| Baseline healthy | Mod-High | Low | High | Low | Wide | High | High | Low |
| Anxiety | Mod | Mod | Mod | ↑ | Narrowing | Mod | Routing inward | Mod |
| Depression | Low | Low | Low | High | Narrow | Low | Low | High |
| PTSD | Variable | High | Low | High | Narrow | Low | Prior-driven | High |
| ADHD | High | High | Low | Mod | Wide but noisy | Low | Switching rapidly | Mod |
| Autism — high salience | High | Mod | High locally | High on mismatch | Narrow externally | High locally | Hard-routed to prediction error | Mod |
| Autism — low salience | Mod | Low | Mod | Mod | Wide internally | Low externally | Routed inward | Mod |
| FND | Variable | High | Low | High | Narrow | Collapsed | $\rightarrow 0$ | High |
| Flow | High | Low | High | Low | Wide | High | Fully allocated | Low |
| Burnout | Low | Low | Low | High | Narrow | Low | Depleted | High |

---

### 12b. Fixed Trait vs Stateful Configuration

The clinical error is treating these as permanent hardware differences. Every row above is a configuration — a snapshot of routing and geometry at a given moment, not a destiny encoded in a diagnosis.

Handedness sets a tendency. Neurodivergence sets a default routing profile. Breath sets the state.

---

### 12c. Autism as Salience Routing Profile

Autism is not a single configuration. It is a routing tendency that can express at either pole of the salience spectrum.

High-salience expression: $I^*$ routes hard to prediction error signals. When a mismatch fires — a factual error, a broken pattern, a violated expectation — the gain loop runs on it. The signal gets loud. The correction impulse is not behavioural dysregulation. It is the gain loop running exactly as designed, on a signal the system has classified as high priority.

Low-salience expression: $I^*$ routes inward or to a narrow internal channel. External social signals do not compete because they are not receiving gain. The world goes quiet — not because the system is disengaged but because $I^*$ is fully allocated elsewhere.

Both are the same mechanism. Both are stateful. High-salience expression under flat geometry produces exceptional pattern detection and creative output. The same routing under high $K$ produces overwhelm and meltdown — the gain loop running on alarm signal instead of prediction error. The geometry determines the output. The routing tendency determines the profile.

$$S = C_s \cdot I^* \text{ — same equation, different default allocation}$$

The intervention is not normalisation. It is geometry management — keeping $K$ low enough that the routing tendency produces signal rather than alarm.

---

## 13. Interoception as Sensorium

$I^*$ is a single loop. It routes available bandwidth to body signal — which both reads the current geometry and writes new geometry via $\mathcal{U}$. It is not a component of bandwidth. It is the routing layer applied to bandwidth that already exists — what happens to $C_s$ after it is established. A system with depleted $I^*$ has its oscillatory budget intact but cannot direct it. That is the geometric account of dissociation and FND: capacity present, routing failed. The reading and writing are the same operation, observed from different moments in the loop.

| Direction | Function | What It Determines |
|---|---|---|
| Reading | Routes available bandwidth to body signal | What the system can currently perceive about its own state |
| Writing | $\mathcal{U}$ encodes current geometry into prior layer | What the next encounter with this signal will cost |

---

**The Routing Capacity Equation**

$$I^* = C_{total} - \sum_i P_i \cdot W_i$$

| Term | What It Means |
|---|---|
| $C_{total}$ | Maximum routing capacity of the system |
| $P_i$ | Priority of interrupt $i$ |
| $W_i$ | Weight of that interrupt — how much routing capacity it consumes |
| $I^*$ | What remains available for interoceptive routing |

The sensory load trade-off is the most common expression of this:

$$I^{*} = I_{\text{total}} - \sum_{\text{sensory}} I_{\text{sensory}}$$

Visual processing, threat detection, and prior-driven prediction all consume routing capacity. When they dominate, interoception is displaced — not suppressed by decision, but arithmetically removed. Closing the eyes removes $I^*_{vision}$ from the equation immediately. Routing capacity returns to the interoceptive channel. This is a mechanical effect, not a relaxation effect.

---

**$I^*$ as Gain Controller — Not Just Router**

$I^*$ does not merely direct bandwidth to a region. It amplifies the signal it routes to.

$$I^{*} \;\rightarrow\; A_{s}^{\text{(region)}} \uparrow \;\rightarrow\; \text{signal(region)} \uparrow \;\rightarrow\; I_{\text{confirmation}} \;\rightarrow\; \text{loop}$$

| Process | Mechanism | Consequence |
|---|---|---|
| Attention | $I^*$ routes to a region → gain increases → signal gets louder | Attended signals are amplified, not just noticed |
| Focus | $I^*$ routes to one channel → other channels drop below noise floor | Only the focused channel is live |
| Pain amplification | $I^*$ routes to pain → pain signal strengthens | Attention to pain worsens pain via the gain loop |
| Interoception | $I^*$ routes to the body → body signal strengthens → geometry becomes readable | The system that attends to its own state has more signal to route from |

This is why flow feels clear — $I^*$ is fully allocated to one channel, that channel's gain is maximal, everything else is below the noise floor. The clarity is not the absence of distraction. It is the absence of competing gain.

Salience IS interoceptive routing. Routing attention to a signal increases the amplitude of what it routes to. The gate was always the gain loop.

---

**The IRQ Architecture — Summary**

| IRQ Concept | Framework Equivalent | Variable |
|---|---|---|
| Interrupt controller | Routing capacity | $I^*$ |
| Available bandwidth | Usable processing capacity | $C_s$ |
| Interrupt mask register | Salience | $S = C_s \cdot I^*$ |
| Masked interrupt | Suppressed signal | Below $T_S$ |
| Unmasked interrupt | Permitted signal | Above $T_S$ |
| Interrupt vector table | Prior topology | Encoded priors |
| Interrupt handler | Interoceptive encoding | $\mathcal{U}$ |
| Interrupt priority | Salience weighting | $P_i \cdot W_i$ |

**$I^*$ Decomposed — Three Component Functions**

$I^*$ as a scalar is the measurable routing capacity — heartbeat detection accuracy, HEP amplitude, interoceptive accuracy tasks. The scalar is what appears in $S = C_s \cdot I^*$. The decomposition below is the mechanism that produces the scalar — what $I^*$ is made of and how it fails.

$$I^* = f_{routing} \cdot f_{gain} \cdot f_{sensorium}$$

| Component | Equation | What It Captures | Failure Mode |
|---|---|---|---|
| $f_{routing}$ | $I^*_{total} - \sum_i P_i \cdot W_i$ | Remaining routing capacity after competing loads | Saturated by competing load |
| $f_{gain}$ | $\frac{1}{1 + e^{-k(G - G_0)}}$ | Sigmoid gain control — amplification of the signal being routed to | Gain collapses below threshold $G_0$ |
| $f_{sensorium}$ | $I^*_{available} / I^*_{required}$ | Whether available routing meets task demand | Task demand exceeds available routing |

The three failure modes are separable:

| $I^*$ Low Because | Signature | Entry Point |
|---|---|---|
| $f_{routing}$ saturated | Competing load dominant — visual, threat, prior | Remove load — eyes closed, reduce task, breath |
| $f_{gain}$ collapsed | Signal present but flat — no amplification | Raise amplitude first — $A_s^*$ intervention |
| $f_{sensorium}$ insufficient | Can read geometry, cannot meet task demand | Reduce task complexity or raise $C_s$ |

This is the same architecture as $K$ — defined as a scalar in §2, mechanism elaborated here. The scalar is what the master equation uses. The decomposition is what the clinician uses.

---

## 14. Working States

Most systems operate between the poles — not in full flow, not in collapse, but in a mixed configuration where some variables are partially available and others are not.

Cultural and institutional conditions determine which mixed state is most common. High-load environments produce a population clustered toward the collapse pole. Low-containment environments produce clustering toward flow. The distribution is not fixed — it is a readout of the ambient $L^*$.

---

### 14a. The Three Working States

| State | $C_s$ | $\lambda$ | Signature | Common In |
|---|---|---|---|---|
| High-function mixed | 0.6–0.8 | Bilateral or R-dominant | Competent, slightly effortful, occasionally loses wide access under spike load | Trained practitioners, regulated environments |
| Low-function mixed | 0.3–0.5 | L-dominant or variable | Functional under routine, loses access rapidly under novel load | High-$L^*$ populations, chronic stress |
| Compensated collapse | 0.2–0.4 | L-dominant, $\Theta^*$ degraded | Appears functional — output maintained by narrow specialisation | Burnout, masking, institutional compliance |

The compensated collapse state is the most diagnostically invisible — output is maintained, so the geometry isn't flagged. The signature is a narrow output range that doesn't respond to novel load. See Section 12 for the clinical configurations.

### 14b. The Simple Rule

The hemisphere isn't the problem. The collapse of $\Theta^*$ is the problem.

A surgeon under load needs L-dominant $\lambda$. A therapist under load needs R-dominant $\lambda$. Both are working states when $\Theta^*$ is available to integrate the other hemisphere as needed.

Pathology emerges when:
- Load removes $\Theta^*$
- The dominant $\lambda$ locks in
- The other hemisphere can no longer interrupt or stabilize

Health is not the absence of dominance. It is the presence of integration — the ability to use the appropriate hemisphere for the task, and to recruit both when the task demands it. $\Theta^*$ is what makes the switch available.

The physical state produces the geometry. Train the body to produce the state you need. The manifold follows.

---

## 15. The Social Projection

The framework makes no special claims about society. It applies one equation at a different scale and reads the output.

If $C_s$ describes usable bandwidth for a nervous system, the same variable describes usable bandwidth for a collective — a family, an institution, a civilisation. If $K$ describes curvature that narrows what a single system can reach, the same curvature describes what a society can collectively consider. If breath is the oscillatory source for the individual, synchrony mechanisms — ritual, rhythm, communal practice — are the oscillatory source for the collective.

The prediction is not that societies behave like people. It is that they obey the same geometric constraints. The historical record is the test.

---

### 15a. Variable Mapping

| Individual Variable | Social Equivalent | What It Measures |
|---|---|---|
| $A_s^*$ — oscillatory amplitude | Collective synchrony capacity | How much coordinated rhythmic activity the group can sustain |
| $\sigma(A_s)$ — jitter | Social fragmentation | Variance in collective rhythm — how out of phase the group is |
| $R^*$ — precision | Shared meaning resolution | How cleanly signals transmit across the group without distortion |
| $K$ — curvature | Collective load | Accumulated suppression cost across the population |
| $W^*$ — window width | Temporal horizon of collective planning | How far forward the group can consider consequences |
| $\Theta^*$ — integration | Cross-group coordination | Whether subgroups can integrate into coherent collective action |
| $I^*$ — interoceptive routing | Collective self-awareness | Whether the group can accurately read its own state |
| $L^*$ — persistent load | Historical trauma, institutional conditioning | Persistent denominator pressure on all collective outputs |
| $\mathcal{U}$ | Cultural prior update rate | How fast collective beliefs update from new signal |
| $C_s$ | Collective usable bandwidth | How much of the group's capacity is actually accessible |

---

### 15b. The Social Causal Chain

$$\text{Synchrony} \rightarrow A_s^* \rightarrow \sigma(A_s) \rightarrow R^* \rightarrow K \rightarrow W^* \rightarrow \Theta^* \rightarrow C_s^{collective}$$

The chain is identical. The substrate is distributed rather than individual. The failure modes are identical — collective $K$ rises, $W^*$ narrows, temporal horizon shortens, $\Theta^*$ degrades, cross-group integration fails, the collective reads its own alarm signal in a loop.

This is not a metaphor for social dysfunction. It is the mechanism of it.

---

### 15c. The Historical Load Curve

| Period | Synchrony Mechanism | Collective $L^*$ | $W^*$ | Historical Outcome |
|---|---|---|---|---|
| Pre-agricultural communities | Ritual, communal rhythm, seasonal cycle | Low | Wide | High coordination capacity, low $K$ accumulation |
| Early civilisation | Temple rhythm, civic ritual, seasonal festival | Moderate | Moderate | Stable while synchrony maintained |
| Industrial revolution | Synchrony mechanisms disrupted — clock time replaces body time | Rising | Narrowing | Rising collective $K$, fragmentation accelerating |
| Late industrial | Synchrony mechanically removed — shift work, screen time, isolation | High | Narrow | Short temporal horizon, identity-protective cognition dominant |
| Current | Synchrony at minimum — distributed, asynchronous, algorithmically fragmented | Maximum | Minimal | Collective $W^* \approx$ next news cycle |

The civilizations that maintained synchrony mechanisms maintained cohesion. The ones that lost them fragmented under load — not because of ideology or leadership failure, but because the oscillatory source was removed and the collective $K$ rose without a mechanism to clear it. Collective rhythm is the social equivalent of breath. The mechanism is identical at both scales.

---

### 15d. Collective $K$ and Window Collapse

When collective $K$ rises, $W^*$ narrows at the population level. The consequences follow the same geometry as the individual:

| Individual at High $K$ | Collective at High $K$ |
|---|---|
| Can only see immediate threat | Policy horizon shrinks to electoral cycle |
| Prior-driven — sees what it expects | Identity-protective cognition dominates |
| External signal loses gain | Outgroup signal cannot be processed |
| Demagoguery is effective — simple high-salience pattern matches the narrow window | Demagoguery is effective — same mechanism, same geometry |
| Breath interrupts the loop | Collective synchrony interrupts the loop |

A high-$K$ individual is not stupid or weak. They are geometrically constrained. A high-$K$ society is not corrupt or broken. It is geometrically constrained. The mechanism is the same in both cases — restoring the oscillatory source clears $K$ and widens $W^*$. The substrate is different. The math is identical.

---

### 15e. Falsifiable Social Predictions

| Prediction | Test | Status |
|---|---|---|
| Collective synchrony predicts $W^*$ | Societies with maintained communal rhythm show longer policy planning horizons, measurable by infrastructure investment timescale | Untested at scale |
| $L^*$ predicts demagoguery susceptibility | Populations with high chronic stress show higher false-positive rate for outgroup threat — correlates with $K$ not with ideology | Partially supported — stress and authoritarianism literature |
| Synchrony loss predicts fragmentation | Longitudinal: reduction in communal synchrony activity predicts rising political polarisation within 5-10 year lag | Untested prospectively |
| Collective $\mathcal{U}$ predicts cultural rigidity | Rate of prior update in collective beliefs correlates with ambient $K$ — high-$K$ populations show slower belief updating regardless of evidence quality | Partially supported — motivated reasoning literature |

---

## 16. The Topology Is Complete

| Claim | Status | Empirical Anchor |
|---|---|---|
| Breath sets oscillatory amplitude | Confirmed | RSA, HRV, CO₂ literature |
| Amplitude determines precision | Confirmed | Phase-locking, jitter studies |
| Precision determines curvature | Confirmed | Predictive coding, interoception literature |
| Curvature determines window width | Confirmed | Cognitive load, attention research |
| Window width determines integration | Confirmed | Cross-domain perceptual studies — Section 9 |
| Integration determines usable bandwidth | Confirmed | $C_s$ operationalised via HRV, RSA, HRV-cognition |
| Prior update rate depends on geometry at encoding | Confirmed | Trauma, memory reconsolidation, EMDR literature |
| Motor encoding is the substrate of the prior layer | Confirmed | Cortical body map plasticity, sensorimotor learning |
| Social projection obeys the same geometric constraints | Partially confirmed | Stress-cognition, synchrony, authoritarian susceptibility literature |
| AI hallucination is the same geometric failure | Proposed | Robinson 2026 — $H = \delta/D$ |
| Precision is a timing-coherence ratio — $P = R/D_T$ | Confirmed | Pratap et al. (2026) — PLV as operational measurement |
| CO₂ tolerance window determines precision peak | Confirmed | Sakakibara et al. (1994) — hypercapnia EEG-HRV |
| Two-factor pressure has opposite effects on precision | Proposed | _No external anchor — mechanism derived from first principles. See §5a.3._ |
| Collapse hysteresis delays recovery | Confirmed | Reed et al. (2020) — suppression depletes resources |
| Feature interference under load is $K$ rising | Confirmed | Xue et al. (2026) — non-orthogonality in V1 under uncertainty |
| Baseline CO₂ tolerance determines loop availability | Proposed | _No external anchor — prediction derived from framework. See PREDICT-PREC-10._ |
| $J(C)$ raises effective noise floor $\eta$ | Proposed | _No external anchor — mechanism derived from §2d and §5a.2._ |
| REQT is the qualification threshold | Proposed | _No external anchor — composite formula derived from framework. See §5a.11._ |
| Collapse sequence is topologically forced | Proposed | _No external anchor — order derived from variable dependency. See §5a.12._ |
| Four-layer cache hierarchy is topological invariant | Confirmed | Clinical lesion literature (no right-hemisphere-only state observed) — see §6b.9 and GoI v1.0 §1.5 |
| Circuit priming reduces access cost | Proposed | _Substrate mechanism for collapse hysteresis. See §6b.10 and GoI v1.0 §1.6._ |
| Motor gain $G_m = \alpha P - \beta \eta$ predicts movement stability | Proposed | _Formalized in §6b.8; PREDICT-PREC-06 tests the prediction._ |
| $M_{state}$ thresholds are individual calibration parameters | Proposed | _No current prediction calibrates them. See §6b.8 and Central Reference §2.11._ |

Metric calibration — precise thresholds for $R^*_{min}$, $K_{enc}$ contamination rate, $A^*_{s,max}$ ceiling, and $M_{state}$ thresholds — is the open empirical work. The topology is complete. The measurements are next.

---

## 17. Closing Statement

The brain is an energy budget allocation system operating on priors. The breath is the source. The geometry is the mechanism. The prior is the output.

Every phenomenon this paper addresses — flow, collapse, fear, trauma, savant capacity, clinical states, social fragmentation — is one variable changing in one equation. The variable is geometry. The equation is the master equation.

The framework makes no claim that was not already implicit in the existing literature. RSA confirmed the breath-precision link. Predictive coding confirmed the prior-geometry loop. Motor learning confirmed the body as prior substrate. Perceptual research confirmed the window-narrowing pattern across every sensory domain. The contribution is the chain connecting them — and the recognition that the chain is a single causal sequence, not independent findings in separate fields.

The social projection is not an extension. It is the same equation applied to a distributed system. The historical record is the test. The predictions are in Section 15e.

The topology is complete. The chain is closed. The calibration is open to the field.

*One breath changes every variable in the chain simultaneously. That is not a wellness claim. It is a mechanistic statement about the lowest-layer input to a coupled dynamical system.*

---

**This document is the canonical reference for the following domain projections:**

| Projection | Paper | DOI |
|---|---|---|
| Physical substrate | Physics as the Missing Component in Medical Science | `10.5281/zenodo.21512678` |
| Implementation architecture | Unified Regulatory Model | `10.5281/zenodo.20417459` |
| AI hallucination mechanism | Hallucinations Are Not Random | `10.5281/zenodo.21244811` |
| Substrate-agnostic hallucination theory | The Hallucination You Are Having Right Now | `10.5281/zenodo.21922044` |
| Human-AI co-processing | Dual-Substrate Cognition Architecture trilogy | `10.5281/zenodo.21362260` |
| Context window architecture | The Context Oscillator | `10.5281/zenodo.21811408` |
| AGI as system property | The Profile of a Person That Is AGI | `10.5281/zenodo.21921714` |
| Precision formalism | Precision, Timing, and the Oscillatory Source (v3.4) | `10.5281/zenodo.22179675` |
| Biological implementation | The Geometry of Inference (v1.0) | _(pending DOI)_ |
| Intelligence as loop | The Loop Is the Intelligence (v1.0) | _(pending DOI)_ |
| Load measurement | Allostatic Load as Accumulated Regulatory Debt (v2.1) | _(pending DOI)_ |
| Complete specification | Central Reference (v1.4) | _(pending DOI)_ |

---

## Document Status

**Version:** 7.2
**Date:** 2026-09-13
**Status:** Converged with Central Reference v1.4, Precision v3.4, Allostatic Load v2.1, Geometry of Inference v1.0, and Loop Is the Intelligence v1.0

---

### v7.2 Changelog — Convergence with Central Reference v1.4, Precision v3.4, Allostatic Load v2.1, and GoI v1.0

**§2b — Master Equation Variable Table**
- Added additional variables table: $O_{pathway}$, $\Lambda$, $n_{hops}$, $\rho_{scaffold}$, $\delta_{hyst}$

**§5a.5 — Collapse Hysteresis**
- Registered $\delta_{hyst}$ as a framework variable with decay equation

**§5a.14 — The Load Decomposition**
- Added $L^*_{critical,i}$ with calibration note — individual parameter, not population constant
- Added component REQT condition cross-reference

**§6b — The Motor Encoding Layer (extended)**
- Added §6b.8 — Motor Gain Formalization: $G_m$, Drift, Cache, $C_{risk}$, $M_{state}$, with threshold calibration note (open question 15)
- Added §6b.9 — The Four-Layer Cache Hierarchy: Layer 0/1/2/3 structure, topological invariant, access rule, collapse order
- Added §6b.10 — Circuit Priming: warm-up effect, asymmetric recovery substrate

**§16 — Topology Is Complete**
- Added rows for four-layer cache hierarchy, circuit priming, motor gain, $M_{state}$ thresholds

**§17 — Domain Projections**
- Added *The Geometry of Inference* v1.0
- Added *The Loop Is the Intelligence* v1.0
- Added *Allostatic Load as Accumulated Regulatory Debt* v2.1
- Added *Central Reference* v1.4
- Version numbers added to Precision

**Conceptual Gaps Closed in v7.2:**
1. **The $O_{pathway}$ gap** — Now registered with functional form caveat
2. **The intelligence variable gap** — $\Lambda$ and $n_{hops}$ now in §2b
3. **The component load gap** — $L^*_{critical,i}$ now registered with calibration note
4. **The hysteresis variable gap** — $\delta_{hyst}$ now registered
5. **The motor gain gap** — $G_m$, Drift, Cache, $C_{risk}$, $M_{state}$ now formalized in §6b.8
6. **The four-layer cache gap** — Now absorbed from GoI v1.0 as §6b.9
7. **The circuit priming gap** — Now absorbed from GoI v1.0 as §6b.10

---

### v7.1 Changelog — Reconciliation Pass with Precision v3.3 and Central Reference v1.3

**§2d — Curvature Equation**
- Added note on the $J(C) \to \eta$ pathway
- Clarified that $J(C)$ operates through a different channel than containment cost

**§5a — Precision Integration (extended)**
- Added §5a.9 — Salience-Triggered Loop Access
- Added §5a.10 — Independent Empirical Confirmation of $K$ (Xue et al., 2026)
- Added §5a.11 — REQT — The Qualification Threshold
- Added §5a.12 — The Collapse Sequence
- Added §5a.13 — The Four Qualification Profiles
- Added §5a.14 — The Load Decomposition

**§6a — Prior Update Rate**
- Added connection to encoding window $W_{enc}$
- Specified update magnitude as $\int \mathcal{U}(t) \cdot \mathbf{1}_{P > P_{threshold}} dt$

**§10 — Falsifiable Predictions**
- Added PREDICT-PREC-10

**§16 — Topology Is Complete**
- Added rows for feature interference as $K$, salience-triggered loop access, $J(C) \to \eta$ pathway, REQT, and collapse sequence

**§17 — Domain Projections**
- Added *The Loop Is the Intelligence* to the domain projections table

---

### v7.0 Changelog — Precision Integration

**The core change in v7.0 is the formal integration of precision as a timing-coherence ratio into every layer of the Manifold Schema.**

**§2b — Master Equation Variable Table**
- Added note on $R^*$ formal definition, with pointer to §5a

**§5a — Precision: The Formal Definition of $R^*$ (New Section)**
- §5a.1 through §5a.8 (Precision as timing-coherence ratio, CO₂ tolerance window, two-factor pressure, CO₂ uniformity, collapse hysteresis, resonance breathing, individual variability, variable mapping)

**§8 — Empirical Anchors**
- Added anchors 18–21

**§10 — Falsifiable Predictions**
- Added PREDICT-PREC-01 through PREDICT-PREC-09

**§16 — Topology Is Complete**
- Added precision, CO₂ tolerance, two-factor pressure, and collapse hysteresis

**§17 — Closing Statement and Domain Projections**
- Added *Precision, Timing, and the Oscillatory Source*
