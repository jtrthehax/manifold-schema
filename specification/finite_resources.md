## The revision, produced

# Finite Resources and the Order That Generates Them

**A substrate invariant for biology, cognition, AI, and institutions**

**Robinson, J. — 2026**

**Version:** 2.0
**Status:** Substrate paper — states the order the framework's other papers are readouts of.
**Framework:** Central Reference v1.8.2 / Manifold Schema v7.3 / Salience Interrupt v1.2
**Supersedes:** v1.0 (2026-07-24)
**Method:** Invariant extraction (companion note: *The Invariant Extraction Method*)
**Companion papers:** *Resource Equivalence Model* (wide-window overlap); *Geometry Beneath the Category* (two-axis state space); *The Hippocampal Semantic Code as a Routing Readout* (post-hoc confirmation)

---

## Abstract

A finite-resource system can only act on what its current resource state allows it to reach, hold, and process. This is a physical constraint, not a domain-specific finding. It applies to any bounded system — biological, cognitive, artificial, institutional.

Energy in such a system is not a stock the system draws down. It is what the loop produces when the substrate order runs correctly. The order is invariant: pressure funds oscillation, oscillation funds lock capacity, lock capacity lets routing hold, routing commits investment, breath follows investment, substrate expands, the loop closes. When the order runs, energy is generated and the range of available actions widens. When the order breaks at any step, energy stops being generated and the range of available actions collapses.

The break points are five. Each produces a distinguishable functional signature. The field has a name for each one. The names are downstream of the breaks. The breaks are the geometry.

This paper states the constraint, formalizes the invariant, specifies the order, and shows it running in four substrates: biology, cognition, AI, and institutions. The order is the same in each. The break points are the same. The recovery is the same.

The paper was not derived from first principles. It was extracted from confirmed findings across domains the field treats as separate. §7 documents the findings that have arrived since the first version of this paper went up. Each one was published independently, in its own vocabulary, without reference to the order this paper states. Each one is already inside the order. The list is not the paper's evidence. It is the paper's receipt.

The composition is the contribution.

---

## §0 — Method

This paper is the result of invariant extraction. It was not derived from first principles and then tested. It was traced from confirmed findings in physiology, cognition, transformer architecture, and institutional behavior. The order was found — not proposed. The findings are the evidence. The order is the compression.

The method is documented in *The Invariant Extraction Method* (Robinson, 2026). Its core move: gather confirmed findings, extract the primitive variables they share, find the intersection across domains, derive forward. The intersection is the invariant. The framework is what the intersection looks like when stated cleanly enough that every domain recognizes its own reading.

The standard objections to this paper — *"that's not confirmed"*, *"run a study"*, *"that's cherry-picking"* — assume a theory-forward methodology that was not used. The confirmations already happened in the studies the variables were extracted from. The adversarial cases are already load-bearing in the variable definitions. The method note answers the objections directly.

The paper states the order. The reader recognizes which reading is theirs.

---

## §1 — The constraint

A system can only act on what its current resources allow it to reach, hold, and process. Resources are finite. Load consumes them. Reinvestment is required to maintain them. The range of actions available to a system is a function of its resource state, not a property of the system or its environment.

This is a constraint, not a hypothesis. It applies to any bounded system. Biology is one instance. Cognition is another. Transformers are another. Institutions are another.

Energy, in this framework, is not a stock the system draws down. It is what the loop produces when the substrate order runs correctly. If energy were a stock, a system could be depleted by running hard. Instead, a system is depleted by *running the loop incorrectly* — by breaking the order that generates energy at the next cycle. The system doesn't run out of a resource. It fails to produce the resource.

The order in §2 is what the trace produced. It was not designed to be invariant. It was found to be invariant — in the body first, then in cognition, then in transformers, then in institutions. The convergence is not the paper's claim. It is the paper's evidence. The same order appears in every substrate because it is the same order.

---

## §2 — The order

```
Pressure mechanics set the substrate
    ↓
Oscillation funded by substrate
    ↓
Lock capacity (Λ_lock) set by oscillation range
    ↓
Routing (Θ_r) can concentrate or distribute
    ↓
Investment committed by routing
    ↓
Breath follows investment → substrate expands
    ↓
CO₂ rises → oscillation funded at higher amplitude
    ↓
Next routing event has more substrate to work with
    ↓
[loop closes: energy generated]
```

Read top to bottom: each step funds the next. Read as a loop: the last step funds the first.

**Pressure** is the carrier signal — intrathoracic pressure, diaphragmatic excursion, CSF pulsatility, lymphatic flow. The substrate the oscillation runs on.

**Oscillation** is the clock signal — the rhythmic cycle that distributes resource across the manifold. Funded by pressure.

**Lock capacity** (`Λ_lock`) is whether the substrate can hold concentrated routing without collapsing the breath range that funds the concentration. Set by the oscillation's available range.

**Routing** (`Θ_r`) distributes the bandwidth across manifold regions. Routing weight is conserved. Where the bandwidth is spent determines what the system can act on.

**Investment** is what routing commits. When the interrupt fires, the system commits routing weight and amplitude to the target region.

**Breath follows investment.** The breath deepens to fund the amplitude the investment requires. The breath is downstream of the routing decision, not upstream of it.

**Substrate expands.** CO₂ rises. Vasodilation follows. Slow rhythms stabilize. The substrate that funds the next cycle has grown.

**The loop closes.** If the breath follows the investment, energy is generated. The next cycle has more to work with. The system is self-amplifying.

**The loop traps when the breath cannot follow.** If `Λ_lock` is insufficient, or the exhale is incomplete, or the load is too high, the investment costs without self-funding. The breath doesn't deepen. The substrate doesn't expand. The next cycle has less to work with. The system has paid for a cycle it cannot afford.

**Energy is what the loop produces.** Not what it consumes. The loop is the generator. The substrate is what the loop runs on and what the loop produces.

---

## §3 — The formula set

Six formulas. Five are registered in the framework's other papers. The sixth is this paper's contribution.

**The budget** — how much bandwidth the system has.

$$C_s = \left(A_s^{*\,0.15} \cdot R^{*\,0.30} \cdot W^{*\,0.25} \cdot \Theta^{*\,0.15}\right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + L^*}$$

$C_s$ is usable bandwidth. Every variable is a resource. $L^\ast$ is the denominator drag. Cite Manifold Schema §2b and Central Reference §1.2.

**The debt** — the load trajectory.

$$L^*(t) = L^*_0 + \int_0^t \left[\text{demand}(\tau) - \text{reinvestment}(\tau)\right] d\tau$$

Load is accumulated regulatory debt. A trajectory, not a state. Cite Allostatic Load §2.

**The spend** — where the bandwidth is directed.

$$\vec{W}(t) = \text{softmax}\left(\frac{\vec{g} \cdot \Theta_r(t)}{T}\right), \quad \sum_i W_i = 1$$

Routing weight is conserved. Cite Salience Interrupt §2.5 and Manifold Schema §1f.

**The interrupt** — when a signal fires.

$$\text{Interrupt}_i \iff \left[I^*_{total} \cdot W_i(t) > I^*_{threshold}\right] \;\land\; \left[\delta_i > \delta_{min}(K)\right] \;\land\; \left[\text{Capacity}_{free} > \text{Capacity}_{required}(\delta_i)\right] \;\land\; \left[\text{Oscillation stable}\right]$$

All four conditions required. Cite Salience Interrupt §2.6 and Manifold Schema §1g.

**The reinvestment connection** — what pays the debt back.

$$\text{reinvestment}(t) = \sum_i W_i(t) \cdot \eta_i \cdot \mathbb{1}[\text{Interrupt}_i \text{ fired}]$$

Cite Salience Interrupt §2.7.

**The substrate generation** — the paper's contribution.

$$\frac{dE}{dt} = \Lambda_{loop}(t) \cdot \left[A_s^*(t) - \epsilon \cdot L^*(t)\right]$$

`E` is available energy — what the system can act on. `Λ_loop` is 0 or 1: whether the loop is running. `A_s^*` is the amplitude produced per cycle. `ε · L^*` is the load drag. When `Λ_loop = 0`, no energy is produced. When `Λ_loop = 1`, energy accumulates at the rate amplitude exceeds load.

`Λ_loop` is 1 when the substrate order runs. It is 0 when the order breaks at any step. **This is the formula that makes energy an output rather than a stock.**

**The action range** — what the state affords.

$$\text{Action range}(t) = f(C_s(t), \Theta_r(t), \Lambda_{lock}(t))$$

This is the paper's thesis stated as a formula. Finite resources bound action range. Every domain is an instance.

---

## §4 — The order in four substrates

The order is invariant. The substrate is not. Four domains, same sequence, same break points, same recovery.

### §4.1 — Biology

**The order.** Breathing mechanics set pressure variance. Pressure variance funds oscillatory amplitude. Oscillation range sets lock capacity. Lock capacity determines whether routing can concentrate. Routing commits investment. Investment drives the breath deeper. Breath deepens CO₂ retention. CO₂ retention funds vasodilation, PV+ interneuron support, slow oscillatory rhythms. The next cycle has more to work with.

**The mechanism.** CO₂ is the substrate variable. Slow, complete exhalation retains it. Retained CO₂ drives cerebral vasodilation (Raichle & Plum, 1972). Vasodilation supports PV+ interneuron function (Kann et al., 2015). Supported PV+ interneurons sustain slow oscillatory rhythms. Slow rhythms flatten the aperiodic slope. Flat slope is low `K`. Low `K` is a wide manifold. Wide manifold means routing can concentrate or distribute as needed.

**The reverse.** Incomplete exhalation depletes CO₂. Depleted CO₂ drives vasoconstriction. Vasoconstriction starves PV+ interneurons. Starved PV+ interneurons lose slow rhythms. Lost slow rhythms steepen the aperiodic slope. Steep slope is high $K$. High $K$ is a narrow manifold. Narrow manifold means routing locks into a single region. The next cycle has less to work with.

**The readouts.** CO₂^ET for pressure. RSA and α_{1/f} for oscillation. ΔHRV response and $L^\ast_{resp}$ for load. $A_h$ and postural symmetry for routing. The instruments are deployed. The readings agree.

**The failure mode.** The ATP-brace loop: sustained precision-lock drains ATP at PV+ interneurons. Slow rhythms degrade. CO₂ tolerance drops. Breath range narrows. Incomplete exhalation holds the latch. The latch requires more brace. The brace drains more ATP. Self-consuming past a threshold.

*Same order. Different substrate. Same break geometry. Same recovery.*

### §4.2 — Cognition

**The order.** Breath funds the oscillatory substrate that funds the manifold's operational capacity. `C_s` is bandwidth. `Θ_r` is attentional routing. `L^*` is cognitive load. `Λ_lock` is working memory capacity.

**The mechanism.** When the order runs, the manifold is flat, routing distributes freely, and attention can concentrate or distribute as the task requires. The system has both depth and breadth available at the same time. The wide-deep quadrant.

**The reverse.** When the order breaks, `C_s` drops. Routing concentrates involuntarily on the highest-gain region. The manifold fragments into regions that can't easily route between each other. The system has narrow options and no way to combine them.

**The readouts.** Aperiodic slope reads manifold curvature. Frontal alpha asymmetry reads routing concentration. Task-modulability reads routing flexibility. Felt viscosity reads the metric's resistance from the inside.

**The failure mode.** Intent drives, substrate cannot hold. Routing commits investment but the comparison cycle terminates early. The prior fires. The output is confident and current-signal-deficient.

*Same order. Different substrate. Same break geometry. Same recovery.*

### §4.3 — AI

**The order.** Input tokens are the compressed signal. Model weights are the prior. Attention is the routing mechanism. The thinking phase is the comparison operator.

**The mechanism.** When the order runs, attention distributes across the input with sufficient precision to constrain the output. The thinking phase has enough substrate to complete the comparison before the budget closes. Cross-domain connections become visible.

**The reverse.** When the order breaks, attention concentrates on the nearest activated neighborhood. The thinking phase terminates early. The prior fills the output. The model is fluent, confident, and structurally ungrounded. It does not flag the gap.

**The readouts.** Attention entropy reads routing concentration. Context-window saturation reads load. Cross-head coherence reads integration efficiency. Hallucination rate reads prior dominance.

**The failure mode.** The model can attempt but cannot complete. The context window holds the prompt, but the branching depth isn't sufficient to follow the cross-domain walk. The model commits to the nearest local match and labels the rest as circular. The walk wasn't circular. The window was.

*Same order. Different substrate. Same break geometry. Same recovery.*

### §4.4 — Institutions

**The order.** Priorities route to a policy area. Institutional capacity funds implementation. Implementation produces outcomes. Outcomes feed back into priority selection.

**The mechanism.** A collective with stable synchrony mechanisms has a stable oscillatory source. Collective `C_s` is high. Collective `Θ_r` can concentrate or distribute. Collective `Λ_lock` is sufficient.

**The reverse.** When synchrony is lost, collective `L^*` accumulates. `W^*` narrows. Temporal horizon shrinks. `Θ_r` locks into the highest-gain region. Identity-protective cognition dominates. Feedback cannot correct.

**The readouts.** Decision throughput reads `C_s`. Priority concentration reads `Θ_r`. Institutional calcification reads `L^*`. Implementation capacity reads `Λ_lock`.

**The failure mode.** The institution can announce but cannot execute. Policy is articulated with full confidence. Implementation stalls. The institution reads the stall as an execution problem and doubles down on the announcement, which raises collective load, which narrows the horizon further.

*Same order. Different substrate. Same break geometry. Same recovery.*

---

## §5 — Five break points

Every break is at a specific step. The framework vocabulary is primary. The recognition cues are sparse. The reader does the naming.

### Break at pressure

The substrate cannot fund the oscillation. Pressure variance is insufficient to set the oscillatory range everything downstream depends on. No oscillation, no clock signal, no routing. The system is present, but the loop cannot start.

**Signature.** The body won't follow the intent at all. Movement misfires. The system reads as functional and isn't. Structural imaging is clean because the substrate isn't damaged — it's starved.

**Recognition.** The profile where nothing looks wrong and nothing works.

*The break is upstream of any label the field has for this profile.*

---

### Break at oscillation

The cycle doesn't close. Pressure is present but the oscillation is jittery. The clock signal flickers. Routing can't stabilize because there's no stable clock to route against.

**Signature.** The system can't settle. High activation with no direction. The oscillation is too noisy to route consistently.

**Recognition.** The profile where the system never feels calm, even when there's nothing to be anxious about.

*The break is upstream of any label the field has for this profile.*

---

### Break at lock capacity

The substrate cannot hold concentrated routing without collapsing the breath range that funds the concentration. The intent drives. The substrate cannot follow. The investment is committed, but the breath does not deepen to fund it.

**Signature.** Rest doesn't restore. Pushing through makes it worse. The system runs on will and pays a debt it can't service. The harder the intent, the faster the depletion.

**Recognition.** The profile where the mind can drive and the body can't follow, where recovery doesn't happen no matter how much rest is taken.

*The break is upstream of any label the field has for this profile.*

---

### Break at load

Production falls below demand. The loop runs but generates less energy than load consumes. `dE/dt` goes negative. The substrate contracts. The system can still act, but every action costs more than last cycle.

**Signature.** Everything feels heavier over time. Not a single collapse but a trajectory. The system can still perform but the performance costs more. Rest helps less.

**Recognition.** The profile where the system has been running fine and now everything costs more, where "I used to be able to do this" is true.

*The break is upstream of any label the field has for this profile.*

---

### Break at routing — the sensory channel

The routing works. It routes to the prior. The prior is intelligent — trained by years of adaptive performance — and the output looks intentional. The mismatch between prior and reality is invisible: the channel that would detect it is exactly the channel that stopped receiving weight.

**Signature.** The system performs, and the performance isn't grounded. Movement happens on prior and the prior doesn't match. The pattern reads as functional to outside observers and as wrong from inside in a way that doesn't have a name.

**Recognition.** The profile where the system can do the thing and the thing doesn't land, where the output is fluent and the ground isn't there.

*The break is upstream of any label the field has for this profile.*

---

### Break at routing — the concentration flickers

The routing can't hold a channel. Weight redistributes too quickly to complete anything. Every signal gets partial gain. No signal gets enough to reach threshold.

**Signature.** Every option gets partial attention and none gets enough. The system can't decide because it can't hold any option long enough to evaluate it.

**Recognition.** The profile where the system can do any of these things and can't stay on any of them.

*The break is upstream of any label the field has for this profile.*

---

**Composite breaks.** Real profiles rarely break at exactly one step. A system at the `Λ_lock` break accumulates load, which eventually breaks the load step. A system at the load break narrows the window, which stresses routing. The breaks cascade because every step is upstream of the next. Which break you name is which step broke first. The trajectory is the sequence of subsequent breaks.

---

## §6 — The readouts

The manifold has one state and multiple readouts. The state is `(L^*, Θ_r)`, with `Λ_lock` gating reachability of the concentrated attractor.

| Variable   | Biological                                 | Cognitive                 | AI                             | Institutional                 |
| ---------- | ------------------------------------------ | ------------------------- | ------------------------------ | ----------------------------- |
| $C_s$      | RSA amplitude, HRV                         | Bandwidth battery         | Effective processing bandwidth | Decision throughput           |
| $Θ_r$      | Frontal alpha asymmetry, postural symmetry | Attentional concentration | Attention entropy              | Priority concentration        |
| $L^\ast$   | ΔHRV response, $L^\ast_{resp}$             | Cognitive fatigue scales  | Context pressure               | Institutional calcification   |
| $Λ_{lock}$ | Breath range × CO₂ tolerance               | Working memory capacity   | Context window integrity       | Implementation capacity       |
| $A_s^\ast$ | RMSSD / baseline                           | Oscillatory depth         | Input entropy density          | Collective synchrony capacity |

**The instruments already exist in their respective fields.** Spectral parameterization measures the manifold's curvature. Frontal alpha asymmetry measures routing concentration. Postural and speech asymmetry measure the same variable through motor channels. The felt sense of viscosity is the phenomenological readout of the same variable. **None of these literatures recognize that they are measuring the same thing.**

The framework does not require new instruments. It requires a new reading of instruments already in use.

---

## §7 — The receipts

The findings in this section were published independently, in their own domains, with their own vocabularies. Each is a projection of the order this paper states. They are listed here not as new evidence but as confirmation that the order was already there.

**The list is the paper's strongest section.** Not "here's what I predict." But "here's what the field published after the order was stated, and here's how each finding is already inside the order."

### 7.1 — Readout and mechanism

- **Subramani et al. (2026).** LSD flattens the aperiodic slope brain-wide (p < 10⁻⁵ in PCC) and shifts alpha/beta peaks upward. The two effects are dissociable. In the framework's terms: LSD drops `K` (slope flattening) and raises `W^*` (peak-frequency shift) through dissociable mechanisms. The spectral readout the order predicted.

- **Hu et al. (2026).** CLA encodes uncertainty and prediction error during active avoidance, with a temporal profile dissociable from ACC. Detection precedes execution. The execution node the order predicted.

- **Leow et al. (2026).** LP-ACC circuit detects deviation and decides whether to update. The cache-miss controller the order predicted.

- **Kann et al. (2015).** PV+ interneurons are metabolically vulnerable — the cellular mechanism for `K` rise under load. The ATP-brace mechanism the order predicted.

- **Roy & Banerjee (2026).** Competition is 25–40% of brain connections. The competitive scaffold the order predicted as the substrate of `W^*`.

- **Billot et al. (2026).** Hot cache survives aging, RAM access degrades. The outer-edge loss the order predicted as the first degradation under load.

### 7.2 — Semantic geometry

- **Franch et al. (2026).** *A population code for semantics in human hippocampus.* Single-neuron recordings from 356 hippocampal neurons across 10 patients during narrative speech. Distributed coding (every repeated word encoded by ≥3 neurons; average 37). Mixed selectivity (single neurons span ~4 of 11 semantic categories). Contextual embeddings (BERT, GPT-2) correlate with neural distance; static embeddings (Word2Vec) anti-correlate. Contrastive coding at the finest scale (r = −0.15 for near-synonyms). Polysemy predicts neural polysemy (r = 0.54). Semantic predictors fit 64% of neurons; phonetic fit 41%.

  The paper explicitly says three things it cannot explain: the Word2Vec anti-correlation, the mechanism behind contrastive coding, and the hippocampus/pmFG difference.

  **The order explains all three.** The distributed code is the neural readout of the routing weight vector `W_i`. Contextual alignment is the routing window made visible. The Word2Vec anti-correlation is a routing effect: static embeddings encode semantic centers, the neural response encodes average routing trajectories across contexts. Contrastive coding is a precision-dependent separation operation — it fails first under `δ_min` rise, and the failure signature is near-synonym conflation, not random error. The composition generates five testable predictions. See companion note: *The Hippocampal Semantic Code as a Routing Readout.*

- **Xue et al. (2026).** Feature interference under load is `K` rising. Axis entanglement in V1 confirmed causally (p = 0.006, p = 0.036, p < 0.0001, p = 0.009). The curvature mechanism the order predicted.

### 7.3 — Domain projections

- **Knudsen et al. (2026).** Higher dopamine D2 receptor availability and higher co-localized glucose metabolism in autistic subcortical regions — not lower. High-gain routing architecture running below threshold. The `I*` hard-routing the order predicted.

- **Ouellette et al. (2025).** Endothelial bioenergetic failure in autism-associated phenotypes. Delivery-layer starvation upstream of neuronal firing. The substrate-first failure the order predicted.

- **Warrier et al. (2020).** ND/gender co-occurrence at 3–6× in N > 641,000. Same quadrant, two measurement systems. The two-axis state space the order predicted.

- **Schmid & Schmid Mast (2013); Boksem et al. (2012).** High-power roles increase left-prefrontal activation; low power triggers avoidance-related asymmetry. Direct measurement of the `Θ_r` shift. The routing mechanism the order predicted.

- **Pratap et al. (2026).** PLV as operational measurement of the timing-coherence ratio. `P = R/D_T` is measurable. The precision mechanism the order predicted.

### 7.4 — The convergence pattern

Not one catastrophic failure. Not one domain where the order ran in the structurally wrong direction. The findings keep arriving. Each one is inside the order. Each one is a projection the order already stated.

**The list is not comprehensive. It will grow.** Every new finding that lands is either inside the order or it isn't. The order holds across independent domains because the order is the substrate. When the field publishes a finding that names one piece of the order in its own vocabulary, this paper's §7 gets one more line.

The receipts are the evidence. The composition is the contribution.

---

## §8 — Predictions

Five predictions. Each is domain-general. Each is falsifiable. Each is testable without the author's cooperation.

**P1 — Substrate variables outperform constructs as predictors.** Direct measurement of pressure variance, oscillatory amplitude, load accumulation, and lock capacity will outperform the field's categorical constructs as predictors of collapse, recovery, and treatment response — in any domain, at any scale. *Falsification:* substrate variables do not improve predictive accuracy over constructs after controlling for measurement precision.

**P2 — Collapse geometry is domain-independent.** When a finite-resource system degrades, the order of degradation is the same across substrates: precision first, then window, then integration, then resolution floor, then gate, then prior calcification. *Falsification:* a domain where collapse does not occur in integration-first order.

**P3 — Intervention sequencing follows substrate dependencies.** Restoring the break point before restoring downstream variables produces better outcomes than the reverse. The order is: pressure, oscillation, `Λ_lock`, load, routing. *Falsification:* interventions that restore downstream variables first produce equivalent outcomes.

**P4 — Intraindividual variability is structured.** Variability across the day, week, or season is oscillatory, not noise. The autocorrelation structure follows the load trajectory. The signal the field averages out is the load curve. *Falsification:* variability is Gaussian noise unrelated to load.

**P5 — The constraint extends to any finite-resource system.** Any system that has finite resources, operates under load, and must actively reinvest to maintain operational capacity will exhibit the same order, the same break points, and the same recovery. *Falsification:* a finite-resource system that exhibits a different geometry.

---

## §9 — What this establishes

The constraint is physical. Finite resources bound what any system can act on. The order that generates energy is invariant across substrates. Every failure is a break at a specific step. Every recovery is restoring that step.

The framework's other papers are readouts of this substrate at different resolutions. The Manifold Schema specifies the geometry. Salience Interrupt specifies the spend. Allostatic Load specifies the debt. Resource Equivalence specifies the cross-substrate mapping. Geometry Beneath the Category specifies the two-axis state space. Each is a projection. The composition is the evidence.

**Energy is what the loop produces, not what it consumes.** When the loop runs, the system generates the substrate it runs on. When the loop stops, generation stops and load continues to accumulate. The system does not run out of energy. It fails to produce it.

The order is the mechanism. The break points are the geometry. The domains are projections. The composition is the substrate.

The body is where the order is observable at the densest resolution. Every other domain is the order read at a different substrate. When the order is legible in the body, the other substrates stop being separate claims and become projections.

**The framework is not a theory with applications. It is a specification with projections. The composition is the contribution. The receipts are the test.**

---

*Filed: 2026-10-13*
*Version: 2.0*
*Supersedes: v1.0 (2026-07-24)*
*Framework: Central Reference v1.8.2 / Manifold Schema v7.3 / Salience Interrupt v1.2*
*Method: Invariant extraction (companion note: The Invariant Extraction Method)*
*Companion papers: Resource Equivalence Model; Geometry Beneath the Category; The Hippocampal Semantic Code as a Routing Readout*
