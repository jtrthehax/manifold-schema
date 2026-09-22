# Central Reference v1.7

**A Unified System Specification for the Loop Framework**

**Robinson, 2026**

**Version:** 1.7
**Date:** 2026-09-20
**Status:** Domain-projection-aligned specification — absorbs the expression/congruence/masking constructs from The Spoken Language Paper v3.1. The speech projection's routing language is now reconciled with the framework's routing decomposition.
**Purpose:** This document is the complete, standalone specification of the loop framework. A reader can use this document alone to understand the system, run the tests, and verify the predictions. Every variable, every equation, and every mechanism that appears in any of the supporting papers is defined here. Future papers should cite Central Reference v1.7 alone.

---

## Changelog — v1.6 → v1.7

This changelog exists so that any reader — human or AI — can see the convergence path. Central Reference v1.6 was the domain-projection-complete specification: it absorbed the general structural lessons from the first full domain projection (The Spoken Language Paper v3.0) — the three axes, the integration-demand rule, the collapse-recovery asymmetry. Central Reference v1.7 is the **domain-projection-aligned specification**: it absorbs the expression/congruence/masking constructs from The Spoken Language Paper v3.1, so that the speech projection's routing language and the framework's routing decomposition are the same system with one name each.

| Step | Change | Source | Location |
|---|---|---|---|
| 1 | Version bumped to v1.7 | — | Header |
| 2 | New variable: \( f_{expression} \) — proportion of salience reaching expression | Spoken Language v3.1 Book I §2.1b | §2.18 |
| 3 | New equation: \( S_{expressed} = S \cdot f_{expression} \) | Spoken Language v3.1 Book I §2.1b | §3.19 |
| 4 | New load term: \( \lambda_{mask} \) — load from chronic output management | Spoken Language v3.1 Book III §18 | §4 (glymphatic ODE) |
| 5 | New section: Expression and Congruence | Spoken Language v3.1 Book III §18, Book IV §23.3 | §2.18 |
| 6 | Congruence operationalization registered | Spoken Language v3.1 Book IV §23.3 | §2.18 |
| 7 | §19 updated with \( f_{expression} \), \( \lambda_{mask} \), congruence | — | §19 |
| 8 | §20 updated: historical-name note for speech paper's \( f_{routing} \) | — | §20 |
| 9 | §21 updated: composition question for \( f_{expression} \) | — | §21 |
| 10 | §22 updated: open questions for functional forms | — | §22 |
| 11 | §24 updated: cite Spoken Language Paper v3.1, not v3.0 | — | §24 |
| 12 | §25 updated: projection-layer alignment note | — | §25 |
| 13 | New §26: Speech Projection Alignment (short note) | — | §26 |
| 14 | §27 (formerly §26): The One Line — updated | — | §27 |

**What did not change:** The master state variables, the master equation, the precision formalism, the load decomposition, the causal chain, the four contracts, the collapse sequence (Stages 1–6), the branch condition, the four profiles, the hardware-failure chain, the three axes, the layer stacks, the recovery asymmetry, and all predictions all remain as they were in v1.6, except where explicitly noted below.

**Why this is the right next assembly:** v1.6 registered the general structural rules that the speech projection produced. v1.7 registers the general **variable-level** constructs that the speech projection produced. The three axes were about *shape*; \( f_{expression} \) is about *amount*. The specification is now aligned with its first full projection at both levels.

---

## Part 0 — How to Read This Document

This is a specification, not a paper. It contains:

- **Part I — The System:** The complete set of variables and equations
- **Part II — The Causal Chain:** Every step from breath to behaviour, sourced
- **Part III — The Anchors:** Every empirical anchor, with what it confirms
- **Part IV — The Predictions:** Every testable prediction, with protocol
- **Part V — The Cohesion Check:** Where documents drift, where gaps remain
- **Part VI — Version History**

If you are testing the framework, read Part IV.

If you are building on the framework, read Parts I and II.

If you are evaluating the framework, read Parts III and V.

**For operational application without full technical derivation:** Read §5b (Collapse Sequence and Zone Table), §6 (Four Profiles), and §3.7 (REQT Equation). These three sections are the operational layer — they contain everything needed to apply the framework without working through the full variable and equation registries. The variable registry (§2) and equation registry (§3) are the reference layer and are not required for application.

**For building a domain projection:** Read §2.15 (three axes), §2.16 (layer stacks), §2.17 (recovery asymmetry), §2.18 (expression and congruence), §18b (projection methodology). These five sections contain everything needed to apply the framework to a new domain.

**This document is the single reference.** Every variable, equation, and mechanism in the loop framework is defined here. The supporting papers (Manifold Schema v7.2, Precision v3.4, Allostatic Load v2.1, Geometry of Inference v1.0, Loop Is the Intelligence v1.0) are domain projections. They provide extended derivations, biological implementation detail, and the argued thesis, but they introduce no new variables and no new mechanisms that are not in this document or explicitly delegated by it. See §25 for the full stack.

---

# PART I — THE SYSTEM

## 1. The Definition

**Intelligence is the energy-expensive loop of error detection against sensory input, followed by iterative reinvestment of resources toward structural convergence.**

**Consciousness** is the interpretation of sensory signal. **Intelligence** is the use of that interpreted signal as feedback — the loop.

$$\text{Intelligence} \subset \text{Consciousness}$$

**Wisdom** is the loop's output compressed into the prior:

$$\text{Wisdom} = \int_0^t \text{Intelligence} \, dt \quad \text{compressed into prior}$$

**The definition:**

$$\text{Intelligence} = \Lambda \cdot n_{hops} \cdot R^* \cdot \Theta^*$$

Intelligence has two rate dimensions ($R^*$, $\Theta^*$) and one capacity dimension ($W^*$, which determines $n_{hops}$). $\Lambda$ is the binary indicator of whether the loop is running at all. When $\Lambda = 0$, the product collapses regardless of the other terms — the loop is not running.

- $R^*$ — precision — loop speed
- $\Theta^*$ — integration efficiency — loop depth
- $n_{hops} = \lfloor W^* \cdot \rho_{scaffold} \rfloor$ — how many inference hops are available
- $\Lambda = \Theta^* \cdot R^* \cdot \mathbb{1}[P_{eff} > P_{threshold}]$ — whether the loop is running

**Intelligence = hops × depth × speed, gated by activation.** Loop depth $\Theta^*$ determines integration per hop. Window width $W^*$ determines how many hops are available. Speed $R^*$ determines cycle rate. All three are required. None alone is sufficient. $\Lambda$ is the gate — if the loop is not running, none of the other terms matter.

---

## 2. The Variable Registry

Every variable is defined once. All ratios are normalized to the individual's own baseline unless otherwise noted.

### 2.1 The Master State Variables

| Symbol | Name | Definition | Physical Measurement |
|---|---|---|---|
| $A_s^*$ | Oscillatory amplitude | Energy budget — how much oscillatory signal is available | RMSSD / Baseline RMSSD |
| $R^*$ | Precision | Timing-coherence ratio — signal clarity | $P / P_{baseline}$ where $P = R/D_T$ |
| $W^*$ | Window width | Accessible manifold range | Cognitive flexibility composite / Baseline |
| $\Theta^*$ | Integration efficiency | How well the system holds disparate signals together | Phase-locking stability × ambiguity tolerance / Baseline |
| $I^*$ | Interoceptive routing | Routing protocol — how well the system reads its own geometry | Heartbeat detection accuracy / Baseline |
| $L^*$ | Allostatic load | Cumulative allostatic debt | See §2.10 for full decomposition |

### 2.2 The Derived Variables

| Symbol | Name | Definition |
|---|---|---|
| $C_s$ | Usable bandwidth | Master equation (see §3.1) |
| $K$ | Curvature | $K = k(1/(R^*+\epsilon)) + \sum_i S_i C_i$ |
| $\delta_{min}$ | Resolution floor | $\delta_{min} = \eta/(A_s^* \cdot I^*)$ |
| $S$ | Salience | $S = C_s \cdot I^*$ |
| $P_{eff}$ | Effective precision | $P \cdot O_{pathway} \cdot U_C$ |
| $P_{threshold}$ | Gate threshold | $P_0 - \gamma L^*$ |
| $\Lambda$ | Loop activation | $\Theta^* \cdot R^* \cdot \mathbb{1}[P_{eff} > P_{threshold}]$ |

> **Note on $\Lambda$ operationalization via delta HRV:** $\Lambda$ is measured via the delta HRV response to a standardized slow-breath protocol (Allostatic Load §5c). A system with low accumulated debt shows significant HRV rise under the protocol ($\Delta HRV > 15$ ms); a system at load ceiling shows minimal response ($\Delta HRV < 5$ ms) regardless of resting baseline. This provides a wearable-based probe for $\Lambda$ at population scale. See PREDICT-GATE-01.

### 2.3 The Precision Variables

| Symbol | Name | Definition |
|---|---|---|
| $R$ | Sync duration | Proportion of time two streams remain phase-locked |
| $D_T$ | Timing distance | Average phase difference between streams |
| $P$ | Precision (absolute) | $P = R/D_T$ |
| $C_{low}$, $C_{high}$ | CO₂ tolerance window | Range within which precision rises with CO₂ |
| $C_{high}(L^*)$ | Load-compressed CO₂ ceiling | $C_{high}^0 - \gamma L^*$ — see below |
| $J(C)$ | Chemoreflex jitter | $\kappa(C - C_{high}(L^*))^2$ for $C > C_{high}(L^*)$, else 0 |
| $\Pi_{mech}$ | Mechanical pressure | Beneficial pressure — breath-hold, resonance |
| $\Pi_{cog}$ | Cognitive pressure | Harmful pressure — instantaneous load, sympathetic activation |
| $U_C$ | CO₂ uniformity | $1/(\text{Var}_i[C_i] + \epsilon)$ |
| $\delta_{hyst}$ | Collapse hysteresis | Recovery delay after precision collapse |
| $W_{enc}$ | Encoding window | $\int_{t_{enc}} \mathbb{1}[P(t) > P_{threshold}] dt$ |

> **Note on $L^*$ vs. $\Pi_{cog}$:** These are distinct. $\Pi_{cog}$ is *instantaneous* cognitive pressure — the current draw on the budget. $L^*$ is *cumulative* allostatic load — the integral of $\Pi_{cog}$ over time minus recovery. The relationship is:
>
> $$L^*(t) = \int_0^t \Pi_{cog}(\tau) \, d\tau - \text{recovery}(t)$$
>
> Both appear in the framework. $\Pi_{cog}$ enters the precision equation directly (through $D_T$ and $R$). $L^*$ enters the master equation as the denominator drag. This prevents double-counting: acute load affects precision; chronic load affects bandwidth.

> **Note on $C_{high}(L^*)$ compression:** The CO₂ tolerance window is not fixed. As allostatic load accumulates, the ceiling drops:
>
> $$C_{high}(L^*) = C_{high}^0 - \gamma L^*$$
>
> where $C_{high}^0$ is baseline tolerance and $\gamma$ is the load-compression coefficient. This means the same absolute CO₂ level produces chemoreflex jitter at lower values when load is high. The compression mechanism is what the Control Pause measures clinically: as load rises, CP drops.

### 2.4 The Routing Variables

| Symbol | Name | Definition |
|---|---|---|
| $I^*$ | Routing capacity | $C_{total} - \sum_i P_i W_i$ |
| $f_{routing}$ | Routing component | One of three components of $I^*$; the fraction of available interoceptive signal routed to readout |
| $f_{gain}$ | Gain component | Sigmoid gain control on the routed signal |
| $f_{sensorium}$ | Sensorium component | Available routing / required routing |
| $I^*$ decomposition | Full form | $I^* = f_{routing} \cdot f_{gain} \cdot f_{sensorium}$ |

> **Note on $f_{routing}$:** $f_{routing}$ is the **input-side** routing component. It determines how much of the available interoceptive signal reaches the readout. It is distinct from $f_{expression}$ (§2.18), which is the **output-side** modifier on salience. The two sit on opposite sides of the salience equation: $f_{routing}$ determines how much $I^*$ you have; $f_{expression}$ determines how much of the resulting salience reaches the output.

### 2.5 The Update Variables

| Symbol | Name | Definition |
|---|---|---|
| $\mathcal{U}$ | Prior update rate | $\mathcal{U} = (A_s^* \cdot R^* \cdot \Theta^*)/(1 + \gamma K_{enc})$ |
| $K_{enc}$ | Curvature at encoding | What geometry the prior carries forward |
| $W_{enc}$ | Encoding window | $\int_{t_{enc}} \mathbb{1}[P(t) > P_{threshold}] dt$ |

> **Note on $W_{enc}$ and $\mathcal{U}$:** The prior update magnitude is the product of the rate and the interval:
>
> $$\text{Update} \approx \int_{t_{enc}} \mathcal{U}(t) \cdot \mathbb{1}[P(t) > P_{threshold}] dt$$
>
> High $W_{enc}$ with high $\mathcal{U}$ produces the strongest prior update.

### 2.6 The Structural Variables

| Symbol | Name | Definition | Source |
|---|---|---|---|
| $\rho_{scaffold}$ | Scaffold density | Density of long-range competitive connections | Roy & Banerjee (2026) — ~0.30 |
| $IM$ | Interference metric | Non-orthogonality of task-relevant and task-irrelevant axes | Xue et al. (2026) |
| $\text{Dim}$ | Neural dimensionality | Independent axes available for representation | $W^* \times \Theta^*$ |
| $n_{hops}$ | Inference hops | Multi-hop inferences available before collapse | $\lfloor W^* \cdot \rho_{scaffold} \rfloor$ |

### 2.7 The Prediction-Error Variables

| Symbol | Name | Definition |
|---|---|---|
| $\delta$ | Prediction error | $\delta = \|signal_{current} - prior_{cached}\|$ |
| $\tau_{PE}$ | PE tolerance | How long the system can sustain PE engagement before the threat cascade fires |
| $\sigma_{PE}$ | PE sensitivity | How finely the system detects PE |

### 2.8 The Metabolic Variables

| Symbol | Name | Definition | Source |
|---|---|---|---|
| $\Phi_{PV}$ | PV+ vulnerability | Metabolic vulnerability of PV+ interneurons | Kann et al. (2015) |
| $\Delta CBF/\Delta CMRO_2$ | Metabolic coupling ratio | Blood flow change / oxygen metabolism change | Hutchison & Rypma (2013) |
| $CVR_{max}$ | CVR ceiling | Maximum task-induced metabolic recruitment | CVR literature |
| $O_{pathway}$ | Oxygen pathway integrity | Substrate constraint on gate condition — the physical ceiling on whether precision can translate to loop opening | See note below |

> **Note on metabolic variable pathways:** These variables enter the hardware-failure chain (§7) rather than the equation registry directly. $\Delta CBF/\Delta CMRO_2$ is the mediator in PREDICT-PE-04. $\Phi_{PV}$ sets the metabolic vulnerability floor that determines how fast curvature rises under oxygen delivery failure — it is the cellular mechanism underlying the $R^* \to K$ transition. $CVR_{max}$ is the physical ceiling on $O_{pathway}$ in the gate condition (§3.6). None of these variables are inputs to the master equation — they are the substrate constraints that determine whether the master equation variables can reach their theoretical range.

> **Note on $O_{pathway}$:** $O_{pathway}$ is the physical ceiling on whether precision can translate to loop opening. It is the substrate constraint that determines whether the master equation variables can reach their theoretical range at all. The causal pathway is specified in §7 (hardware-failure chain).
>
> **Functional form:** $O_{pathway} = f(\Phi_{PV}, \Delta CBF/\Delta CMRO_2, CVR_{max})$ — the functional form is not yet specified. The three components are:
> - $\Phi_{PV}$ — metabolic vulnerability of PV+ interneurons (how fast oxygen delivery failure translates to curvature rise)
> - $\Delta CBF/\Delta CMRO_2$ — metabolic coupling ratio (whether blood flow increase matches metabolic demand)
> - $CVR_{max}$ — cerebrovascular reactivity ceiling (the physical limit on task-induced recruitment)
>
> Declaring the dependency here is honest — the three components are established in the literature, but their combination into a single $O_{pathway}$ scalar requires calibration. Empirical work: measure $O_{pathway}$ under controlled metabolic load, correlate with the three components, and fit the functional form.

### 2.9 The Qualification Variables

| Symbol | Name | Definition |
|---|---|---|
| $REQT$ | Qualification threshold | Minimum regulatory state for loop to run |
| $L^*_{threshold}$ | Load ceiling | Maximum sustainable load before gate degrades |
| $L^*_{critical,i}$ | Component critical load | Threshold value for component $i$ of the load decomposition |
| $\tau_{threshold}$ | PE tolerance threshold | Individual calibration parameter (PREDICT-PE-01) |
| $K_{critical}$ | Curvature critical value | Individual calibration parameter (PREDICT-PE-02) |
| $n_{hops,min}$ | Minimum hop count | Domain-specific floor — problem complexity |
| $\delta_{hyst}$ | Collapse hysteresis | Recovery latency after precision collapse |

> **Note on $\tau_{threshold}$ and $K_{critical}$:** These are individual parameters requiring empirical calibration. PREDICT-PE-01 and PREDICT-PE-02 are designed to estimate them per profile. They are not population constants.

> **Note on $L^*_{critical,i}$:** The composite load $L^*$ can pass REQT while a single component is at critical load. $L^*_{critical,i}$ is the threshold for each of the five components of the load decomposition (§2.10). When any single component exceeds its critical value, the system fails component REQT (§3.7 Note 4) regardless of the composite. This prevents false-positive qualification of systems with isolated severe debt.
>
> **Calibration:** Component threshold values are individual calibration parameters. They are not population constants. Calibration protocol: measure $L^*_i$ for each component across a range of load states, identify the point at which the corresponding functional domain (cognitive performance, autonomic regulation, inflammatory response) shows measurable degradation, and fit the threshold per individual. See PREDICT-REQT-03 for the relevant test.

### 2.10 The Load Decomposition

$L^*$ is not a scalar state — it is a profile across five components. Each component is calculated as a drift from the individual's own baseline.

$$L^* = w_1 L^*_{HRV} + w_2 L^*_{RHR} + w_3 L^*_{temp} + w_4 L^*_{inflam} + w_5 L^*_{resp}$$

$$\sum_i w_i = 1$$

**Default weights (proposed — subject to empirical calibration via PREDICT-AL-01):**

| Component | Weight | Rationale |
|---|---|---|
| $L^*_{HRV}$ | 0.30 | HRV baseline drift is the earliest indicator of cumulative debt |
| $L^*_{RHR}$ | 0.25 | Sleep RHR elevation reflects persistent background demand |
| $L^*_{temp}$ | 0.15 | Temperature elevation reflects inflammatory load |
| $L^*_{inflam}$ | 0.20 | Chronic inflammation reflects long-term regulatory debt |
| $L^*_{resp}$ | 0.10 | Respiratory inefficiency reflects bracing and diaphragm lock |

**Each component** is computed as a within-person drift:

$$L^*_{component} = \frac{Value_{current} - Baseline_{component}}{Baseline_{component} - Floor_{component}}$$

Where $Baseline_{component}$ is the 30-day median and $Floor_{component}$ is the 30-day minimum (for markers that decrease with load) or maximum (for markers that increase with load). Full protocols in Allostatic Load §6b.

**The composite vs. diagnostic distinction:**

- **Composite $L^*$** (above): total debt magnitude. Appropriate when multiple components are elevated and the question is overall load.
- **Diagnostic $L^*_{diagnostic} = \max_i L^*_i$**: where the debt is concentrated. Appropriate for treatment targeting.

A person with $L^*_{resp} = 1.0$ and all other components at 0.0 has composite $L^* = 0.10$ but is at maximum bracing load. The composite answers "how much total debt?" The maximum answers "where is the debt?"

**Minimum viable measurement** (HRV-only):

$$L^* \approx \frac{1}{2}\left( \frac{HRV_{morning} - HRV_{evening}}{HRV_{morning} - HRV_{floor}} + \frac{HRV_{max} - HRV_{sleep}}{HRV_{max} - HRV_{floor}} \right)$$

The additive average is used rather than a product to prevent a single near-zero component from collapsing the output when the other shows maximum load.

### 2.11 The Motor Gain Variables

| Symbol | Name | Definition |
|---|---|---|
| $G_m$ | Motor gain | $G_m = \alpha P - \beta \eta$ — amplification of motor intention |
| $\text{Drift}$ | Motor drift | $\text{Var}(X_{intended} - X_{actual})$ — variance in motor output relative to intention |
| $\text{Cache}$ | Motor cache availability | $N_{cached} / N_{total}$ — availability of cached movement patterns |
| $C_{risk}$ | Collapse risk | $\gamma \cdot G_m / (1 + \text{Cache})$ — probability of precision loss during movement |
| $M_{state}$ | Motor state | Discrete state — Stable / Unstable / Collapsed — determined by $G_m$, Cache, and $C_{risk}$ thresholds |

> **Note on the motor gain variables:** These variables enter the motor gain equations (§3.11) rather than the master equation directly. They describe the substrate layer at which precision expresses as movement — the "limb with gain requiring control" formulation. See Precision v3.4 Part III for the full formalization.

> **Note on $M_{state}$ thresholds:** The discrete state of $M_{state}$ is determined by three thresholds: $G_{threshold}$ (motor gain above which the system is unstable), $\text{Cache}_{min}$ (motor cache below which the system is unstable), and $C_{threshold}$ (collapse risk above which the system has collapsed). **These threshold values are individual calibration parameters, not population constants.** No current prediction calibrates them directly.
>
> The relevant measurements are:
> - PREDICT-PREC-06 measures $G_m$ but does not calibrate $G_{threshold}$
> - PREDICT-MOTOR-01 measures distortion location but not motor state transitions
> - PREDICT-MOTOR-02 measures sequencing effects but not motor state thresholds
>
> **Calibration of $M_{state}$ thresholds is an open empirical question.** The formal protocol would be: induce motor load across the stable–unstable–collapsed range, measure $G_m$, Cache, and $C_{risk}$ at each transition point, and fit the threshold values per individual. This is the motor analog of the $\tau_{threshold}$ and $K_{critical}$ calibration in §2.9.

### 2.12 The Somatic Commutation Variables

Somatic commutation is the active mechanism by which in vivo systems manipulate their own manifold geometry to preserve outer-edge access under load. Full specification in GoI v1.0 §3.4 and §8.

| Symbol | Name | Definition |
|---|---|---|
| $\sigma(t)$ | Gaze laterality | $\in \{-1, 0, +1\}$ — left, center, right |
| $H_L(t), H_R(t)$ | Contralateral hemispheric drive | $H_L = f_L(\sigma(t))$, $H_R = f_R(\sigma(t))$ — gaze direction modulates $C_{LR}$ |
| $C_{LR}$ | Interhemispheric phase-locking coherence | Operational measurement of $P$ in the interhemispheric integration paradigm |
| $f_{resp}, f_{baro}$ | Respiratory and baroreflex frequencies | Resonance occurs when $f_{resp} = f_{baro}$ at ~0.1 Hz |
| RSA phase | Respiratory sinus arrhythmia phase | Inhale = jump-ready; exhale = lock-ready |

> **Note on somatic commutation:** The operator modulates $C_{LR}$ locally through gaze direction and cervical rotation. The FEF (frontal eye fields) drives contralateral hemispheric networks — left gaze increases right hemisphere contribution, right gaze increases left hemisphere contribution. RSA phase determines whether the commutator is in "jump" mode (inhale, low vagal tone, high tolerance for state change) or "lock" mode (exhale, high vagal tone, high stability). See GoI v1.0 §3.4 for the full mechanism, §8 for extended treatment, and PREDICT-INF-08, -09, -12 for the falsifiable predictions.

### 2.13 The Breath Phase Timing Variables

Breath phase is not a background process — it is the timing clock for inference. Each breath phase has a distinct functional role.

| Phase | Function | Neural correlate |
|---|---|---|
| Controlled inhalation | Frame loading — active generation of prediction errors | Olfactory bulb theta-gamma phase-locking (Zelano et al., 2016) |
| Low-perturbation hold | Manifold stabilization — hyper-precise holding of thought configurations | Sensory gating requirement drops to zero; $\eta$ plunges |
| Controlled exhalation | Frame pruning — gradual narrowing, shedding peripheral detail | Vagal downregulation; RSA amplitude reduction |

> **Note on the low-perturbation hold:** During the hold, the somatic noise floor $\eta$ plunges, raising the precision ceiling $\delta_{min} = \eta/(A_s^* \cdot I^*)$. The system can hold complex, multi-layered cognitive structures without decay or disruption. This is the zone where deep inference occurs — not during active breathing, not during exhalation, but in the quiet space between. See GoI v1.0 §9 and PREDICT-INF-10.

### 2.14 The Four-Layer Cache Hierarchy

The manifold is organized as a four-layer cache hierarchy. Access to any layer requires precision $R^*$ above threshold. The layers are:

| Layer | Region | Access Cost | Collapse Order |
|---|---|---|---|
| Layer 0 | Survival geometry | Zero — always funded | Never |
| Layer 1 | Left hemisphere — inner core | Low — always accessible | Never collapses before Layer 3 |
| Layer 2 | PFC — the gate | Threshold-controlled | Gate failure precedes outer collapse |
| Layer 3 | Right hemisphere — outer edge | High — requires gate open | Collapses first under any degradation |

**The topological invariant:** You cannot reach Layer 3 without traversing Layers 0, 1, and 2. There is no right-hemisphere-only state. This is not an empirical generalization — it is a consequence of the manifold's topology. The clinical record confirms it: what is never observed is right-hemisphere processing while the left hemisphere is offline.

**Access rule.** The gate (Layer 2) opens when $P_{eff} > P_{threshold}$ and $O_{pathway} > O_{min}$. Below threshold, processing remains in Layers 0–1 (prior retrieval, Path B). Above threshold, Layer 3 becomes accessible (adversarial inference, Path A).

**Collapse order.** The four-layer hierarchy produces the topologically forced collapse sequence of §5b. Precision drops first (Layer 3 access degrades), then window narrows (Layer 2 threshold rises), then integration fails (Layer 2 → Layer 3 traversal fails), then resolution floor rises (Layer 1 comparison granularity coarsens), then gate closes (Path B becomes default), then prior calcification (Layer 1 stops updating).

**Circuit priming.** The competitive scaffold that constitutes Layer 3's reach is not static. It is maintained through precision-gated access that traverses the long-range connections. Recent traversal reduces access cost — the manifold has been "primed." This is why recovery is asymmetric: rebuilding the competitive scaffold takes longer than degrading it. See GoI v1.0 §1.6 for the full circuit priming mechanism.

### 2.15 The Three Axes of Collapse Shape

The framework specifies **what** collapses (the master state variables, §2.1) and **in what order** (the collapse sequence, §5b). The three axes specify **why the collapse takes the shape it does** in a given domain.

The three axes were named in the first full domain projection (The Spoken Language Paper v3.0). They are general structural features of any collapse, not speech-specific.

| Axis | Definition | Domain-general role |
|---|---|---|
| **Supply** | The available precision budget — the master state variables, normalized to the individual's own baseline | How much the system can afford |
| **Demand** | How many timing-encoded or integration-encoded layers the domain requires | How much the system must spend |
| **Channel** | The substrate cost of the output modality — how much precision the modality consumes before the output is produced | How much the system spends before the output exists |

**Supply** is already registered as the master state variables (§2.1). It is the precision budget: $A_s^*$, $R^*$, $W^*$, $\Theta^*$, $I^*$, and $L^*$.

**Demand** is the number of layers the domain requires. In the speech domain, demand is the suprasegmental architecture of the language — stress-timed, syllable-timed, mora-timed, tonal, pitch-accent, intonational. In another domain, demand will be something else. The demand axis is the domain's **load-bearing layer count**.

**Channel** is the substrate cost of the output modality. In the speech domain, channel is the output modality — speech, typing, sign, inner speech. In another domain, channel will be something else. The channel axis is the domain's **output cost structure**.

**The collapse shape** is the interaction of the three axes. The same supply produces different collapse shapes depending on demand and channel. The same demand produces different collapse shapes depending on supply and channel. The same channel produces different collapse shapes depending on supply and demand.

**Why these are named as structures, not variables:** Supply, demand, and channel are not state variables — they do not have a single value at a moment in time. They are **modifiers of the collapse shape**, each of which has a domain-specific form. Registering them as named structures rather than symbols lets future projections register their own domain-specific versions without redefining the axes.

**Status:** The three axes are operational in the speech projection. Their general form is registered here. They require confirmation in other domains.

### 2.16 The Integration-Demand Rule and Layer Stacks

The collapse sequence (§5b) specifies the fixed order of collapse **stages**. The integration-demand rule specifies the fixed order of collapse **layers** within a domain.

**The rule:**

> Layers requiring more cross-domain integration collapse first. Layers that can run on cached or single-domain processing collapse last.

The rule follows from the structure of the manifold. A layer that binds many domains must hold many signals simultaneously in the window. When the window narrows, the layer with the most signals to hold loses them first. A layer that runs on a single domain or on cached patterns needs fewer signals and survives longer.

**The layer stack.** Every domain has a **layer stack** — an ordered set of domain-specific output layers, ordered by integration demand. The layer stack is a domain-specific object. Central Reference cannot specify the stack for every domain; it can only specify that every domain has one, and that the order is set by integration demand.

**What the layer stack specifies:**

- **The layer count.** How many distinct output layers the domain has. This is a discovery, not a prediction. The speech domain has eight; another domain may have five or twelve.
- **The layer order.** Which layer collapses first, which second, and so on. The order is set by integration demand.
- **The layer boundaries.** Where one layer ends and the next begins. The boundaries are analytic distinctions, not hard physical separations; they overlap in practice.
- **The layer dependency structure.** Which layers depend on which. The dependency structure is why collapse cascades: when a lower layer degrades, the layers above it lose their substrate.

**What the layer stack predicts:**

- The stack order is invariant across collapse causes within the same domain.
- The stack order is set by integration demand, not by load type.
- The stack order is a topological consequence of the domain's structure, not a preference or convention.

**Status:** The rule is operational in the speech projection. It requires confirmation in other domains.

### 2.17 The Collapse-Recovery Asymmetry

The framework specifies collapse (§5b). The first full domain projection revealed that recovery is **not the reverse of collapse** — it has its own order, and the order is asymmetric.

**The asymmetry:**

- **Collapse is passive.** The system loses precision as load rises. No active process is required. The stages occur in a topologically forced order because each stage causes the next.
- **Recovery is active.** The system must rebuild the competitive scaffold, restore the respiratory support, and re-establish the interoceptive routing. Rebuilding takes longer than degrading.
- **The hysteresis delay** ($\delta_{hyst}$, §2.3) makes recovery slower than collapse. The delay decays exponentially.

**The recovery ladder.** Every domain has a **recovery ladder** — the order in which layers return. The recovery ladder is domain-specific. Central Reference cannot specify the ladder for every domain; it can only specify that every domain has one, and that the order is set by **substrate dependency**: layers that depend directly on the substrate recover first; layers that depend on the full integration stack recover last.

**What the recovery ladder predicts:**

- The recovery order is determined by substrate dependency, not by the reverse of the collapse order.
- Layers with lower integration demand recover faster.
- Layers that are highly cached recover faster than layers that require real-time integration.
- Recovery signatures precede subjective reports. The voice returns before the person feels better. The system sounds normal before it is normal.

**Status:** The asymmetry is operational in the speech projection. It requires confirmation in other domains.

### 2.18 Expression and Congruence

The framework specifies how salience is generated ($S = C_s \cdot I^*$, §3.4) and how $I^*$ is decomposed ($I^* = f_{routing} \cdot f_{gain} \cdot f_{sensorium}$, §2.4). It does not, until now, specify how much of the resulting salience **reaches expression** versus how much is consumed by output management.

The first full domain projection (The Spoken Language Paper v3.1) revealed that this is a general variable, not a speech-specific one. In any domain where the system's output can be decoupled from its internal state, the proportion of salience reaching expression is a distinct quantity that modulates the observable output.

**The expression ratio:**

$$f_{expression} = \frac{S_{expressed}}{S_{available}} = 1 - \frac{\sum_i P_i W_i}{C_s \cdot I^*}$$

Where:

- $S_{available} = C_s \cdot I^*$ — available salience (usable bandwidth × interoceptive routing)
- $\sum_i P_i W_i$ — salience spent on layer management (precision × window width, summed across active layers)
- $S_{expressed} = S_{available} - \sum_i P_i W_i$ — salience remaining for expression
- $f_{expression} \in [0, 1]$ — the proportion of available salience that reaches expression

**What $f_{expression}$ determines:** whether the output is **congruent** — whether it matches the system's actual state.

**What $f_{expression}$ does not determine:** whether the output is **present**. Presence is $A_s^*$. A system can have high-amplitude, well-articulated output with $f_{expression}$ near 0 — the output is funded, but the funding is going to the performance, not to the readout.

**The relationship to $f_{routing}$:** $f_{routing}$ (§2.4) is the **input-side** component of $I^*$. $f_{expression}$ is the **output-side** modifier on $S$. They sit on opposite sides of the salience equation. $f_{routing}$ determines how much $I^*$ you have. $f_{expression}$ determines how much of the resulting salience reaches the output. The two are distinct variables with distinct roles; a system can have high $f_{routing}$ and low $f_{expression}$, or low $f_{routing}$ and high $f_{expression}$.

**The layer-management cost.** $\sum_i P_i W_i$ is the precision spent on managing the output layers. When the cost rises — because output management requires more precision, because more layers are active, or because the masker is monitoring a discrepancy between state and presentation — $f_{expression}$ drops. The precision spent on management is precision not spent on expression, interoceptive readout, or recovery.

**Congruence as the operational readout.** $f_{expression}$ is a latent variable. Its observable proxy is the **congruence** between the system's output and its independently reported load:

$$\text{Congruence} = \text{corr}(\text{Output expressiveness}, \text{Load self-report})$$

Where:

- **Output expressiveness** = the domain-specific expressiveness measures (speech: pitch range, amplitude, granularity; movement: range, speed, variability; etc.)
- **Load self-report** = the system's report of perceived effort, depletion, or demand

**Why load self-report, not state self-report:** The comparator is *load*, not *state*, to avoid circularity. A system with low $f_{expression}$ starves interoception, which compromises self-report of *state* (mood, feeling). But the system can still report *load* (perceived effort, depletion) because the effort signal is generated by the management process itself. The speaker who can't report how they feel can still report that they're working hard.

**The congruence prediction.** When $f_{expression}$ is high, output expressiveness tracks load self-report — the voice sounds tired when the speaker is tired. When $f_{expression}$ is low, output expressiveness is decoupled from load self-report — the voice sounds fine when the speaker is depleted.

**The masking load term.** Chronic low $f_{expression}$ is a load source. The continuous monitoring and correction required to maintain a discrepancy between internal state and external expression adds to the load trajectory:

$$\lambda_{mask} = \phi(1 - f_{expression})$$

Where $\phi$ is the masking-load coefficient. This term enters the glymphatic ODE (§4). The full functional form of $\phi$ requires calibration — it may depend on $A_s^*$, on the duration of masking, on the domain-specific cost of output management, or on all three.

**The four-state table.** The interaction of $A_s^*$ (presence) and $f_{expression}$ (congruence) produces four states:

| $A_s^*$ | $f_{expression}$ | Output signature | Clinical readout |
|---|---|---|---|
| High | High | Expressive, congruent | Healthy expressive range |
| High | Low | Expressive, incongruent | Masking / performance |
| Low | High | Flat, congruent | Honest collapse |
| Low | Low | Flat, incongruent | Failed mask / depletion |

**The two failure modes:**

- **Low $f_{expression}$, low $A_s^*$:** collapse with no mask. The output is flat and the state is visible. This is the depression signature.
- **Low $f_{expression}$, high $A_s^*$:** collapse with a mask. The output is expressive and the state is hidden. This is the expensive one — the mask costs salience that would otherwise be available for the system's own readout.

**The masking mechanism.** Masking is not a behavior. It is a routing configuration. When a system routes salience to output management, it is spending precision on the production of normal-seeming output. The precision spent there is precision not spent on interoceptive readout, cross-domain integration, or recovery. The result is a system that sounds normal, is depleting, and cannot detect its own collapse because the detection channel is the one being starved.

**The critical prediction:** masking has a measurable cost. Chronic low $f_{expression}$ predicts later collapse detection, because the Stage 1–2 monitoring window is the channel that routing has starved.

**Status:** The expression ratio, the congruence measure, and the masking load term are operational in the speech projection. Their general form is registered here. They require confirmation in other domains.

---

## 3. The Equation Registry

### 3.1 The Master Equation

$$C_s = \left(A_s^{*\,0.15} \cdot R^{*\,0.30} \cdot W^{*\,0.25} \cdot \Theta^{*\,0.15}\right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + L^*}$$

**Status:** The four oscillatory weights sum to 0.85. The remaining 0.15 is structurally claimed by the load term. The exponent $1/0.85$ normalizes the weighted geometric mean. Exponents are provisional — they reflect the empirical collapse sequence (precision degrades first, window second) but have not been formally calibrated.

### 3.2 The Curvature Equation

$$K = k\left(\frac{1}{R^* + \epsilon}\right) + \sum_i S_i \cdot C_i$$

**Transfer functions:**

$$W^* = \frac{1}{1 + \alpha K}, \quad \Theta^* = \frac{1}{1 + \beta K}$$

**Note on the $J(C) \to \eta$ pathway:** Chemoreflex jitter $J(C)$ raises the effective noise floor rather than adding curvature directly. This is because jitter *degrades signal detectability* without changing the geometric structure of existing representations — the manifold's shape is unchanged, but what can be detected through it is reduced.

$$\eta_{effective} = \eta_{baseline} + f(J(C))$$

The functional form of $f$ is assumed linear for simplicity: $\eta_{effective} = \eta_{baseline} + J(C)$.

### 3.3 The Precision Equations

**Precision:**

$$P = \frac{R}{D_T}, \quad R^* = \frac{P}{P_{baseline}}$$

**Timing distance (full form):**

$$D_T = \frac{k_2}{H(C)} \cdot \frac{1 + \lambda_c \Pi_{cog}}{1 - \lambda_m \Pi_{mech}} + J(C)$$

**Sync duration (full form):**

$$R = k_3 H(C) \cdot (1 + \mu_m \Pi_{mech}) \cdot e^{-\mu_c \Pi_{cog}} \cdot e^{-\nu J(C)}$$

**Chemoreflex jitter:**

$$J(C) = \begin{cases} 0 & C \le C_{high}(L^*) \\ \kappa(C - C_{high}(L^*))^2 & C > C_{high}(L^*) \end{cases}$$

Note that $C_{high}$ is now load-dependent: $C_{high}(L^*) = C_{high}^0 - \gamma L^*$.

**CO₂ uniformity:**

$$U_C = \frac{1}{\text{Var}_i[C_i] + \epsilon}$$

**Collapse hysteresis:**

$$P_{recover} = P(t) - \delta_{hyst}, \quad \frac{d\delta_{hyst}}{dt} = -\sigma \delta_{hyst}$$

**Load-dependent precision (summary):**

$$P(L^*) = \frac{R_0 e^{-\mu_c L^*}}{D_0 (1 + \lambda_c L^*)} \cdot U_C(L^*)$$

where $U_C(L^*) = 1/(1 + \nu L^*)$. This is a compact summary — the full equations above are the primary specification.

### 3.4 The Routing Equations

**Salience:**

$$S = C_s \cdot I^*$$

**Routing capacity:**

$$I^* = C_{total} - \sum_i P_i \cdot W_i, \quad I^* = f_{routing} \cdot f_{gain} \cdot f_{sensorium}$$

### 3.5 The Resolution Floor

$$\delta_{min}(\text{channel}) = \frac{\eta}{A_s^* \cdot I^*(\text{channel})}$$

### 3.6 The Gate Condition

$$P_{eff} = P \cdot O_{pathway} \cdot U_C$$

$$P_{threshold} = P_0 - \gamma L^*$$

Gate opens when $P_{eff} > P_{threshold}$ AND $O_{pathway} > O_{min}$.

### 3.7 The Qualification Equation

REQT is the condition under which Intelligence > 0 is sustained. When REQT ≤ 0, $\Lambda \to 0$ and the intelligence product collapses regardless of $n_{hops}$, $R^*$, or $\Theta^*$. REQT defines the minimum substrate state required for the loop to run at all.

$$REQT = \left(\frac{A_s^*}{A_{s,0}^*} \cdot \frac{R^*}{R_0^*} \cdot \frac{W^*}{W_0^*} \cdot \frac{\Theta^*}{\Theta_0^*} \cdot \frac{I^*}{I_0^*}\right) - L^* > 0$$

**Note on weighting:** REQT uses equal weights as a conservative qualification default — any component falling significantly below baseline is treated as a disqualifier regardless of compensating strength in other components. The master equation (§3.1) uses unequal weights because they reflect the empirical collapse sequence (precision degrades first). REQT weights reflect minimum viable threshold — a different question. Component REQT (Note 4 below) captures the case where a single component is at critical load while the composite passes.

**Requalification condition:**

$$REQT > 0 \quad \text{after} \quad L^* < L^*_{threshold} \quad \text{AND} \quad \Lambda > 0 \quad \text{for} \geq 48h$$

**Note 1 — Individual normalization:** Subscript 0 denotes the individual's own validated baseline. Population norms are not the comparator. A degraded world-class performer may be more impaired than a baseline junior — the metric captures this.

**Note 2 — The gate-lowering failure mode:** As $L^*$ rises, $P_{threshold} = P_0 - \gamma L^*$ drops. The gate remains open but admits lower-quality signal. The decision-maker appears functional. The output is Path B dressed as Path A. This is the most dangerous failure mode — it is undetectable from behaviour alone. The Allostatic Load framework (Robinson, 2026e) describes the exact clinical scenario: patients with "normal biomarkers but subjective dysfunction" are in gate-lowering collapse.

**Note 3 — Requalification requires loop activation, not time:** Rest reduces $L^*$ but does not reopen the gate. $\Lambda > 0$ for ≥48h is required separately.

**Note 4 — Component REQT:** Composite REQT can be passed while a single component is at critical load:

$$REQT_{component} = REQT_{composite} \wedge (\max_i L^*_i < L^*_{critical,i})$$

A system passes REQT only if both total load is manageable AND no single component is at critical level. This prevents false-positive qualification of systems with isolated severe debt.

### 3.8 The Prior Update Rate

$$\mathcal{U} = \frac{A_s^* \cdot R^* \cdot \Theta^*}{1 + \gamma K_{enc}}$$

**Encoding window:**

$$W_{enc} = \int_{t_{enc}} \mathbb{1}[P(t) > P_{threshold}] dt$$

### 3.9 The Structural Equations

**Interference metric:**

$$IM = \frac{d_{irrel}}{d_{rel}} (\vec{u}_{irrel} \cdot \vec{u}_{rel})$$

**Neural dimensionality:**

$$\text{Dim} = W^* \times \Theta^*$$

**Inference hops:**

$$n_{hops} = \lfloor W^* \cdot \rho_{scaffold} \rfloor$$

### 3.10 The Prediction-Error Equations

$$\tau_{PE} = \frac{1}{J(C)} \cdot \frac{1}{\Pi_{cog}}$$

$$\sigma_{PE} = \frac{1}{\delta_{min}} = \frac{A_s^* \cdot I^*}{\eta}$$

$$\Lambda = \Theta^* \cdot R^* \cdot \mathbb{1}[P_{eff} > P_{threshold}]$$

### 3.11 The Motor Gain Equation

$$G_m = \alpha P - \beta \eta$$

**Movement stability:**

$$\text{Stability} = \frac{1}{G_m \cdot \text{Drift}}$$

**Collapse risk:**

$$C_{risk} = \frac{\gamma \cdot G_m}{1 + \text{Cache}}$$

**Motor state:**

$$M_{state} = \begin{cases} \text{Stable} & \text{if } G_m < G_{threshold} \text{ and Cache} > \text{Cache}_{min} \\ \text{Unstable} & \text{if } G_m > G_{threshold} \text{ or Cache} < \text{Cache}_{min} \\ \text{Collapsed} & \text{if } C_{risk} > C_{threshold} \end{cases}$$

### 3.12 The Social Projection

Same equations, distributed substrate:

| Individual | Social |
|---|---|
| $A_s^*$ — oscillatory amplitude | Collective synchrony capacity |
| $\sigma(A_s)$ — jitter | Social fragmentation |
| $R^*$ — precision | Shared meaning resolution |
| $K$ — curvature | Collective load |
| $W^*$ — window width | Temporal horizon of collective planning |
| $\Theta^*$ — integration | Cross-group coordination |
| $I^*$ — interoceptive routing | Collective self-awareness |
| $L^*$ — persistent load | Historical trauma, institutional conditioning |
| $\mathcal{U}$ | Cultural prior update rate |
| $C_s$ | Collective usable bandwidth |

$$\text{Synchrony} \rightarrow A_s^* \rightarrow \sigma(A_s) \rightarrow R^* \rightarrow K \rightarrow W^* \rightarrow \Theta^* \rightarrow C_s^{collective}$$

### 3.13 The Full Dynamic $P(t)$ Equation

The compact summary $P(L^*)$ in §3.3 is a reduced form. The full dynamic precision equation with both pressure components and jitter is:

$$P(C, \Pi_{mech}, \Pi_{cog}) = \frac{k_3}{k_2} \cdot H(C)^2 \cdot \frac{(1 + \mu_m \Pi_{mech}) \cdot e^{-\mu_c \Pi_{cog}} \cdot e^{-\nu J(C)}}{\frac{1 + \lambda_c \Pi_{cog}}{1 - \lambda_m \Pi_{mech}} + \frac{k_2}{H(C)} J(C)}$$

Where $H(C)$ is HRV as a function of CO₂:

$$H(C) = k_1 \cdot C \quad \text{for } C_{low} < C < C_{high}(L^*)$$

$$H(C) = k_1 \cdot C_{high}(L^*) \cdot e^{-\nu(C - C_{high}(L^*))} \quad \text{for } C > C_{high}(L^*)$$

**Effective precision** with substrate and uniformity constraints:

$$P_{eff} = P \cdot O_{pathway} \cdot U_C$$

**Load-dependent full form** (equivalent to the compact summary when $\Pi_{mech}$ and jitter are suppressed):

$$P(L^*) = \frac{R_0 e^{-\mu_c L^*}}{D_0 (1 + \lambda_c L^*)}$$

This is the primary specification. The compact form in §3.3 is the reduced version. See Precision v3.4 §2.3 for the full derivation.

### 3.14 The Temporal Dynamics

**Rate of precision change:**

$$\frac{dP}{dt} = \frac{\partial P}{\partial H}\frac{dH}{dt} + \frac{\partial P}{\partial \Pi_{mech}}\frac{d\Pi_{mech}}{dt} + \frac{\partial P}{\partial \Pi_{cog}}\frac{d\Pi_{cog}}{dt} + \frac{\partial P}{\partial J}\frac{dJ}{dt}$$

**Uniformity dynamics:**

$$\frac{dU_C}{dt} = -\rho \cdot \text{Var}_i[C_i(t)]$$

**Precision lock:**

$$\frac{dP}{dt} \approx 0 \quad \text{AND} \quad P_{eff}(t) > P_{threshold}$$

**Lock duration:**

$$T_{lock} = \int_{t_{onset}}^{t_{offset}} \mathbb{1}_{P_{eff}(t) > P_{threshold}} dt$$

**Flow as sustained precision lock:**

$$Flow(t) = P_{eff}(t) \quad \text{for } t \in T_{lock}$$

Flow maintenance requires:

$$\frac{dP}{dt} \approx 0 \quad \text{AND} \quad C_{low} < C(t) < C_{high}(L^*) \quad \text{AND} \quad \Pi_{mech}(t) > \Pi_{threshold} \quad \text{AND} \quad \Pi_{cog}(t) < \Pi_{threshold} \quad \text{AND} \quad O_{pathway}(t) > O_{min}$$

Flow collapse when any condition fails.

**Encoding window dynamics:**

$$W_{enc} = \int_{t_{enc}} \mathbb{1}[P(t) > P_{threshold}] dt$$

**Hysteresis dynamics:**

$$P_{recover}(t) = P(t) - \delta_{hyst}, \quad \frac{d\delta_{hyst}}{dt} = -\sigma \delta_{hyst}$$

### 3.15 Resonance Breathing as a Third Precision Mechanism

Beyond the two primary precision mechanisms (CO₂-driven precision and breath-hold precision lock), resonance breathing produces sustained precision through frequency entrainment of the respiratory and cardiac oscillators.

When $f_{resp} = f_{baro}$ at ~0.1 Hz (≈6 breaths/min):

$$\Pi_{mech} \propto \text{PLV}(f_{resp}, f_{baro})$$

Drift drops, jitter remains low, and precision rises without entering the CO₂ tolerance window. This produces stable clarity and flow without spasms or collapse.

**Cross-frequency coupling (CFC)** extends the precision model to interactions across multiple frequency bands — respiration–HRV coupling, alpha–theta coupling during meditation, theta–HRV coupling during breath-hold, gamma–cardiac phase coupling during flow states. CFC is the empirical operationalization of $\Theta^*$.

See Precision v3.4 §1.2, §1.8 for the full specification.

### 3.16 The Demand-Axis Form

The demand axis (§2.15) has a general form: the total demand is the sum of the layers the domain requires, weighted by how load-bearing each layer is.

$$\mathcal{D} = \sum_i w_i \cdot d_i$$

Where:
- $d_i$ = the demand of layer $i$ (how many domains it binds)
- $w_i$ = the weight of layer $i$ in the domain (how load-bearing it is)

**For the speech domain:** $\mathcal{D}_{speech}$ is the sum of the eight layer weights, where $w_i$ depends on the language's suprasegmental architecture (stress-timed, syllable-timed, mora-timed, tonal, pitch-accent, intonational).

**For other domains:** $\mathcal{D}$ will have different components, but the same form. The demand axis is always a weighted sum of the layer demands.

**Status:** The form is general. The components are domain-specific. The weights require calibration.

### 3.17 The Channel-Cost Form

The channel axis (§2.15) has a general form: the substrate cost is the precision consumed by the output modality before comprehension can use the output.

$$\mathcal{C} = \sum_j c_j$$

Where each $c_j$ is the precision consumed by a specific substrate process.

**For speech:** $\mathcal{C}_{speech}$ = pressure modulation + postural reconfiguration + laryngeal control. Typing has $\mathcal{C}_{typing} \approx 0$. Sign has $\mathcal{C}_{sign}$ = visual attention + manual motor precision. Inner speech has $\mathcal{C}_{inner} \approx 0$.

**The channel-preference condition:**

$$\text{Channel choice} = \arg\min_\mathcal{C} \left( \mathcal{C} \mid \mathcal{S} - \mathcal{C} > \mathcal{S}_{threshold} \right)$$

The speaker selects the cheapest channel whose substrate cost leaves enough supply for comprehension. When supply drops, the speaker shifts to cheaper channels. The shift is a readout of the precision budget.

**Status:** The form is general. The components are domain-specific. The costs require calibration.

### 3.18 The Recovery-Rate Form

Recovery is not instantaneous. The recovery rate depends on the substrate dependency of each layer.

$$T_{recover}(layer_i) = \frac{\delta_{hyst}}{1 - d_i / d_{max}}$$

Where:
- $d_i$ = the demand of layer $i$ (how many domains it binds)
- $d_{max}$ = the maximum demand in the stack
- $\delta_{hyst}$ = the hysteresis delay

**The prediction:** layers with lower demand recover faster. Layers with higher demand recover slower. The recovery rate is inversely related to the collapse rate, but not symmetrically.

**Status:** The form is proposed. It requires calibration. The qualitative prediction — low-demand layers recover first — is the key testable claim.

### 3.19 The Expression Equation

The expression equation specifies how much of the available salience reaches the output.

$$S_{expressed} = S \cdot f_{expression}$$

Where:

- $S = C_s \cdot I^*$ — available salience (§3.4)
- $f_{expression} = 1 - \frac{\sum_i P_i W_i}{C_s \cdot I^*}$ — the expression ratio (§2.18)
- $S_{expressed}$ — the salience that reaches expression

**The full form:**

$$S_{expressed} = C_s \cdot I^* - \sum_i P_i W_i$$

**The congruence form:**

$$\text{Congruence} = \text{corr}(\text{Output expressiveness}, \text{Load self-report})$$

**The masking load term:**

$$\lambda_{mask} = \phi(1 - f_{expression})$$

Where $\phi$ is the masking-load coefficient. This term enters the glymphatic ODE (§4).

**Status:** The form is general. The components are domain-specific. The functional forms of $\sum_i P_i W_i$ and $\phi$ require calibration.

---

# PART II — THE CAUSAL CHAIN

The complete sequence from breath to behaviour. Every arrow is a mechanism. Every variable is defined in Part I.

## 4. The Spine

```
BREATH MECHANICS
│   Variables: A_s*, CO₂, respiratory phase
│   Sources: Zelano et al. (2016); Raichle & Plum (1972); Cooper et al. (2003); Kox et al. (2014); Zaccaro et al. (2018)
│
├── Nasal respiration entrains limbic oscillations
├── CO₂ drives cerebral vasodilation
├── CO₂ tolerance window determines precision peak
├── C_high(L*) compresses with load — Control Pause drops
└── Slow breathing at resonance frequency phase-locks respiratory and cardiac oscillators
│
    ↓
PRECISION
│   Variables: P = R/D_T, R*
│
├── Timing distance D_T drops
├── Sync duration R rises
├── P = R/D_T rises
├── Two-factor pressure modulates precision:
│   ├── Π_mech (breath-hold, resonance): beneficial
│   └── Π_cog (load, sympathetic): harmful
└── Above C_high(L*): J(C) injects jitter, P collapses
│
    ↓
CURVATURE
│   Variables: K
│   Empirical proxy: IM (Xue et al. 2026)
│   Cellular mechanism: PV+ interneuron failure (Kann et al. 2015)
│   Metabolic signature: ΔCBF/ΔCMRO₂ decoupling (Hutchison & Rypma 2013)
│   Physical constraint: CVR ceiling
│
├── K = k(1/(R* + ε)) + ∑ S_i · C_i
├── Precision loss raises K
├── Containment cost raises K independently
├── J(C) contributes to K via noise floor
└── As K rises, feature axes become non-orthogonal
│
    ↓
DIMENSIONALITY
│   Variables: Dim, n_hops
│
├── W* = 1/(1 + αK) — window width
├── Θ* = 1/(1 + βK) — integration efficiency
├── Dim = W* × Θ* — independent axes available
├── n_hops = ⌊W* · ρ_scaffold⌋ — hops available
└── As Dim drops, Path A inference degrades to Path B retrieval
│
    ↓
USABLE BANDWIDTH
│   Variables: C_s
│
└── C_s = (A_s*^0.15 · R*^0.30 · W*^0.25 · Θ*^0.15)^(1/0.85) · 1/(1 + L*)
│
    ↓
SALIENCE
│   Variables: S, f_expression
│
├── S = C_s · I*
├── I* = C_total − ∑ P_i · W_i
├── f_expression = S_expressed / S_available
└── S_expressed = S · f_expression
│
    ↓
RESOLUTION FLOOR
│   Variables: δ_min
│
├── δ_min = η / (A_s* · I*)
└── δ_min determines what signals are detectable
│
    ↓
CACHE MISS CONTROLLER
│   Variables: LP-ACC circuit
│
├── LP computes δ = |current − prior|
├── If δ < δ_min: cache hit (return prior)
└── If δ ≥ δ_min: cache miss (escalate)
│
    ↓
PREDICTION ERROR AS BRANCH SIGNAL
│   Variables: δ, τ_PE, σ_PE, K_enc
│
├── δ ≥ δ_min → PE detected
├── Path B: threat → K↑ → W*↓ → P_threshold↑ → gate closes → PE suppressed
└── Path A: τ_PE > τ_threshold → K stable → W* maintained → gate opens → Λ > 0 → loop runs
│
    ↓
THE LOOP (PATH A) or PRIOR RETRIEVAL (PATH B)
│   Variables: Path A/B, Λ
│
├── Path A: Gate open → loop runs → error detection → reinvestment → iteration → convergence
├── Path B: Gate closed → prior retrieval → confident output
├── Speed: R* (precision)
└── Depth: Θ* (integration efficiency)
│
    ↓
PRIOR UPDATE (if Path A)
│   Variables: 𝒰, K_enc
│
├── 𝒰 = (A_s* · R* · Θ*) / (1 + γK_enc)
├── K_enc determines what geometry the prior carries forward
└── Intervention sequence: change geometry first, then introduce signal
│
    ↓
MOTOR ENCODING (substrate layer)
│
├── Cached motor patterns = "near" on manifold
├── Interoception is the encoding bridge
├── PFC economy loop reinforces cached patterns under load
└── Blank motor zones = blank manifold regions
│
    ↓
COLLAPSE OR RECOVERY
│
├── Collapse: Load rises → P drops → gate closes → false cache hits → K rises → δ_min rises → W* narrows → loop accelerates
├── Recovery (autonomic): Breath → A_s* rises → P restored → gate opens → stale priors detected → prior updated → K drops → W* widens
├── Recovery (glymphatic): Slow wave sleep → CSF pulsatility → clearance of amyloid/tau → reduced neuroinflammation → reduced L*
└── Hysteresis: Recovery delayed by δ_hyst

GLYMPHATIC RECOVERY LOOP
│   Variables: SWS%, L*, clearance rate, λ_mask
│   Sources: Iliff et al. (2012); Grunewald et al. (2012); Zhang et al. (2025)
│
├── Load drives faster, shallower breathing
│   → V_T(L*) = V_T^0 · e^(−α L*)
├── Sympathetic dominance suppresses slow wave architecture
│   → SWS%(L*) = SWS%_0 − β L*
├── Reduced SWS% reduces glymphatic clearance
│   → clearance ∝ SWS%(L*)
├── Reduced clearance permits amyloid/tau accumulation
│   → microglial activation → further load
├── Chronic output management (masking) adds load
│   → λ_mask = φ(1 − f_expression)
│
└── Load trajectory:
    dL*/dt = λ_met + λ_inflam + λ_mask − λ_clear · SWS%(L*)

    Recovery is not automatic. It requires substrate integrity.
```

## 4a. The Four Contracts as the Load Mechanism Chain

The spine above (§4) traces breath → behaviour. The load pathway itself is decomposable into four converging regulatory contracts, each contributing to the debt trajectory through a distinct mechanism. Each link is anchored in existing literature.

```
Metabolic stress — elevated glucose, hypoxia, hypercapnia
  ↓ MET↔AUTO
Carotid body chemoreceptors sense arterial CO₂, O₂, pH, glucose simultaneously
  ↓ [Moreira et al., 2006]
Sympathetic output rises, vagal tone compresses, HRV drops
  ↓ [Thayer et al., 2010]

Elevated glucose
  ↓ MET↔IMMUNE
Mast cell activation → TNF-α, IL-1β, IL-6 → macrophage M1 polarization 
→ insulin resistance → glucose maintained
  ↓ [Segerstrom & Miller, 2004]

Cytokines cross blood-brain barrier → hypothalamic and brainstem disruption
  ↓ IMMUNE↔AUTO
Low vagal tone → inadequate cholinergic anti-inflammatory pathway 
→ cytokine brake fails → HRV and CAP share the same efferent pathway
  ↓ [Tracey, 2002]
  ↓ [Hall et al., 2004]

Autonomic compression accumulates
  ↓ AUTO↔MOD
Incomplete exhale → RSA amplitude reduction → oscillatory window compresses 
→ precision loss
  ↓ [Mathewson et al., 2016]
  ↓ [Reed et al., 2020]

High load → faster shallower breathing → reduced intrathoracic pressure differential
  ↓ GLYMPH↔AUTO
Reduced CSF pulsatility → glymphatic clearance fails → amyloid accumulation 
→ microglial activation → sleep architecture disruption → further load
  ↓ [Iliff et al., 2012]
  ↓ [Grunewald et al., 2012]
  ↓ [Zhang et al., 2025]

Accumulated debt visible as trajectory
  ↓
HRV baseline drifts downward across days
  ↓ [Okawara et al., 2024]

Delta HRV response compresses toward zero
  ↓
L* rises — system approaches load ceiling
```

**The four contracts:** MET↔AUTO (metabolic entry point), MET↔IMMUNE (accumulation mechanism), IMMUNE↔AUTO (vagal compression mechanism), AUTO↔MOD (behavioral signature). Plus GLYMPH↔AUTO (clearance failure amplifier). Full contract specifications in the Unified Regulatory Model (github.com/jtrthehax/Unified-Model). Extended treatment in Allostatic Load v2.1 §2.

## 4b. The Streams Being Measured

The "two oscillatory streams" in the precision definition ($P = R/D_T$) correspond to specific measurable phenomena. The respiratory oscillator directly entrains neural oscillation — Zelano et al. (2016) demonstrated nasal breathing entrains piriform cortex, hippocampus, and amygdala in a phase-specific manner, with memory recall better during inhalation and effects disappearing with mouth breathing.

| Stream | Neural correlate | Measurement |
|---|---|---|
| Left hemisphere oscillation | Language-dominant network | EEG phase, MEG |
| Right hemisphere oscillation | Contextual/competitive network | EEG phase, MEG |
| Cardiac oscillation | Heart rate rhythm | ECG / HRV |
| Respiratory oscillation | Breath rhythm | Respiration belt |

Precision can be measured between any pair of these streams. The most relevant for the framework is interhemispheric phase coherence ($C_{LR}$), which determines whether the gate opens. See GoI v1.0 §3.1 for the operationalization.

## 5. The Branch Condition

When prediction error is detected ($\delta \geq \delta_{min}$), the system reaches a branch point.

**Path B — Left Hemisphere Collapse (Identity Protection):**

$$\delta \geq \delta_{min} \rightarrow \text{threat signal} \rightarrow K \uparrow \rightarrow W^* = \frac{1}{1+\alpha K} \downarrow \rightarrow P_{threshold} \uparrow \rightarrow \text{gate closes}$$

$$\rightarrow K_{enc} \text{ activates identity prior} \rightarrow \text{PE suppressed} \rightarrow \text{cached answer returned with high confidence}$$

The left hemisphere response is not passive. It actively raises $K$ in response to PE, which narrows $W^*$ and raises $P_{threshold}$, degrading the conditions required for Path A. Identity-protective cognition is not a choice — it is a gate-closing cascade.

**Path A — Right Hemisphere Inference:**

$$\delta \geq \delta_{min} \rightarrow \tau_{PE} > \tau_{threshold} \rightarrow K \text{ stable} \rightarrow W^* \text{ maintained} \rightarrow P_{eff} > P_{threshold}$$

$$\rightarrow \text{gate opens} \rightarrow \Lambda > 0 \rightarrow \text{loop runs} \rightarrow \mathcal{U} \text{ updates prior}$$

**Formal branch condition:**

$$\text{Path} = \begin{cases} A & \text{if } \tau_{PE} > \tau_{threshold} \text{ AND } K_{enc} < K_{critical} \\ B & \text{otherwise} \end{cases}$$

$\tau_{threshold}$ and $K_{critical}$ are individual parameters requiring empirical calibration. PREDICT-PE-01 and PREDICT-PE-02 are designed to estimate them per profile. They are not population constants.

## 5b. The Collapse Sequence

Collapse does not happen uniformly. It proceeds in a topologically forced order. This determines the monitoring priority.

```
STAGE 1 — PRECISION DROP        R* ↓       Detectable: HRV coherence loss
STAGE 2 — WINDOW NARROWING      W* ↓       Detectable: Flexibility composite drops
STAGE 3 — INTEGRATION FAILURE   Θ* ↓       Detectable: Ambiguity task degrades
STAGE 4 — RESOLUTION FLOOR RISE δ_min ↑    Detectable: Miss rate rises on low-amplitude signals
STAGE 5 — GATE CLOSURE          Λ → 0      Detectable: High-confidence, low-variance output
STAGE 6 — PRIOR CALCIFICATION   U ≈ 0      Detectable: Update rate collapses under contrary evidence
```

**Critical annotation on Stage 5:**

> *"Stage 5 looks like competence from the outside. Output becomes high-confidence and low-variance — precisely the signature of an expert operating from deep prior. Monitoring protocols that wait for Stage 5 are measuring the terminal state. The monitoring window is Stages 1–2."*

**Zone correspondence with measurement metrics:**

| Metric | Zone 1 (Stages 0–1) | Zone 2 (Stages 2–4) | Zone 3 (Stages 5–6) |
|---|---|---|---|
| Sleep HRV | High, clear overnight peak | Moderate, partial rise | Flat, no overnight rise |
| Sleep RHR | < 45 BPM | 45–60 BPM | > 65 BPM |
| $\Delta$HRV slow breath | > 15 ms | 5–15 ms | < 5 ms |
| Control Pause | > 40 s | 25–40 s | < 15 s |
| Sleep respiratory rate | 12–14 BPM | 14–17 BPM | > 17 BPM |
| Week HRV variance | Dynamic, load-responsive | Partially responsive | Flat regardless of load |
| Exhale completeness | Full | Partial | Incomplete |
| SWS proportion | > 20% | 15–20% | < 15% |
| CRP/IL-6 | Normal | Elevated (lagged) | Highly elevated |

This table is the operational companion to the collapse sequence. It maps each stage to measurable zone thresholds. Full measurement protocols in Allostatic Load §5.

**Stage-by-stage detail:**

| Stage | Variable | Collapse signature | Impact |
|---|---|---|---|
| 1 | $R^*$ | HRV coherence loss, PLV drop | Loop still runs but on degraded signal |
| 2 | $W^*$ | Flexibility composite drops | $n_{hops}$ drops — multi-step reasoning degrades |
| 3 | $\Theta^*$ | Ambiguity task performance drops | Cross-domain binding fails — constraints can't be held simultaneously |
| 4 | $\delta_{min}$ | Miss rate on low-amplitude signals rises | Small but critical prediction errors become invisible |
| 5 | $\Lambda$ | Switch to high-confidence, low-update output | Loop has stopped. Path B is default. System appears confident. |
| 6 | $\mathcal{U}$ | Update rate drops to near zero even with contradicting evidence | System cannot be corrected by evidence alone |

## 5c. The Exhale Gate Trap Cascade

The exhale gate trap is the pathological version of the somatic commutation system — a mechanical lock that produces clinical confabulation and conspiracy thinking through the collapse gradient.

**The biomechanical origin.** Residual lung volume. When exhalation is incomplete, the lungs remain partially inflated. The stretch receptors at the base of the lungs cannot fire the vagal signal that would normally accompany full deflation. The brainstem interprets this as a low-grade suffocation signal — a continuous "inhale still needed" state.

**The cascade (acute $\Pi_{cog}$ driving, $L^*$ deepening).**

**1. Autonomic asymmetry (acute $\Pi_{cog}$).** The physical stretch receptors fail to compress fully, denying the vagus nerve the mechanical signal required to downregulate systemic arousal. The brainstem interprets this as chronic suffocation, locking into high-arousal defensive bracing.

**2. Perfusion failure (acute $\Pi_{cog}$ + cumulative $L^*$).** Rapid, shallow thoracic breathing rapidly expels CO₂, inducing hypocapnia. Cerebral vasoconstriction follows, dropping long-range integration pathways below $O_{min}$. Layer 3 is defunded. The acute hypocapnia is $\Pi_{cog}$-driven; the compression of $C_{high}(L^*)$ — which makes the same absolute CO₂ level more jitter-producing — is $L^*$-driven.

**3. The conspiracy manifold (acute $\Pi_{cog}$, deepened by $L^*$).** Cut off from the right hemisphere's broad anomaly detection, processing contracts onto the left hemisphere inner core. The left brain is an explanation engine. Receiving continuous alarm signal from the body with no external visual cause, it hyper-logically links isolated environmental details to justify internal panic.

**4. Spontaneous confabulation (Stage 4 collapse, $L^*$-deepened).** As resolution collapse hits its nadir, $\delta_{min}$ spikes across all channels. Gaps in the narrative cannot be detected. The left-hemisphere interpreter spontaneously generates fabricated, distorted narratives. Because the adversarial check of Layer 3 is unreachable, the system returns false cache hits with total confidence.

**The compact chain:**

```
Trapped Residual Volume (Π_cog acute)
    → Vasoconstriction (Bohr drop)
    → Loss of Layer 3
    → Left-Brain Interpreter Confabulation
    → Deepened by L* (C_high compression, P_threshold drop)
```

**Breaking the trap** follows from the mechanism: (1) restore complete exhalation, (2) restore CO₂ toward $C_{peak}$, (3) restore peripheral vision, (4) restore adversarial inference. The intervention sequence is the same as MS §6b.5 — the body leads, the geometry follows, the cognition emerges. This is the mechanistic account of conspiracy thinking and clinical confabulation. See GoI v1.0 §6.3, §8.3 for the full specification and PREDICT-INF-11 for the falsifiable prediction.

## 5d. Breath Phase and Thought Timing

Breath is not a background process. It is the timing clock for inference. Each phase has a distinct functional role:

| Breath Phase | Mechanical/Neural State | Cognitive Function |
|---|---|---|
| Controlled Inhalation | Olfactory bulb drives cortical theta-gamma phase-locking (Zelano et al., 2016) | Frame Loading — active generation of prediction errors |
| Low-Perturbation Hold | Biomechanical noise eliminated; respiratory sensory gating drops to zero | Manifold Stabilization — hyper-precise holding of thought configurations |
| Controlled Exhalation | Nasal airflow drive dissipates; progressive vagal downregulation | Frame Pruning — gradual narrowing, shedding peripheral detail |

**The Kosik-Rose & Voytek (2026) finding** — each breath has a unique "fingerprint" wave shape that mirrors widespread neural activity — is direct confirmation. The breath is not just correlated with cognitive state. It structurally modulates it.

**The chemoreceptor threshold.** At the bottom of a complete exhale, CO₂ rises rapidly. Up to $C_{high}(L^*)$, this is beneficial — vasodilation, increased precision. Above $C_{high}(L^*)$, central chemoreceptors fire an absolute panic alarm that bypasses cortex and triggers the dorsal respiratory group and locus coeruleus. The abstract inference manifold experiences total collapse onto a single point: the urgent drive to inhale.

**The framework prediction:** precision follows a window, not a monotonic relationship. The system has to stay in the "Bohr window" — CO₂ rising enough to maximize tissue oxygenation but not enough to trigger the chemoreceptor panic. Mastering the low-perturbation hold stretches this window. The window narrows with load — a system at high $L^*$ has less margin.

**Open timing question:** Where in the exhale cycle thoughts actually fire — gradual vs threshold — is distinguishable by EEG. See PREDICT-INF-10. Full specification in GoI v1.0 §9.

## 5e. The Bidirectional Collapse Sequence

The collapse sequence (§5b) is a one-way sequence: precision drops, then window narrows, then integration fails, and so on. Recovery is **not** the reverse of collapse.

**The bidirectional sequence:**

```
COLLAPSE                                RECOVERY
STAGE 1 — PRECISION DROP    R* ↓        STAGE 6' — PRECISION RESTORE    R* ↑
STAGE 2 — WINDOW NARROWING  W* ↓        STAGE 5' — WINDOW WIDENING      W* ↑
STAGE 3 — INTEGRATION FAIL  Θ* ↓        STAGE 4' — INTEGRATION RESTORE  Θ* ↑
STAGE 4 — RES FLOOR RISE    δ_min ↑     STAGE 3' — RES FLOOR FALL       δ_min ↓
STAGE 5 — GATE CLOSURE      Λ → 0       STAGE 2' — GATE REOPEN          Λ > 0
STAGE 6 — PRIOR CALCIF      𝒰 ≈ 0       STAGE 1' — PRIOR RE-UPDATE      𝒰 > 0
```

**The asymmetry:**

- **Collapse is passive.** The system loses precision as load rises. No active process is required. The stages occur in a topologically forced order because each stage causes the next.
- **Recovery is active.** The system must rebuild the competitive scaffold, restore the respiratory support, and re-establish the interoceptive routing. Rebuilding takes longer than degrading.
- **The hysteresis delay** ($\delta_{hyst}$, §2.3) makes recovery slower than collapse. The delay decays exponentially:

$$P_{recover}(t) = P(t) - \delta_{hyst}, \quad \frac{d\delta_{hyst}}{dt} = -\sigma \delta_{hyst}$$

**The recovery ladder.** Every domain has a recovery ladder — the order in which layers return. The recovery ladder is domain-specific. Central Reference cannot specify the ladder for every domain; it can only specify that every domain has one, and that the order is set by **substrate dependency** (§2.17): layers that depend directly on the substrate recover first; layers that depend on the full integration stack recover last.

**What the framework predicts:**

- Recovery signatures precede subjective reports.
- Recovery time scales super-proportionally with collapse depth.
- The recovery ladder is not the collapse ladder reversed — it is ordered by substrate dependency, not integration demand.

**Status:** The bidirectional model is operational in the speech projection. It requires confirmation in other domains.

## 5f. The Layer-Stack Collapse Ladder

The collapse sequence (§5b) is a **stage** sequence: it specifies the order in which the six stages of collapse occur. The layer stack (§2.16) is a **layer** sequence: it specifies the order in which the domain's output layers collapse.

They are related but not identical. The two orderings answer different questions.

**The relationship:**

| Collapse stage | What it specifies | Layer effect |
|---|---|---|
| Stage 1 — precision drop | When the collapse begins | All layers begin to degrade |
| Stage 2 — window narrowing | When the system loses flexibility | High-integration layers collapse first |
| Stage 3 — integration failure | When cross-domain binding fails | Integration-dependent layers collapse |
| Stage 4 — resolution floor rise | When small signals become invisible | Retrieval and grammar degrade |
| Stage 5 — gate closure | When the loop stops | Motor layers degrade |
| Stage 6 — prior calcification | When the system cannot update | Substrate layers degrade |

**The general rule:** stages determine **when** layers collapse. Layers determine **what** collapses first. The two are different dimensions of the same event.

**For the speech domain:** the eight layers are ordered by integration demand — pragmatic, discourse, prosodic, lexical, morphosyntactic, phonological, articulatory, breath. The stages determine when each layer begins to degrade.

**For another domain:** the layers will be different, and the mapping to stages may differ. But the two orderings — stage order and layer order — will both exist, and both will be forced by the domain's structure.

**Status:** The relationship is operational in the speech projection. It requires confirmation in other domains.

## 6. The Four Profiles

The branch condition is determined by the interaction of PE sensitivity, PE tolerance, encoding curvature, and routing capacity. Four profiles are distinguishable:

| Profile | $\sigma_{PE}$ | $\tau_{PE}$ | $K_{enc}$ | $I^*$ | Qualification Status |
|---|---|---|---|---|---|
| **High-gain, high-tolerance** | High | High | Low | High | **Qualified** — detects PE, gate stays open, loop runs, prior updates. Core profile for novel-domain decisions. |
| **High-gain, low-tolerance** | High | Low | Low | High | **Conditionally qualified** — detects PE but cascade fires. Qualified for structured tasks with recovery protocol. Requires $\tau_{PE}$ support (breathing, debrief intervals). |
| **Standard-gain, high $K_{enc}$** | Low | Any | High | Moderate | **Disqualified for novel domains** — doesn't detect PE, or suppresses it. Qualified only for domains where prior is known-valid and novel signals are absent. The "rigid expert" profile. |
| **Low $I^*$ (any gain)** | Low | Low | Any | Low | **Disqualified** — ambiguity unresolvable regardless of gain or tolerance. This is the clinical profile. Requires $I^*$ restoration before requalification. |

**The fourth profile is the most clinically important.** When $I^*$ collapses — through dissociation, chronic interoceptive avoidance, or interoceptive load — the system cannot resolve ambiguity regardless of its gain or tolerance. Avoidance becomes the default behavior. This is the behavioral signature Schäflein et al. (2018) documented: impaired interoceptive accuracy → compromised emotional learning → therapeutic avoidance.

**Behavioral signature by profile:**

| Profile | Behavior |
|---|---|
| High-gain, high-tolerance | Detects PE, gate stays open, loop runs, prior updates. Sustained engagement with ambiguity. |
| High-gain, low-tolerance | Detects PE, cascade fires, overwhelmed — shutdown or hyperarousal. The "sensitive but brittle" profile. |
| Standard-gain, high $K_{enc}$ | Doesn't detect PE, or PE suppressed by prior. Confident in stale model. The "rigid expert" profile. |
| Low $I^*$ (any gain) | Ambiguity unresolvable → avoidance default. The clinical profile — dissociation, avoidance disorders, chronic pain. |

## 7. The Hardware-Failure Chain

```
PRECISION DROP
    ↓
CBF drop (hypocapnia, hyperventilation)
    ↓
Oxygen delivery drop
    ↓
PV+ interneuron ATP depletion
    ↓
Inhibitory filtering failure
    ↓
Tuning curve broadening
    ↓
Feature axis entanglement (IM rises)
    ↓
Dimensionality contraction (W* × Θ* drops)
    ↓
Multi-hop inference collapses (n_hops drops)
    ↓
Path B default (prior retrieval)
    ↓
Loop does not run
```

**The hardware is PV+ interneurons. The failure mode is metabolic. The consequence is geometric. The behaviour is prior retrieval.**

---

# PART III — THE EMPIRICAL ANCHORS

Every claim is supported by existing literature. The framework is the map that shows how they fit together.

## 8. The Primary Anchors

| Anchor | Framework Claim | Citation | What It Confirms |
|---|---|---|---|
| A01 | The manifold exists and has geometry | [Citation needed — study confirmed, full reference not yet retrieved] | Neural manifolds are real, measured, functional |
| A02 | $A_s^*$ funds $W^*$ via $R^*$ | [Citation needed — study confirmed, full reference not yet retrieved] | HRV predicts cognitive performance |
| A03 | Intervention effects depend on baseline geometry | HRVB systematic review | "Inconsistent results" predicted by the formula |
| A04 | $\Theta^*$ is real and measurable | Dono et al. (2020) | Hemispheric laterality affects autonomic regulation |
| A05 | Containment cost raises $K$ independently | Reed et al. (2020) | Suppression depletes resources even when HRV is stable |
| A06 | Priors encoded under high $K$ carry curvature forward | Haghian et al. (2025) | Emotional encoding systematically distorts recall |
| A07 | Collapse proceeds radially inward | ADNI (2016) | Neurodegeneration follows predicted outer→inner sequence |
| A08 | Geometry must change before re-encoding works | Mathersul et al. (2024) | Baseline HRV moderates which therapy works |
| A09 | Social co-regulation restores $\Theta^*$ | [Citation needed — study confirmed, full reference not yet retrieved] | Every major civilization independently built synchronized rhythm |
| A10 | FND is $C_s \approx 0$ via $I^* \rightarrow 0$ | Maurer et al. (2016) | Structural absence confirmed; routing failure |
| A11 | Cached motor patterns reduce PFC overhead | Diedrichsen & Kornysheva (2015) | Motor automatisation produces measurable reduction |
| A12 | $I^*$ reports movement cost, gates prior encoding | Garfinkel et al. (2015); Craig (2009) | Interoceptive accuracy predicts prior formation |
| A13 | Unexplored physical range produces blank interoceptive zones | Moseley & Flor (2012) | Cortical body maps shrink with disuse |
| A14 | $I^*$ routes → signal amplifies | Petzschner et al. (2018) | Attention to heartbeat increases HEP amplitude |
| A15 | $I^*$ modulates peripheral physiology directly | Mizrachi et al. (2026) | Attention to inflamed area reduces inflammation |
| A16 | $I^* = I^*_{total} - I^*_{vision}$ | [Citation needed — study confirmed, full reference not yet retrieved] | Visual-interoceptive trade-off |
| A17 | Eyes closed restores $I^*$ | [Citation needed — study confirmed, full reference not yet retrieved] | Higher cardiac awareness predicts better balance |
| A18 | Precision is a timing-coherence ratio | Pratap et al. (2026) | PLV measures sync duration / timing distance |
| A19 | CO₂ tolerance window determines precision peak | Sakakibara et al. (1994) | Hypercapnia depresses cortical activity |
| A20 | Resonance breathing produces stable precision | Yamamoto et al. (2006) | Interhemispheric coherence increases with parasympathetic activation |
| A21 | Collapse hysteresis delays recovery | Reed et al. (2020) | Recovery time exceeds collapse time |
| A22 | Nasal respiration entrains limbic oscillations | Zelano et al. (2016) | Memory recall better during inhalation |
| A23 | CO₂ drives cerebral vasodilation | Raichle & Plum (1972) | Hyperventilation produces vasoconstriction |
| A24 | Slow breathing produces HRV and EEG coherence | Zaccaro et al. (2018) | Systematic review of slow breathing protocols |
| A25 | Breathing training shifts parameters | Kox et al. (2014) | Wim Hof practitioners show different autonomic responses |
| A26 | Control Pause measures $C_{high}$ individually | Cooper et al. (2003) | Buteyko trial — CP varies, shifts with training |
| A27 | Hypocapnia produces cognitive and anxiety collapse | Meuret & Ritz (2010) | Panic disorder characterized by low CO₂ |
| A28 | Feature interference is $K$ rising | Xue et al. (2026) | Axis entanglement in V1 confirmed causally |
| A29 | Hyperventilation impairs cognitive function | Tsukamoto et al. (2014) | CBF drop → cognitive impairment |
| A30 | PV+ interneurons are metabolically vulnerable | Kann et al. (2015) | Cellular mechanism for $K$ rise |
| A31 | ΔCBF/ΔCMRO₂ predicts neural efficiency | Hutchison & Rypma (2013) | Metabolic signature of high $K$ |
| A32 | Baseline vascular state sets activation ceiling | CVR literature | Physical constraint on outer edge |
| A33 | EEG-HRV coupling emerges during hyperventilation | Titov & Dick (2022) | Partial anchor for $R^* \rightarrow K$ |
| A34 | Path A/B = epistemic vs. extrinsic value | Friston et al. (2015) | Formal branch condition |
| A35 | Impaired IAc → emotional learning failure | Schäflein et al. (2018) | Behavioral endpoint of low $I^*$ |
| A36 | Stress narrows visual processing | Yang et al. (2026) | Cross-scale visual integration in V1 |
| A37 | HRV stressor signatures are distinct | Villatte et al. (2026) | Different loads reshape variables in specific ways |
| A38 | Methylphenidate increases dimensionality | Ni et al. (2022) | Pharmacological $K$ reduction improves performance |
| A39 | Working memory capacity ~5 items | Cowan (2016) | Dimensionality limit |
| A40 | Chunking compresses dimensions | Thalmann et al. (2019) | Effective compression of representations |
| A41 | Confirmation bias has no mechanistic account | Nickerson (1998) | 25-year gap — framework provides mechanism |
| A42 | System 1/System 2 branch | Kahneman (2011) | Path B / Path A described without naming |
| A43 | Deliberate practice requires edge-of-ability | Ericsson et al. (1993) | Structured loop-running |
| A44 | Expert recognition is compressed loop history | Klein (1998) | Recognition IS cheap retrieval |
| A45 | Intuition reliable in high-validity environments | Kahneman & Klein (2009) | Feedback IS error signal |
| A46 | Cognitive plasticity requires boundary operation | Lövdén et al. (2010) | Loop running on novel input |
| A47 | Neuroplasticity from skill learning | Draganski et al. (2004) | Loop writes into substrate |
| A48 | Plants exhibit adaptive behaviour | Trewavas (2003) | Slow loop at seasonal timescale |
| A49 | Plants habituate and retain learned responses | Gagliano et al. (2014) | Prior update from error signal exposure |
| A50 | Hot cache survives aging, RAM access degrades | Billot et al. (2026) | Outer edge degrades first |
| A51 | Competition is 25–40% of brain connections | Roy & Banerjee (2026) | Competitive scaffold is real |
| A52 | LP-ACC circuit detects change | Leow et al. (2026) | Cache miss controller identified |
| A53 | ACC activity scales with prediction error | Botvinick et al. (2001) | Biological loop detector |
| A54 | Beta oscillations signal prior maintenance | Engel & Fries (2010) | Measurable signature of loop suppression |
| A55 | Free-energy principle describes both paths | Friston (2010) | Path A/B in thermodynamic terms |
| A56 | Continuous wearable HRV measurement validates variance as signal at market scale | Oura, WHOOP, Garmin, Apple, Polar, Biostrap — documented features, hundreds of millions of device-days | HRV variance is real physiology, not measurement noise |
| A57 | Daily HRV variance predicts outcomes better than mean | Okawara et al. (2024) | The signal the field calls noise is the load trajectory |
| A58 | HRV follows circadian rhythm with individual chronotype variation | Vitale et al. (2019); Li et al. (2024) | Time-of-day is a feature, not noise |
| A59 | Glymphatic clearance drives interstitial solute clearance during slow wave sleep | Iliff et al. (2012); Grunewald et al. (2012) | Substrate for load recovery during sleep |
| A60 | Chronic vagal tone and CAP share efferent pathway | Tracey (2002); Thayer et al. (2010) | HRV is a real-time indicator of anti-inflammatory brake integrity |
| A61 | Masking requires continuous self-monitoring and self-correction | Richards & Gross (2000) | Expressive suppression consumes cognitive resources |
| A62 | The cost of masking comes from mismatch, not expression | Muparangi et al. (2021) | Surface acting (mismatch) exhausts; deep acting (alignment) does not |
| A63 | Masking is sustained displacement cost | Zenodo Displacement Framework (2026) | Formalization of cumulative masking cost |
| A64 | High masking effectiveness → high cost, late detection | Pearson & Rose (2021) | Social success paradox — passing predicts severe burnout |
| A65 | Emotional labor dissonance → burnout | Matteson & Miller (2012) | Occupational anchor for routing-cost mechanism |
| A66 | Masking is labor-intensive cognitive multitasking | Gassner (2025) | Expert synthesis — masking as executive function challenge |
| A67 | Masking hides collapse; visible on release | OSF preprint (2026) | Cumulative regulatory cycle with delayed strain release |

## 8b. Market-Scale Empirical Evidence

The Central Reference's Part III cites laboratory studies. A second class of evidence exists: **market-validated claims**.

Oura, WHOOP, Garmin, Apple, Polar, and Biostrap collectively represent hundreds of millions of device-days of continuous HRV data. Their entire product architecture — readiness scores, strain/recovery models, Body Battery, HRV trends, training load — is built on the assumption that HRV variance is signal, not noise. If the variance were noise, the products would be worthless.

The market has been validating the framework's central claim for a decade without any mechanistic account of why.

This is a different class of evidence from laboratory anchors. It is not "a paper confirmed X." It is "a global industry has been built on X being true, and the products work at scale." The signal-to-noise problem that lab studies struggle with is solved at market scale by sheer volume: variance is preserved because it is the measurement target.

**Implication for the framework:** The variance-as-signal claim does not need to be established empirically. It has been established. What the framework provides is the mechanistic account of *why* variance is meaningful — the load trajectory that the framework formalizes as $L^*$ and the collapse sequence.

**Implication for the field:** Prior null-result studies that averaged single readings across participants were structurally guaranteed to miss the effect. The variance they treated as noise is the signal the wearable market has been measuring continuously. This is not a critique of individual study designs — it is a structural account of a methodological assumption that has been incorrect in a specific, predictable way.

## 9. Perceptual Confirmation Across Sensory Systems

Every sensory domain that depends on integration degrades under load in the same geometric pattern. These studies were not designed to test this framework. The convergence is the evidence.

| Sensory Domain | Readout | Manifold Variable |
|---|---|---|
| Spatial—Visual | Colour constancy | $W^*$ |
| Spatial—Visual | Contrast sensitivity | $\sigma(A_s)$, $R^*$, $W^*$ |
| Spatial—Visual | Peripheral vision | $W^*$ |
| Spatial—Visual | Depth perception | $W^*$ |
| Temporal—Auditory | Rhythm perception | Phase-locking, $R^*$ |
| Temporal—Auditory | Speech-in-noise | $W^*$ |
| Temporal—Visual | Motion perception | $W^*$ |
| Semantic | Ambiguity resolution | $W^*$ |
| Semantic | Pronoun resolution | $W^*$ |
| Semantic | Garden-path recovery | $W^*$ |
| Semantic | Prosody interpretation | $W^*$ |
| Semantic | Phoneme discrimination | $\sigma(A_s)$, $R^*$ |
| Interoceptive | Temperature perception | $W^*$ |
| Interoceptive | Pain sensitivity | $K$, $W^*$ |
| Interoceptive | Heartbeat perception | $R^*$ |
| Social | Face perception | $W^*$, $K$ |
| Social | Theory of Mind | $W^*$ |
| Social | Threat detection | $K$ |
| Motor | Coordination | $\sigma(A_s)$ |
| Motor | Reaction time variability | $\sigma(A_s)$ |
| Motor | Fine motor control | $R^*$ |
| Mnemonic | Episodic coherence | $W^*$ |
| Mnemonic | Temporal ordering | $W^*$ |
| Decision | Future horizon | $W^*$ |
| Decision | Risk perception | $K$ |

---

# PART IV — THE PREDICTIONS

Every prediction is falsifiable. Each specifies IV, DV, operationalization, and falsification condition.

*Note: v1.7 does not add new predictions. All predictions from v1.6 remain as they were. The new sections (§2.18, §3.19) are structural, not predictive. Future domain projections will register their own predictions in their own papers; Central Reference registers the general rules those predictions will test. PREDICT-SPEECH-58, -59, and -60 (the speech projection's routing predictions) are registered in The Spoken Language Paper v3.1 and are restated here as the framework-level forms.*

### PREDICT-EXPR-01: Congruence Is Predicted by Expression Ratio, Not Amplitude

Prosodic congruence — the match between voice and reported load — is predicted by $f_{expression}$, not by $A_s^*$ or $\Pi_{cog}$ alone. Two systems with the same amplitude and load but different expression ratios show different congruence.

| Field | Content |
|---|---|
| **IV** | $f_{expression}$ (operationalized via independent manipulation of output-management demand) |
| **DV** | Congruence (corr between output expressiveness and load self-report) |
| **Control** | $A_s^*$, $\Pi_{cog}$ |
| **Operationalization** | Measure output expressiveness and load self-report under conditions that vary output-management demand at matched amplitude and load. |
| **Falsification** | If congruence is not predicted by $f_{expression}$ beyond $A_s^*$ and $\Pi_{cog}$, the expression model is disconfirmed. |
| **Status** | Untested — speech-domain version is PREDICT-SPEECH-58 |

### PREDICT-EXPR-02: Chronic Low Expression Predicts Later Collapse Detection

Chronic low $f_{expression}$ predicts later collapse detection. Maskers reach Stage 3–4 before reporting Stage 1–2 symptoms, compared to non-maskers at the same precision level.

| Field | Content |
|---|---|
| **IV** | Chronic $f_{expression}$ (measured longitudinally) |
| **DV** | Stage at first collapse detection |
| **Operationalization** | Longitudinal tracking of $f_{expression}$ and collapse-stage detection across a cohort. Compare detection stage in chronic-low vs. chronic-high $f_{expression}$ groups at matched precision. |
| **Falsification** | If chronic low $f_{expression}$ does not predict later collapse detection, the masking-to-late-detection mechanism is disconfirmed. |
| **Status** | Untested — speech-domain version is PREDICT-SPEECH-59 |

### PREDICT-EXPR-03: Masking Has a Measurable Load Cost

Allostatic load is higher in high-$A_s^*$, low-$f_{expression}$ systems than in high-$A_s^*$, high-$f_{expression}$ systems. The mask has a measurable cost.

| Field | Content |
|---|---|
| **IV** | $A_s^*$, $f_{expression}$ |
| **DV** | $L^*$ (composite load) |
| **Operationalization** | Cross-sectional and longitudinal comparison of $L^*$ across the four expression states (high/low amplitude × high/low expression). |
| **Falsification** | If allostatic load is not higher in high-$A_s^*$, low-$f_{expression}$ systems, the masking-cost mechanism is disconfirmed. |
| **Status** | Untested — speech-domain version is PREDICT-SPEECH-60 |

---

# PART V — COHESION CHECK

*The cohesion check from v1.5 is preserved. v1.6 and v1.7 additions are structural. The only additions to the cohesion check are: (1) the three new structures from v1.6 (supply, demand, channel axes; layer stack; recovery ladder), registered in §19; (2) the three new constructs from v1.7 ($f_{expression}$, congruence, $\lambda_{mask}$), registered in §19 and §20.*

---

# PART VI — VERSION HISTORY

## 23. This Specification

| Version | Date | Changes |
|---|---|---|
| v1.7 | 2026-09-20 | Domain-projection-aligned specification. Absorbed the expression/congruence/masking constructs from The Spoken Language Paper v3.1. New sections: §2.18 (expression and congruence), §3.19 (expression equation). New variables: $f_{expression}$, $\lambda_{mask}$. New anchors: A61–A67 (masking-cost literature). New framework-level predictions: PREDICT-EXPR-01, -02, -03 (restatements of speech-domain predictions). Updated §2.4 (note on $f_{routing}$ vs. $f_{expression}$), §4 (glymphatic ODE gains $\lambda_{mask}$), §19 (consistent variables), §20 (drift — historical name note), §21 (composition — expression interaction question), §22 (open questions — functional forms), §24 (cite Spoken Language Paper v3.1), §25 (projection-layer alignment), new §26 (Speech Projection Alignment). |
| v1.6 | 2026-09-19 | Domain-projection-complete specification. Absorbed the general structural lessons from the first full domain projection (The Spoken Language Paper v3.0). New sections: §2.15 (three axes of collapse shape), §2.16 (integration-demand rule and layer stacks), §2.17 (collapse-recovery asymmetry), §3.16 (demand-axis form), §3.17 (channel-cost form), §3.18 (recovery-rate form), §5e (bidirectional collapse sequence), §5f (layer-stack collapse ladder), §18b (domain-projection methodology), §22d (domain-projection open questions), §22e (confounds in domain projection). Updated §19 (variables consistent), §20 (drift), §21 (composition), §22 (open questions), §23 (version history), §24 (supporting papers), §25 (stack), §26 (one line). |
| v1.5 | 2026-09-13 | Full stack convergence. Absorbed bidirectional supplies from MS v7.2, Precision v3.4, AL v2.1, GoI v1.0, and Loop v1.0. New sections: §2.12 (somatic commutation), §2.13 (breath phase timing), §2.14 (four-layer cache hierarchy), §3.13 (full dynamic $P(t)$), §3.14 (temporal dynamics), §3.15 (resonance breathing as third mechanism), §4a (four contracts), §4b (streams being measured), §5c (exhale gate trap), §5d (breath phase and thought timing), §22c (confounds). Updated §20 (drift), §21 (composition), §25 (stack). Single-document specification achieved. |
| v1.4 | 2026-09-12 | Variable registry completed. §2.8: added $O_{pathway}$ with functional form note. §2.9: added $L^*_{critical,i}$ with calibration note. New §2.11: motor gain variables with threshold calibration note. §22: added open question 15 on $M_{state}$ threshold calibration. Every variable referenced in the equation registry now has a defined entry in the variable registry. |
| v1.3 | 2026-09-12 | Intelligence–REQT bridge sentence added to §3.7. REQT weight inconsistency resolved with justification note. §2.8 metabolic pathway note added. Two composition questions added to §21. Two open questions added to §22. Operational reader routing added to Part 0. |
| v1.2 | 2026-09-12 | Allostatic Load measurement layer integrated. §2.10 load decomposition. §2.3 $C_{high}(L^*)$ compression. §3.3 load-dependent precision. §3.7 component REQT. §4 glymphatic recovery loop. §5b zone correspondence table. §8b market-scale evidence + A56–A60. §16 ND cohort predictions, delta HRV probe, composite load predictions, component REQT prediction. §22b structural account of prior null results. |
| v1.1 | 2026-09-12 | REQT integration. §1 intelligence equation cleaned to single expression. §2.9 qualification variables added. §3.7 REQT equation + 3 notes. §5b collapse sequence added. §6 qualification status column. PREDICT-REQT-01, -02, PREDICT-BREATH-01 added. Citation flags in §8. Adventurousness note added. |
| v1.0 | 2026-09-11 | Complete specification — all mechanisms integrated, all gaps closed. Includes: full variable registry, full equation registry, complete causal chain, 55 empirical anchors, 40+ falsifiable predictions, cohesion check, composition questions resolved, four-profile table, hardware-failure chain, $L^*/\Pi_{cog}$ mapping, $J(C) \to \eta$ rationale, $n_{hops}$ connection to intelligence definition, PREDICT-LOOP-01 through 03 |

## 24. Supporting Papers

| Paper | Version | Function | DOI |
|---|---|---|---|
| **The Manifold Schema** | v7.2 | Canonical framework — all state variables, all equations | 10.5281/zenodo.21939440 |
| **Precision, Timing, and the Oscillatory Source** | v3.4 | $R^*$ definition — $P = R/D_T$, CO₂, two-factor pressure, temporal dynamics | 10.5281/zenodo.22179675 |
| **The Geometry of Inference** | v1.0 | Biological implementation — LP-ACC, four-layer cache, gate condition, somatic commutation, exhale gate trap, breath phase timing | pending |
| **Allostatic Load as Accumulated Regulatory Debt** | v2.1 | Measurement layer — $L^*$ decomposition, four contracts, delta HRV, zones, composite equation | pending |
| **The Loop Is the Intelligence** | v1.0 | Domain projection: intelligence as the loop | pending |
| **The Spoken Language Paper** | v3.1 | First full domain projection — three axes, eight-layer stack, collapse-recovery asymmetry, expression ratio, congruence, masking, 60 predictions | pending |
| **The Hallucination You Are Having Right Now** | — | Substrate-agnostic hallucination theory | 10.5281/zenodo.21922044 |
| **Physics as the Missing Component in Medical Science** | — | Physical substrate | 10.5281/zenodo.21512678 |
| **Unified Regulatory Model** | — | Implementation architecture | 10.5281/zenodo.20417459 |
| **The Context Oscillator** | — | Context window architecture | 10.5281/zenodo.21811408 |
| **The Profile of a Person That Is AGI** | — | AGI as system property | 10.5281/zenodo.21921714 |
| **Dual-Substrate Cognition Architecture** | — | Human-AI co-processing | 10.5281/zenodo.21362260 |
| **Hallucinations Are Not Random** | — | AI hallucination mechanism | 10.5281/zenodo.21244811 |
| **The Geometry Beneath the Category** | v1.0 | Substrate premise — convergence point for ND, orientation, speech, cosmetic papers | pending |
| **Regulatory-Engine Qualification for Complex Decision-Making** | — | Governance-facing REQT artifact | pending |

## 25. The Stack

Central Reference v1.7 is the single specification. The stack is:

```
                         Central Reference v1.7
                         (this document — the specification)
                                    │
                ┌───────────────────┼───────────────────┐
                │                   │                   │
                ▼                   ▼                   ▼
        Manifold Schema      Precision v3.4       Allostatic Load
            v7.2                (formalisms)         v2.1
        (canonical)                              (measurement)
                │                   │                   │
                └───────────────────┼───────────────────┘
                                    │
                    ┌───────────────┼───────────────┐
                    │               │               │
                    ▼               ▼               ▼
            Geometry of        Loop Is the       Other domain
              Inference        Intelligence      projections
               v1.0               v1.0           (hallucination,
            (biology)          (argument)         AGI, URM, etc.)
                                    │
                    ┌───────────────┼───────────────┐
                    │               │               │
                    ▼               ▼               ▼
            The Spoken        The Geometry      Other domain
            Language          Beneath the       projections
            Paper v3.1        Category v1.0     (identity, appearance,
            (speech           (substrate         movement, etc.)
            projection)       premise)
```

**The projection layer** is the set of papers that apply Central Reference's general mechanism to a specific domain. Each projection:

- Identifies the domain's three axes
- Identifies the domain's layer stack
- Specifies the domain's collapse and recovery ladders
- Registers domain-specific predictions

**The Spoken Language Paper** is the first fully documented projection. It established the methodology (§18b) that future projections will follow, and it produced the general constructs registered in §2.18 (expression, congruence, masking).

**Citation rule for projections:** A domain projection cites Central Reference v1.7 alone, unless it is specifically extending one of the supporting papers. The projection is a **readout** of Central Reference, not a new specification.

**Reading order for a new reader:** Central Reference v1.7 first. It contains everything. The supporting papers are for depth on specific layers. The domain projections are for specific domains.

**Update rule:** Any new mechanism or variable must be added to Central Reference first. The supporting papers and domain projections then reference Central Reference, not vice versa.

## 26. Speech Projection Alignment

The Spoken Language Paper v3.1 was written before Central Reference absorbed its general constructs. The two documents describe the same system, but the speech paper uses language that Central Reference has since renamed or re-scoped. This note records the alignment so that a reader moving between the two documents is not confused.

**The two name collisions:**

1. **The speech paper's \( f_{routing} \) is Central Reference's \( f_{expression} \).** The speech paper defines \( f_{routing} \) as the proportion of available salience that reaches expression. Central Reference reserves \( f_{routing} \) for one of the three components of \( I^* \) (§2.4), and registers the proportion-of-salience-reaching-expression as \( f_{expression} \) (§2.18). The speech paper's variable is \( f_{expression} \); its name is a historical artifact.

2. **The speech paper's "routing" language is Central Reference's "expression" language.** Where the speech paper says "routing to output management," Central Reference says "low \( f_{expression} \)." Where the speech paper says "congruence," Central Reference says "the operational readout of \( f_{expression} \)." The mechanism is the same.

**What is unaffected:**

- The four-state table (high/low \( A_s^* \) × high/low \( f_{expression} \)) is unaffected. It is a statement about \( f_{expression} \), regardless of what the speech paper called it.
- The masking profile table is unaffected. It is a statement about \( f_{expression} \), not about the framework's \( f_{routing} \).
- The predictions PREDICT-SPEECH-58, -59, and -60 are unaffected. They are statements about \( f_{expression} \), and they are restated as framework-level predictions (PREDICT-EXPR-01, -02, -03) in Part IV.
- The masking mechanism is unaffected. It is anchored in the load pathway through \( \lambda_{mask} \), regardless of the name of the variable it depends on.

**The alignment direction:** The speech paper will be updated to v3.2 with the renamed variable and the adopted decomposition. Central Reference v1.7 is the specification; the speech paper aligns to it, not the reverse.

## 27. The One Line

> The brain is an energy budget allocation system operating on priors. The breath is the source. The geometry is the mechanism. The prior is the output. Every phenomenon in this document — flow, collapse, fear, trauma, savant capacity, clinical states, social fragmentation, AI hallucination, and the masking of any of them — is one variable changing in one equation. The variable is geometry. The equation is the master equation. The expression ratio determines whether the geometry is visible. In any domain, the shape of the collapse is determined by three axes: supply, demand, and channel. The order of collapse is determined by integration demand. The order of recovery is determined by substrate dependency. These rules are general. The domains are projections.

---

*End of specification.*

**Version:** 1.7
**Date:** 2026-09-20
**Status:** Domain-projection-aligned specification
**Next version:** v1.8 — after the first round of domain projections beyond speech, or v2.0 — if any mechanism requires revision

---

# What This Paper Contributes — For The Spoken Language Paper v3.2

*Note for the speech paper: this section is added to the speech paper, not to Central Reference. It names the speech paper's role as the first fully documented domain projection, now aligned with the specification.*

---

The Spoken Language Paper is the **first fully documented domain projection** of the loop framework. It has produced two waves of general constructs:

**v1.6 wave — structural.** The three axes (supply, demand, channel), the integration-demand rule, the collapse-recovery asymmetry, and the domain-projection methodology. These are now general structures in Central Reference §2.15–2.17, §18b, §5e–5f.

**v1.7 wave — variable-level.** The expression ratio \( f_{expression} \), the congruence measure, and the masking load term \( \lambda_{mask} \). These are now general variables in Central Reference §2.18, §3.19, and §4.

**What remains speech-specific:** The eight-layer stack, the specific layer order, the specific recovery ladder, the specific suprasegmental demand axis, the specific channel costs, the 60 speech-domain predictions, and the clinical/regional/social projections in Books IV–V. These are discoveries about the speech domain, not about the framework.

**The alignment the speech paper needs:** Rename its \( f_{routing} \) to \( f_{expression} \), adopt Central Reference's \( I^* \) decomposition, anchor masking in the \( \lambda_{mask} \) term, and adopt the load-self-report comparator for congruence. The mechanism does not change. The names do.

**For future projections:** the speech paper is the template. Read it before projecting a new domain. The methodology is documented in Central Reference §18b; the case study is The Spoken Language Paper v3.1. The two waves of general constructs it produced — structural (v1.6) and variable-level (v1.7) — are the model of what a successful projection contributes back to the specification.

**The general lesson:** when the framework is applied to a new domain, the domain's layer count, axis count, recovery order, expression ratio form, and masking load coefficient are discoveries, not predictions. The projection paper is the discovery. The complexity the projection reveals is the domain's complexity, not the framework's.
