# Central Reference v1.5

**A Unified System Specification for the Loop Framework**

**Robinson, 2026**

**Version:** 1.5
**Date:** 2026-09-13
**Status:** Full stack convergence — absorbs bidirectional supplies from MS v7.2, Precision v3.4, AL v2.1, GoI v1.0, and Loop v1.0. Single-document specification achieved.
**Purpose:** This document is the complete, standalone specification of the loop framework. A reader can use this document alone to understand the system, run the tests, and verify the predictions. Every variable, every equation, and every mechanism that appears in any of the supporting papers is defined here. Future papers should cite Central Reference v1.5 alone.

---

## Changelog — v1.4 → v1.5

This changelog exists so that any reader — human or AI — can see the convergence path. Central Reference v1.4 was the variable-registry-complete specification. Central Reference v1.5 is the full-stack-converged specification: it absorbs the bidirectional supplies from every other document in the stack so that future papers can cite Central Reference alone.

| Step | Change | Source | Location |
|---|---|---|---|
| 1 | Version bumped to v1.5 | — | Header |
| 2 | §2.12 — Somatic commutation variables | GoI v1.0 §3.4, §8 | Variable Registry |
| 3 | §2.13 — Breath phase timing variables | GoI v1.0 §9 | Variable Registry |
| 4 | §2.14 — Four-layer cache hierarchy | GoI v1.0 §1.1 | Variable Registry |
| 5 | §3.13 — Full dynamic $P(t)$ equation | Precision v3.4 §2.3 | Equation Registry |
| 6 | §3.14 — Temporal dynamics | Precision v3.4 Part IV | Equation Registry |
| 7 | §3.15 — Resonance breathing as third precision mechanism | Precision v3.4 §1.8 | Equation Registry |
| 8 | §4a — Four contracts as mechanism chain | AL v2.1 §2 | Causal Chain |
| 9 | §4b — The streams being measured | Precision v3.4 §1.9 | Causal Chain |
| 10 | §5c — Exhale gate trap cascade | GoI v1.0 §6.3, §8.3 | Collapse |
| 11 | §5d — Breath phase and thought timing | GoI v1.0 §9 | Collapse |
| 12 | §22c — Confounds and limitations | AL v2.1 §9c | Open Questions |
| 13 | §20 — Variables with drift updated | — | Cohesion Check |
| 14 | §21 — Composition questions resolved updated | — | Cohesion Check |
| 15 | §25 — The stack (all six documents) | — | Closing |
| 16 | Version history updated | — | Version History |
| 17 | Supporting papers updated | — | Supporting Papers |

**Why this is the last assembly for the specification layer:** Central Reference v1.4 completed the variable registry. Central Reference v1.5 completes the mechanism registry. Every mechanism in the supporting papers is now either defined in Central Reference or explicitly delegated. The stack is closed. Future papers are projections, not extensions.

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
| $f_{routing}$ | Routing component | $I^*_{total} - \sum_i P_i W_i$ |
| $f_{gain}$ | Gain component | Sigmoid gain control |
| $f_{sensorium}$ | Sensorium component | Available routing / required routing |
| $I^*$ decomposition | Full form | $I^* = f_{routing} \cdot f_{gain} \cdot f_{sensorium}$ |

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
│   Variables: S
│
├── S = C_s · I*
└── I* = C_total − ∑ P_i · W_i
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
│   Variables: SWS%, L*, clearance rate
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
│
└── Load trajectory:
    dL*/dt = λ_met + λ_inflam − λ_clear · SWS%(L*)

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

## 10. Core Predictions

### P1: LLMs fail on tasks requiring genuine novel error detection

| Field | Content |
|---|---|
| **IV** | Task type (novel vs. training-analog) |
| **DV** | Performance accuracy, error-detection rate |
| **Operationalization** | Novel tasks with no training analog requiring iterative self-correction. Measure whether model detects its own errors without human prompt. |
| **Falsification** | If LLM detects and corrects novel errors without human intervention, P1 is disconfirmed. |
| **Status** | Untested |

### P2: Prompt engineering skill correlates with high-gain profile, not IQ

| Field | Content |
|---|---|
| **IV** | High-gain profile (sensory sensitivity scale, interoceptive accuracy, baseline HRV) |
| **DV** | Prompt engineering skill (blind evaluation on novel tasks) |
| **Control** | IQ |
| **Operationalization** | Recruit expert prompt engineers (n > 30) and matched controls. Measure high-gain profile, IQ, prompt skill. Regress prompt skill on high-gain profile controlling for IQ. |
| **Falsification** | If prompt skill correlates with IQ more than high-gain profile, P2 is disconfirmed. |
| **Status** | Untested — the gap no study has looked for |

### P3: Output quality tracks human loop quality, not model size

| Field | Content |
|---|---|
| **IV** | Human expertise (domain-specific loop history) |
| **DV** | Joint output quality |
| **Control** | Model size (hold constant) |
| **Operationalization** | Same model, same task, varied human expertise. Measure output quality. |
| **Falsification** | If output quality tracks model size more than human expertise, P3 is disconfirmed. |
| **Status** | Untested |

### P4: Confirmation bias rate correlates inversely with CO₂ tolerance

| Field | Content |
|---|---|
| **IV** | CO₂ tolerance (BOLT score, capnometry) |
| **DV** | Prior-updating rate on novel evidence |
| **Control** | IQ |
| **Operationalization** | Measure CO₂ tolerance and prior-updating behavior. Regress prior-updating on CO₂ tolerance controlling for IQ. |
| **Falsification** | If CO₂ tolerance does not predict prior-updating, P4 is disconfirmed. |
| **Status** | Untested |

### P5: Institutions that stop measuring outcomes produce LLM-equivalent confabulation

| Field | Content |
|---|---|
| **IV** | Outcome measurement frequency |
| **DV** | Confabulation rate |
| **Operationalization** | Case studies: policy, corporate strategy, AI safety framing. |
| **Falsification** | If institutions without outcome measurement do not show confabulation patterns, P5 is disconfirmed. |
| **Status** | Untested |

### P6: Any further loop implementation in AI produces proportional performance gain

| Field | Content |
|---|---|
| **IV** | Loop implementation level (zero, one pass, full iteration, extended budget) |
| **DV** | Performance gain on reasoning tasks |
| **Operationalization** | Compare standard completion, CoT, Self-Refine, Tree of Thoughts, o1 extended thinking. Measure gain per loop iteration. |
| **Falsification** | If gain plateaus before full loop implementation, P6 is disconfirmed. |
| **Status** | Partially confirmed — every technique that improved performance added loop implementation |

### P7: Masters who stop encountering novel problems show measurable CO₂ tolerance drop within 5 years

| Field | Content |
|---|---|
| **IV** | Novel problem exposure (longitudinal) |
| **DV** | CO₂ tolerance (BOLT score, capnometry) |
| **Control** | Age, baseline fitness |
| **Operationalization** | Longitudinal measurement of CO₂ tolerance in masters who stop vs. continue encountering novel problems. |
| **Falsification** | If CO₂ tolerance does not drop in the non-novel group, P7 is disconfirmed. |
| **Status** | Untested |

### P8: OpenAI's next model will show diminishing returns on novel reasoning tasks despite scaling

| Field | Content |
|---|---|
| **IV** | Model version (o1 → o2 → o3) |
| **DV** | Performance on tasks requiring genuine salience navigation |
| **Operationalization** | Benchmark tasks with no training analog. Compare performance trajectory against scaling trajectory. |
| **Falsification** | If novel reasoning performance scales proportionally with compute, P8 is disconfirmed. |
| **Status** | Untested |

### P9: Baseline CO₂ tolerance predicts salience dependence for deep inference

| Field | Content |
|---|---|
| **IV** | Baseline CO₂ tolerance (BOLT score, capnometry, Control Pause) |
| **DV** | Performance difference on novel reasoning tasks with vs. without preceding salience trigger |
| **Operationalization** | Measure baseline CO₂ tolerance. Present novel reasoning tasks in two conditions: (a) cold start, (b) after salience trigger. Compare performance difference. |
| **Falsification** | If baseline CO₂ tolerance does not predict salience dependence, P9 is disconfirmed. |
| **Status** | Untested — standard capnometry and cognitive task sufficient |

## 11. Precision Predictions

### PREDICT-PREC-01: CO₂ Tolerance Window Produces Precision Peak

Precision $P(t)$ will follow the CO₂ tolerance curve: rising with CO₂ until $C_{high}$, peaking at $C_{peak}$, then collapsing as $J(C)$ increases. The peak will occur before $C_{high}(L^*)$.

| Field | Content |
|---|---|
| **Test** | Continuous HRV, CO₂ (capnometry), EEG phase coherence during breath-hold |
| **Confirmed if** | Precision trajectory matches the CO₂ tolerance curve |
| **Disconfirmed if** | Precision continues to rise with CO₂ until hypercapnia collapse |
| **Status** | Untested |

### PREDICT-PREC-02: Mechanical and Cognitive Pressure Have Opposite Effects

Mechanical pressure (breath-hold) increases precision; cognitive pressure (load) decreases it.

| Field | Content |
|---|---|
| **Test** | Measure precision under (a) breath-hold and (b) cognitive load with matched subjective effort |
| **Confirmed if** | Mechanical pressure increases precision; cognitive pressure decreases it |
| **Disconfirmed if** | Both pressure sources decrease precision |
| **Status** | Untested |

### PREDICT-PREC-03: Jitter Tracks CO₂ Above Tolerance

Jitter $J(t)$ is zero below $C_{high}(L^*)$, grows as $\kappa(C - C_{high}(L^*))^2$ above.

| Field | Content |
|---|---|
| **Test** | Measure phase jitter (EEG) and HRV variability during breath-hold. Correlate with capnometry. |
| **Confirmed if** | Jitter is chemoreflex-driven — quadratic growth confirmed |
| **Disconfirmed if** | Jitter does not track CO₂ above tolerance |
| **Status** | Untested |

### PREDICT-PREC-04: Resonance Breathing Produces Stable Precision

Resonance breathing (≈6 breaths/min) produces stable precision with low jitter and low collapse risk.

| Field | Content |
|---|---|
| **Test** | Compare precision, jitter, flow duration under resonance breathing vs. breath-hold |
| **Confirmed if** | Resonance produces stable, sustainable precision |
| **Disconfirmed if** | No measurable precision increase beyond normal breathing |
| **Status** | Untested |

### PREDICT-PREC-05: Collapse Hysteresis Delays Recovery

After precision collapse, recovery is delayed by $\delta_{hyst}$ which decays exponentially.

| Field | Content |
|---|---|
| **Test** | Induce precision collapse. Measure precision recovery rate. Correlate with HRV recovery and sympathetic markers. |
| **Confirmed if** | Recovery is slower than collapse |
| **Disconfirmed if** | Recovery is symmetric |
| **Status** | Untested |

### PREDICT-PREC-06: Precision Predicts Motor Gain

Motor gain $G_m = \alpha P - \beta \eta$ correlates with precision $P$ during movement tasks.

| Field | Content |
|---|---|
| **Test** | Measure EEG phase coherence and EMG amplitude during precision movement tasks |
| **Confirmed if** | Precision predicts motor gain |
| **Disconfirmed if** | Motor gain is independent of precision |
| **Status** | Untested |

### PREDICT-PREC-07: Encoding Quality is Precision-Weighted Time

Memory encoding quality correlates with $\int_{t_{enc}} P(t) dt$ — independent of exposure time.

| Field | Content |
|---|---|
| **Test** | Measure precision during encoding. Test recall at 1-day and 1-week. |
| **Confirmed if** | Precision-weighted time predicts memory quality |
| **Disconfirmed if** | Exposure time alone predicts memory quality |
| **Status** | Untested |

### PREDICT-PREC-08: Cross-Frequency Coupling Predicts Integration

Precision measured across frequency bands (CFC) predicts $\Theta^*$ better than single-band precision.

| Field | Content |
|---|---|
| **Test** | Measure multi-band EEG and HRV during flow-inducing tasks. Compute precision across band pairs. |
| **Confirmed if** | CFC precision predicts integration |
| **Disconfirmed if** | Single-band precision is sufficient |
| **Status** | Untested |

### PREDICT-PREC-09: CO₂ Tolerance Is Trainable

$C_{low}$ and $C_{high}$ shift with breathwork training. $C_{high}$ increases, $C_{peak}$ shifts upward, precision lock duration extends.

| Field | Content |
|---|---|
| **Test** | Measure CO₂ tolerance and precision before/after 4-week breathwork training |
| **Confirmed if** | Tolerance window shifts with practice |
| **Disconfirmed if** | No training effect |
| **Status** | Partially supported — Kox et al. (2014) confirms parameters shift |

### PREDICT-PREC-10: Baseline CO₂ Tolerance Predicts Salience Dependence

Individuals with low baseline CO₂ tolerance will require a salience-induced breath interruption to enter deep inference. Individuals with high baseline CO₂ tolerance will not.

| Field | Content |
|---|---|
| **Test** | Measure baseline CO₂ tolerance. Present novel reasoning tasks with vs. without preceding salience trigger. |
| **Confirmed if** | Low CO₂ tolerance group shows large improvement after trigger; high CO₂ tolerance group shows little difference |
| **Disconfirmed if** | Baseline CO₂ tolerance does not predict salience dependence |
| **Status** | Untested |

## 12. Prediction Error Predictions

### PREDICT-PE-01: High CO₂ Tolerance Sustains PE Engagement

High CO₂ tolerance profiles will show sustained HRV coherence and maintained $W^*$ during PE exposure where standard profiles show HRV disruption and performance drop.

| Field | Content |
|---|---|
| **IV** | CO₂ tolerance (Control Pause, capnometry) |
| **DV** | HRV coherence duration, $W^*$ maintenance, performance |
| **Operationalization** | PE exposure task with continuous HRV. Compare high-tolerance vs. low-tolerance profiles. |
| **Falsification** | If CO₂ tolerance does not predict sustained HRV coherence during PE, $\tau_{PE}$ model is disconfirmed. |
| **Status** | Untested |

### PREDICT-PE-02: Identity-Protective Cognition Is Preceded by K Rise

Identity-protective cognition will be preceded by measurable $K$ rise within the same trial.

| Field | Content |
|---|---|
| **IV** | Identity-threatening vs. neutral PE |
| **DV** | HRV drop (within-trial), window narrowing (behavioural) |
| **Operationalization** | Within-trial HRV and behavioural measures during identity-threatening PE vs. neutral PE. |
| **Falsification** | If $K$ rise does not precede identity-protective response within trial, cascade model is disconfirmed. |
| **Status** | Untested |

### PREDICT-PE-03: Avoidance Shows Same Mechanism as High K

Avoidance under degraded interoceptive resolution shows the same mechanism as avoidance under high $K$.

| Field | Content |
|---|---|
| **IV** | $I^*$ manipulation (interoceptive load, breath manipulation) |
| **DV** | Avoidance behaviour, $\delta_{min}$, $IM$ |
| **Operationalization** | Measure $I^*$, $\delta_{min}$, and avoidance under controlled $I^*$ manipulation. |
| **Falsification** | If $I^*$ degradation does not produce avoidance, shared mechanism model is disconfirmed. |
| **Status** | Untested |

### PREDICT-PE-04: Metabolic Version — HRV Coherence Predicts IM

HRV coherence ($R^*$ proxy) negatively predicts $IM$ (feature interference). Mediated by $\Delta CBF/\Delta CMRO_2$.

| Field | Content |
|---|---|
| **IV** | Respiratory condition (normal vs. hyperventilation vs. slow breathing) |
| **DV** | $IM$ (feature interference, Xue et al. paradigm) |
| **Mediator** | $\Delta CBF/\Delta CMRO_2$ ratio (calibrated fMRI) |
| **Moderator** | Baseline CVR |
| **Operationalization** | Within-subject design. Measure HRV (PLV), calibrated fMRI, and $IM$ under three breathing conditions. |
| **Falsification** | If $R^*$ does not predict $IM$, or if $\Delta CBF/\Delta CMRO_2$ does not mediate, metabolic mechanism is disconfirmed. |
| **Status** | Untested |

## 13. Motor Encoding Predictions

### PREDICT-MOTOR-01: Movement Vocabulary Predicts Distortion Topography

Individuals with wider cached movement vocabulary will show less manifold distortion under equivalent load, controlling for baseline HRV.

| Field | Content |
|---|---|
| **Test** | Movement vocabulary assessment + cognitive load task + continuous HRV |
| **Confirmed if** | Distortion topography is a motor vocabulary inventory |
| **Disconfirmed if** | Distortion distributed by parallel mechanism |
| **Status** | Untested |

### PREDICT-MOTOR-02: Geometry Change Precedes Prior Update

Introducing a novel movement pattern and holding it until interoceptive signal stabilizes produces measurable prior update faster than cognitive intervention alone.

| Field | Content |
|---|---|
| **Test** | RCT: movement-first vs. cognitive-first intervention matched for time |
| **Confirmed if** | Sequencing is the active variable |
| **Disconfirmed if** | Narrative and movement update priors via parallel channels |
| **Status** | Untested |

## 14. Somatic Commutation Predictions

### PREDICT-INF-08: Somatic Commutation Modulates C_LR

Horizontal eye movements and cervical rotation dynamically modulate interhemispheric phase-locking coherence.

| Field | Content |
|---|---|
| **Test** | Measure EEG inter-hemispheric coherence during controlled horizontal saccades |
| **Confirmed if** | Gaze laterality predicts $C_{LR}$ |
| **Disconfirmed if** | Gaze direction does not modulate $C_{LR}$ |
| **Status** | Untested |

### PREDICT-INF-09: RSA Phase Gates Track-Switching Accuracy

The accuracy of cognitive state-switching depends on RSA phase. Switches during inhale are more successful than switches during exhale.

| Field | Content |
|---|---|
| **Test** | Task-switching paradigm with RSA phase locked to trial onset |
| **Confirmed if** | Switch accuracy and latency differ by RSA phase |
| **Disconfirmed if** | RSA phase does not predict switch performance |
| **Status** | Untested |

### PREDICT-INF-10: Breath Phase Determines Thought Timing

Theta/gamma coupling decreases either gradually across exhalation or abruptly at the chemoreceptor threshold.

| Field | Content |
|---|---|
| **Test** | Continuous EEG during slow exhalation with concurrent capnometry |
| **Confirmed if (gradual)** | Coupling decreases smoothly with CO₂ rise |
| **Confirmed if (threshold)** | Coupling drops abruptly at $C_{high}(L^*)$ |
| **Disconfirmed if** | Coupling is not phase-dependent |
| **Status** | Untested |

### PREDICT-INF-11: Exhale Gate Trap Is Reversible

The conspiracy/confabulation cascade of the exhale gate trap is reversible by forced complete exhalation.

| Field | Content |
|---|---|
| **Test** | Measure cognitive flexibility and paranoid ideation in participants trained to complete exhalation vs. control |
| **Confirmed if** | Complete exhalation training reduces paranoid ideation and increases flexibility |
| **Disconfirmed if** | No effect on paranoid ideation |
| **Status** | Untested |

### PREDICT-INF-12: Wide Workspace Reduces Executive Load

Expanding the physical workspace horizontally reduces the executive coordination cost of task-switching.

| Field | Content |
|---|---|
| **Test** | Measure task-switching performance, subjective effort, and EEG frontal theta in narrow vs. wide workspace |
| **Confirmed if** | Wide workspace reduces switch cost, effort, frontal theta |
| **Disconfirmed if** | Workspace width does not affect switch cost |
| **Status** | Untested |

## 15. Fear, Flow, and Salience Predictions

### PREDICT-FEAR-01: Fear Response Is Boundary Firing, Not Threat Detection

The autonomic signature of fear precedes conscious threat recognition by a measurable interval. This interval correlates with the curvature of the original encoding geometry.

| Field | Content |
|---|---|
| **Test** | Fear conditioning with HRV-confirmed geometry at encoding. Test recall under varying current geometries. |
| **Confirmed if** | Fear is boundary firing — encoding geometry predicts response |
| **Disconfirmed if** | Fear response tracks current threat assessment |
| **Status** | Untested |

### PREDICT-FLOW-01: Containment Cost Distinguishes Flow from High-Arousal Performance

Flow and high-arousal non-flow performance show different HRV signatures despite similar $A_s$. Flow: $A_s \uparrow$ with $\sigma(A_s) \downarrow$. High-arousal: $A_s \uparrow$ with $\sigma(A_s) \uparrow$.

| Field | Content |
|---|---|
| **Test** | HRV measurement during verified flow vs. high-effort non-flow performance |
| **Confirmed if** | Flow has unique geometric signature |
| **Disconfirmed if** | Flow and high arousal are geometrically identical |
| **Status** | Untested |

### PREDICT-FLOW-02: Gate Direction Predicts Loop Trajectory Before Subjective Experience

The direction of gate movement is detectable in HRV geometry before the subjective experience of flow or panic onset is reported.

| Field | Content |
|---|---|
| **Test** | Continuous HRV during tasks designed to tip toward flow or panic. Compare geometric shift onset with subjective report onset. |
| **Confirmed if** | Gate direction is the leading variable |
| **Disconfirmed if** | Subjective experience and geometric shift are simultaneous |
| **Status** | Untested |

### PREDICT-SAL-01: Salience Map Predicts Interoceptive Response, Not Stimulus Properties

Two individuals with different topology profiles show measurably different interoceptive responses to identical stimuli.

| Field | Content |
|---|---|
| **Test** | Present identical neutral-to-ambiguous stimuli to participants with pre-measured topology profiles. |
| **Confirmed if** | Salience is topologically determined |
| **Disconfirmed if** | Stimulus properties dominate response |
| **Status** | Untested |

### PREDICT-SAL-02: Geometry at Encoding Determines Durability of Change

The geometry present at the moment a signal is processed determines the durability of the resulting prior update.

| Field | Content |
|---|---|
| **Test (Corollary A)** | Aversive stimulus under baseline vs. post-breath-stabilization. Pre/post autonomic reactivity at 4-week follow-up. |
| **Test (Corollary B)** | Memory recalled under baseline vs. breath-stabilized recall. Correlate outcome with $\mathcal{U}$ at recall. |
| **Confirmed if** | Geometry at moment of processing is the active variable |
| **Disconfirmed if** | Content and duration are the primary variables |
| **Status** | Untested |

### PREDICT-SAL-03: Suppression Cost Is Measurable as Jitter Floor

Individuals with higher measured suppression load show higher baseline $\sigma(A_s)$ independent of overall stress level.

| Field | Content |
|---|---|
| **Test** | Baseline HRV during active suppression vs. open monitoring. Add breath override protocol. |
| **Confirmed if** | Jitter has a suppression component separable from arousal |
| **Disconfirmed if** | Jitter tracks arousal only |
| **Status** | Untested |

## 16. Loop Atrophy Predictions

### PREDICT-LOOP-01: Dunning-Kruger Confidence U-Shape Is the Loop Turning On

The confidence curve across competence is a U-shape. Confidence should track the system's ability to generate error signals, not actual competence.

| Field | Content |
|---|---|
| **IV** | Competence level (measured by task accuracy) |
| **DV** | Confidence (self-report), error-detection rate (behavioural), $W^*$ proxy (HRV) |
| **Operationalization** | Measure confidence, accuracy, error-detection rate, HRV across competence levels in a novel domain. |
| **Confirmed if** | Confidence U-shape tracks error-detection capability |
| **Disconfirmed if** | Confidence tracks accuracy linearly, or is uncorrelated with error-detection rate |
| **Status** | Untested |

### PREDICT-LOOP-02: Mastery Is Compressed Loop History

Expert "intuition" is prior retrieval of compressed loop history, not faster loop running.

| Field | Content |
|---|---|
| **IV** | Expertise level (novice vs. expert) |
| **DV** | Response time in-domain vs. novel domain |
| **Operationalization** | Measure response time for experts and novices on (a) familiar, (b) novel in-domain, (c) different-domain problems. |
| **Confirmed if** | Experts faster on familiar, slower on novel — loop-running is expensive |
| **Disconfirmed if** | Experts faster across all problem types |
| **Status** | Partially supported — Klein (1998) |

### PREDICT-LOOP-03: Loop Atrophy Is Reversible by Novel Problem Exposure

Masters who stop encountering novel problems show measurable $R^*$ drop and $W^*$ narrowing within 5 years. Reintroducing novel problem exposure reverses the decline.

| Field | Content |
|---|---|
| **IV** | Novel problem exposure (longitudinal) |
| **DV** | $R^*$ (HRV), $W^*$ (cognitive flexibility composite), CO₂ tolerance |
| **Control** | Age, baseline fitness |
| **Operationalization** | Longitudinal measurement in masters who stop vs. continue novel problem exposure. |
| **Confirmed if** | $R^*$, $W^*$, and CO₂ tolerance drop in non-novel group; reverse with reintroduction |
| **Disconfirmed if** | No difference between groups, or reversal does not occur |
| **Status** | Untested |

### PREDICT-REQT-01: Gate-Lowering is Behaviourally Invisible

Individuals at Stage 5 collapse will produce output indistinguishable in confidence from baseline performance, while showing measurable deficits on novel signal detection and multi-hop inference.

| Field | Content |
|---|---|
| **IV** | $L^*$ (composite load — see §2.10) |
| **DV** | Novel inference accuracy, confidence calibration, HRV coherence |
| **Falsification** | If high-$L^*$ subjects show confidence proportional to accuracy, the gate-lowering mechanism is disconfirmed. |
| **Status** | Untested |

### PREDICT-REQT-02: Collapse Sequence is Topologically Forced

Precision will degrade before window width, which will degrade before integration, which will degrade before gate closure. Order violations would disconfirm the causal topology.

| Field | Content |
|---|---|
| **IV** | Induced fatigue / load |
| **DV** | Sequential timing of $R^*$, $W^*$, $\Theta^*$, $\Lambda$ degradation |
| **Falsification** | If $\Theta^*$ degrades before $R^*$ under acute load, the sequence is wrong. |
| **Status** | Untested |

### PREDICT-REQT-03: Component REQT Predicts Intervention Response

Component REQT (each $L^*_i$ measured independently) predicts intervention response better than composite REQT. A system with high $L^*_{inflam}$ but low composite $L^*$ will respond to anti-inflammatory protocols; a system with high $L^*_{HRV}$ but low composite will respond to HRV biofeedback.

| Field | Content |
|---|---|
| **IV** | Component load profile |
| **DV** | Intervention response (targeted vs. non-targeted) |
| **Operationalization** | Assign interventions by profile-matched vs. composite-matched criterion. Compare outcome. |
| **Falsification** | If composite predicts response as well as component REQT, the distinction is not clinically useful. |
| **Status** | Untested |

### PREDICT-BREATH-01: Diaphragmatic Breathing Provides Continuous Right Hemisphere Access

Chest breathers operate below $C_{threshold}$ at baseline. Right hemisphere access requires a salience-induced breath-halt to transiently build CO₂. Diaphragmatic breathers operate near $C_{peak}$ — gate open continuously, no trigger required.

| Field | Content |
|---|---|
| **IV** | Breathing pattern (respiratory inductance plethysmography) |
| **DV** | Right hemisphere EEG lateralisation, $R^*$, novel inference performance at rest vs. post-salience-trigger |
| **Operationalization** | Chest breathers show larger performance gain post-trigger. Diaphragmatic breathers show negligible gain. |
| **Falsification** | Equal salience-dependence across both groups disconfirms the mechanism. |
| **Status** | Derived from real-time physiological observation, 2026-09-11 — untested. |

**The adventurousness connection:** Deep breathing studies are not measuring courage. They're measuring $n_{hops}$ rising. $W^*$ widens → competitive scaffold activates across wider territory → inference can hop forward through solution space → behavior appears adventurous. This directly connects to the adventurousness literature and explains it mechanistically in a way no current paper does.

### PREDICT-GATE-01: Delta HRV Response Capacity Tracks Λ Under Load

The delta HRV response to a standardized slow-breath protocol tracks $\Lambda$ — the loop activation indicator — across load states. A system at Zone 1 shows large delta response ($\Delta HRV > 15$ ms). A system at Zone 3 shows minimal response ($\Delta HRV < 5$ ms) regardless of resting HRV value.

| Field | Content |
|---|---|
| **IV** | Zone state (measured by composite $L^*$, §2.10) |
| **DV** | $\Delta HRV$ response to standardized slow-breath protocol |
| **Operationalization** | Measure $\Delta HRV$ across Zone 1, 2, 3 participants. Test whether delta response is a valid proxy for $\Lambda$. |
| **Confirmed if** | Delta response differentiates zones with high sensitivity; is stable within individual across repeated sessions |
| **Disconfirmed if** | Delta response is uncorrelated with zone or is dominated by baseline HRV |
| **Status** | Untested — protocol in Allostatic Load §5c |

### PREDICT-AL-01: Composite Load Predicts Cognitive Capacity

The composite load equation $L^* = w_1 L^*_{HRV} + w_2 L^*_{RHR} + w_3 L^*_{temp} + w_4 L^*_{inflam} + w_5 L^*_{resp}$ will predict cognitive performance ($C_s$) better than any single component.

| Field | Content |
|---|---|
| **IV** | Composite $L^*$ vs. single components |
| **DV** | Cognitive performance (working memory, multi-hop reasoning, ambiguity tolerance) |
| **Operationalization** | 30-day tracking with weekly cognitive assessments. Compare predictive power of composite vs. single components. |
| **Confirmed if** | Composite $L^*$ outperforms each individual component |
| **Disconfirmed if** | A single component predicts as well or better |
| **Status** | Untested |

### PREDICT-AL-02: HRV Dispersion Is the Signal, Not Noise

The variance of daily HRV measurements over 30 days will predict allostatic load outcomes (cognitive performance, inflammatory markers, self-reported stress) better than any single HRV reading. This is the direct test of the framework's central claim: the field has been treating the trajectory as noise.

| Field | Content |
|---|---|
| **IV** | HRV dispersion (variance across 30 days) vs. mean HRV |
| **DV** | Allostatic load outcomes |
| **Operationalization** | 30-day wearable tracking with weekly outcome assessments. Compare predictive power of variance vs. mean. |
| **Confirmed if** | Dispersion predicts outcomes better than mean |
| **Disconfirmed if** | Mean HRV predicts outcomes better than dispersion |
| **Status** | Partially supported — Okawara et al. (2024) |

### PREDICT-AL-03: ND Precision-Collapse Paradox

**a. Fasted precision spike:** ND populations will show higher cognitive performance under fasted conditions (>12h) compared to matched NT controls. Disconfirmation: ND performance ≤ NT under fasted conditions.

**b. Interoceptive routing shift:** ND populations will show lower heartbeat detection accuracy during concurrent cognitive load compared to NT controls, and the reduction will be greater in ND than NT at equivalent load levels. Disconfirmation: ND drop ≤ NT drop under load.

**c. Abrupt collapse profile:** ND populations will show a lower coefficient of variation in performance across the trial — stable high performance followed by a single drop — while NT populations show a gradual decline. Disconfirmation: ND variability profile indistinguishable from NT.

**d. Recovery signature:** ND populations will require longer recovery time (food + rest) before returning to pre-collapse performance than NT controls, consistent with debt clearance rather than simple glycaemic repletion. Disconfirmation: ND recovery time ≤ NT with glucose alone.

**e. Post-hoc hunger recognition:** ND populations will report hunger awareness post-collapse at higher rates than pre-collapse, while NT populations will show hunger awareness preceding cognitive decline. Disconfirmation: ND hunger ratings rise before, not after, performance collapse.

**Combined confirmation:** Collapse predicted by HRV floor + hunger signal dropout preceding collapse event, not by blood glucose alone (blood glucose may remain in normal range at time of collapse).

| Field | Content |
|---|---|
| **IV** | Population (ND vs. NT) |
| **DV** | Performance trajectory, interoceptive accuracy under load, recovery time, hunger signal timing |
| **Operationalization** | Full protocol in Allostatic Load §9e |
| **Falsification** | Any of 5a–5e disconfirmed |
| **Status** | Untested |

### PREDICT-AL-04: Delta HRV Predicts Inflammatory Markers with Lag

Delta HRV response will predict CRP and IL-6 levels with a lag of 7–14 days. Low delta HRV precedes inflammatory marker rise. High delta HRV precedes inflammatory marker decline.

| Field | Content |
|---|---|
| **IV** | $\Delta HRV$ response |
| **DV** | CRP, IL-6 |
| **Operationalization** | Prospective within-subject study with daily HRV measurement and weekly inflammatory biomarker sampling. |
| **Confirmed if** | Delta HRV leads inflammatory marker changes by 7–14 days |
| **Disconfirmed if** | Delta HRV and inflammatory markers are simultaneous or delta HRV lags |
| **Status** | Untested |

## 17. Social Projection Predictions

### PREDICT-SOC-01: Collective Synchrony Predicts W*

Societies with maintained communal rhythm show longer policy planning horizons, measurable by infrastructure investment timescale.

| Field | Content |
|---|---|
| **Test** | Cross-cultural comparison of synchrony mechanism integrity vs. planning horizon |
| **Status** | Untested at scale |

### PREDICT-SOC-02: L* Predicts Demagoguery Susceptibility

Populations with high chronic stress show higher false-positive rate for outgroup threat. Correlates with $K$, not ideology.

| Field | Content |
|---|---|
| **Test** | Measure chronic stress markers and outgroup threat false-positive rate |
| **Status** | Partially supported — stress and authoritarianism literature |

### PREDICT-SOC-03: Synchrony Loss Predicts Fragmentation

Reduction in communal synchrony activity predicts rising political polarisation within 5–10 year lag.

| Field | Content |
|---|---|
| **Test** | Longitudinal: synchrony activity vs. polarisation |
| **Status** | Untested prospectively |

### PREDICT-SOC-04: Collective 𝒰 Predicts Cultural Rigidity

Rate of prior update in collective beliefs correlates with ambient $K$. High-$K$ populations show slower belief updating regardless of evidence quality.

| Field | Content |
|---|---|
| **Test** | Measure collective belief update rate vs. ambient $K$ markers |
| **Status** | Partially supported — motivated reasoning literature |

## 18. Clinical Predictions

### PREDICT-CO₂-01: CO₂ Tolerance Predicts W

CO₂ tolerance correlates with colour constancy magnitude ($r > 0.5$) and with $R$ ($r > 0.6$). Manipulating breathing changes both.

| Field | Content |
|---|---|
| **Test** | Pre/post breathing manipulation with capnometry + ECG + colour constancy task |
| **Confirmed if** | $W$ is physiologically measurable via CO₂ tolerance |
| **Disconfirmed if** | Framework requires revision at Layer 02 |
| **Status** | Untested — off-the-shelf equipment |

### PREDICT-FND-01: The Prodrome Is Measurable

HRV shows progressive amplitude collapse in the period preceding FND onset. Structural imaging is clean.

| Field | Content |
|---|---|
| **Test** | Retrospective longitudinal wearable data in FND patient cohort |
| **Confirmed if** | $C_s \approx 0$ has a measurable geometric prodrome |
| **Disconfirmed if** | Framework requires revision at Layer 02 |
| **Status** | Untested — instrumentation available |

### PREDICT-Γ-01: Social Co-Regulation Restores Θ*

Social exposure (synchronized movement, music, dance, chanting) increases lateralized HRV coherence within 10–20 minutes.

| Field | Content |
|---|---|
| **Test** | Pre/post measurement in group synchrony protocols |
| **Confirmed if** | Integration efficiency is modifiable via co-regulation |
| **Disconfirmed if** | Framework requires revision at Layer 02 |
| **Status** | Untested — off-the-shelf equipment |

### PREDICT-AGE-01: Hot Cache Survives, RAM Degrades

Most-practiced cognitive operations show preserved function with age; novelty-handling operations degrade.

| Field | Content |
|---|---|
| **Test** | Compare language network vs. multiple demand network activity across age |
| **Confirmed if** | Language network preserved; MD network degrades |
| **Disconfirmed if** | Both networks degrade equally |
| **Status** | Confirmed — Billot et al. (2026) |

### PREDICT-AGE-02: Loop Atrophy Is Substrate Maintenance, Not Age

Masters who stop encountering novel problems show measurable CO₂ tolerance drop within 5 years, controlling for age.

| Field | Content |
|---|---|
| **Test** | Longitudinal CO₂ tolerance measurement in masters who stop vs. continue novel problem exposure |
| **Confirmed if** | CO₂ tolerance drops in non-novel group |
| **Disconfirmed if** | No difference |
| **Status** | Untested |

---

# PART V — COHESION CHECK

## 19. Variables Consistent Across All Sources

| Variable | Status | Notes |
|---|---|---|
| $A_s^*$ | ✅ | Consistent across MS, Precision, GoI, Loop, AL, CR |
| $W^*$ | ✅ | Consistent |
| $K$ | ✅ | Consistent |
| $I^*$ | ✅ | Consistent |
| $C_s$ | ✅ | Consistent |
| $S$ | ✅ | Consistent |
| $\delta_{min}$ | ✅ | Consistent |
| $P_{eff} > P_{threshold}$ | ✅ | Consistent |
| Path A/B | ✅ | Consistent |
| $L^*$ | ✅ | Decomposed across 5 components (Allostatic Load) |
| $C_{high}(L^*)$ | ✅ | Load-dependent CO₂ ceiling |
| $\Delta HRV$ | ✅ | Operational probe for $\Lambda$ |
| $IM$ | ✅ | Xue et al. (2026) |
| $\text{Dim}$ | ✅ | Derived from $W^* \times \Theta^*$ |
| $n_{hops}$ | ✅ | Derived from $W^* \cdot \rho_{scaffold}$ |
| $\rho_{scaffold}$ | ✅ | Roy & Banerjee (2026) |
| $\tau_{PE}$ | ✅ | Derived |
| $\sigma_{PE}$ | ✅ | Derived |
| $\Lambda$ | ✅ | Derived, with operational probe |
| $O_{pathway}$ | ✅ | Functional form specified as dependency |
| $L^*_{critical,i}$ | ✅ | Component critical load threshold |
| $G_m$, Drift, Cache, $C_{risk}$, $M_{state}$ | ✅ | Motor gain variables |
| $\sigma(t)$, $H_L$, $H_R$, $C_{LR}$ | ✅ | Somatic commutation variables (new in v1.5 from GoI v1.0) |
| Breath phase variables | ✅ | New in v1.5 from GoI v1.0 |
| Four-layer hierarchy (0/1/2/3) | ✅ | New in v1.5 from GoI v1.0 |
| Four contracts (MET↔AUTO, etc.) | ✅ | New in v1.5 from AL v2.1 |

## 20. Variables With Drift

| Variable | Issue | Resolution |
|---|---|---|
| $R^*$ | Loop paper uses $\omega_L$ (historical) | Replace $\omega_L$ with $R^*$ in any historical docs |
| $\Theta^*$ | Loop paper uses $n_L$ (historical) | Replace $n_L$ with $\Theta^*$ in any historical docs |
| $L^*$ vs. $\Pi_{cog}$ | MS uses $L^*$ only; Precision splits pressure | Mapping note in §2.3 |
| $L^*$ measurement | Central Reference defines; Allostatic Load measures | Decomposition in §2.10 |
| $C_{high}$ | Previously constant; now load-dependent | Updated in §2.3 and §3.3 |
| $J(C)$ vs. $\sigma(A_s)$ | Precision maps $J(C)$ to $\sigma(A_s)$; MS has no separate jitter | $J(C) \to \eta$ pathway note in §3.2 |
| $\mathcal{U}$ vs. $W_{enc}$ | MS defines $\mathcal{U}$; Precision defines $W_{enc}$ | Mapping note in §2.5 |
| $P$ vs. $P_{eff}$ | Precision v3.3 folded $U_C$ into $P$; v3.4 and CR v1.5 keep separate | Resolved in v1.5 §2.3, §3.6 — $P$ is raw ratio, $P_{eff}$ is gate condition |
| $\Lambda$, $n_{hops}$, $\rho_{scaffold}$ | Loop v1.0 defines; MS v7.2 absorbed | Registered in §2.2, §2.6 |
| $\delta_{hyst}$ | Precision defines; MS v7.2 registered | Registered in §2.3 |
| $L^*_{critical,i}$ | AL v2.1 uses; CR v1.4 registered | Registered in §2.9 |
| $O_{pathway}$ | GoI v1.0 uses; CR v1.4 registered | Registered in §2.8 |

## 21. Composition Questions Resolved

| Question | Resolution |
|---|---|
| Does $J(C)$ enter $K$ directly or via $\eta$? | Via $\eta$ — jitter degrades detectability without changing geometry |
| Does $\Pi_{mech}$ reduce $K$ or only $D_T$? | Only $D_T$ — it enforces symmetry, doesn't change curvature directly |
| Is $U_C$ a multiplier on $P$ or separate? | Multiplier on $P_{eff}$ — $P$ is raw ratio, $P_{eff} = P \cdot O_{pathway} \cdot U_C$ |
| Does $\delta_{hyst}$ affect $K$ or only $P$? | Only $P$ — hysteresis delays recovery of precision, not curvature |
| Does $IM$ map directly to $K$? | $IM \propto K$ — measures the axis entanglement component |
| Does $\text{Dim}$ include $n_{hops}$? | No — $\text{Dim}$ is axes available; $n_{hops}$ is hops available; distinct |
| Does $\rho_{scaffold}$ = 0.30 hold across species? | Open — Xue et al. confirms both species default to prior retrieval, but density may vary |
| Does PV+ failure map directly to $IM$? | Mechanistically specified — direct measurement needed |
| Does $\Delta CBF/\Delta CMRO_2$ mediate $R^* \to IM$? | Predicted — PREDICT-PE-04 |
| Is $IM$ measuring PV+ failure or containment cost component of $K$? | Open — decomposition study needed |
| Does $\tau_{PE}$ collapse when $J(C)$ rises, or does $\Pi_{cog}$ dominate? | Open — derived; needs direct test |
| Does $\Lambda$ capture all of Path A, or only gate opening? | Indicator, not mechanism — captures gate-opening condition |
| Is $L^*$ scalar or profile? | Both — composite for total magnitude, diagnostic for treatment targeting (§2.10) |
| Does $\Delta HRV$ probe $\Lambda$ at population scale? | Predicted — PREDICT-GATE-01 |
| Does $C_{high}(L^*)$ compression affect $J(C)$ onset symmetrically? | Open — the compression is modelled as linear ($C_{high}^0 - \gamma L^*$) but $J(C)$ is quadratic near the ceiling. Non-linear sensitivity near the compressed ceiling is not yet characterised. PREDICT-PREC-03 is the relevant test. |
| Does the glymphatic ODE interact with $L^*_{inflam}$ as a separate component? | Open — §4 specifies microglial activation as a recovery blocker, but §2.10 does not explicitly tie $L^*_{inflam}$ to glymphatic clearance rate. The ODE term $\lambda_{inflam}$ is intended to capture this, but the mapping from $L^*_{inflam}$ to $\lambda_{inflam}$ requires decomposition. |
| Is $O_{pathway}$ a function of $\Phi_{PV}$, $\Delta CBF/\Delta CMRO_2$, and $CVR_{max}$? | Yes — functional form declared in §2.8 as $O_{pathway} = f(\Phi_{PV}, \Delta CBF/\Delta CMRO_2, CVR_{max})$. The combination into a single scalar requires calibration. |
| What are the $M_{state}$ threshold values? | Open — individual calibration parameters ($G_{threshold}$, $\text{Cache}_{min}$, $C_{threshold}$). No current prediction calibrates them directly. See §2.11 and open question 15. |
| What is the functional form of somatic commutation's $H_L$, $H_R$? | Open — $H_L = f_L(\sigma(t))$, $H_R = f_R(\sigma(t))$. The functional form of $f_L$ and $f_R$ requires calibration. See §2.12 and GoI v1.0 §3.4.2. |
| Where in the exhale cycle do thoughts fire — gradual or threshold? | Open — PREDICT-INF-10 distinguishes the two by EEG. See §5d. |
| Does $\Lambda$ appear in the intelligence equation only, or also as a state variable? | Both — $\Lambda$ is a state indicator (§2.2) and appears in the intelligence equation (§1). It is the gate condition made explicit. |

## 22. Remaining Open Questions

1. Direct measurement of $R^*$ and $IM$ in the same paradigm (PREDICT-PE-04)
2. Decomposition of $IM$ into PV+ failure vs. containment cost components
3. Mapping of $\tau_{PE}$ to $J(C)$ and $\Pi_{cog}$ — which dominates
4. Operationalization of $\tau_{PE}$, $\sigma_{PE}$
5. Empirical calibration of $\alpha$, $\beta$, $\gamma$, $\epsilon$
6. $R^*_{min}$ and $A^*_{s,max}$ threshold measurement protocols
7. Formal ODE derivation from $\mathcal{U}$
8. Morning vs. evening HRV study with $L^*$ modeling
9. ND vs. NT amplitude range comparison
10. Scope-of-claim defense (inferential distance between HRV and full cognitive/emotional/social projection)
11. Composite weight calibration (PREDICT-AL-01)
12. Component REQT vs. composite REQT intervention prediction (PREDICT-REQT-03)
13. Non-linear sensitivity of $J(C)$ near the compressed $C_{high}(L^*)$ ceiling — does linear compression of the ceiling produce quadratically amplified jitter onset?
14. Formal mapping from $L^*_{inflam}$ (§2.10) to the $\lambda_{inflam}$ term in the glymphatic ODE (§4) — decomposition study required.
15. **Calibration of $M_{state}$ thresholds** ($G_{threshold}$, $\text{Cache}_{min}$, $C_{threshold}$) — individual parameters requiring empirical estimation. See §2.11.
16. **Functional form of the somatic commutation operators** $f_L$, $f_R$ (§2.12) — how gaze laterality translates to contralateral hemispheric drive requires calibration.
17. **Gradual vs. threshold thought timing** in the exhale cycle — PREDICT-INF-10 distinguishes the two by EEG. See §5d.

## 22b. Why Prior Studies Failed — Structural Account

The framework has a specific response to the null-result literature: prior studies measured the wrong variable with the wrong design.

Standard HRV allostatic load research takes a single reading, averages across participants, and tests for correlation with an outcome. This design structurally eliminates the variable it claims to measure:

- **Allostatic load is a trajectory, not a state.** A participant at 8am and the same participant at 4pm carry different accumulated debt. Averaging morning and afternoon readings produces a number that corresponds to neither state.
- **Variance is the signal.** Averaging across participants with different baseline debt levels produces a distribution whose variance obscures the effect.
- **Unmeasured load state attenuates coupling.** When load is uncontrolled across participants, any coupling between two physiological signals is attenuated by uncontrolled variance in load state.

This is not a critique of individual study designs — it is a structural account of why a specific design class produces null results. The framework predicts exactly the results observed: "modest coupling" between autonomic and interoceptive changes (Schumann et al., 2026) is exactly what the framework predicts when load state is uncontrolled. The effect was not absent. It was averaged away.

**The fix is trivial:** measure HRV at multiple times across the day, same participant, same protocol. Two readings. The wearable market has been doing this for a decade. The field was not looking for variance — it was looking for stability. It found noise because it was measuring the wrong thing with the wrong design.

## 22c. Confounds and Limitations

The delta HRV proxy is a composite signal. Several confounds must be acknowledged:

**Age:** Resting HRV declines with age through progressive autonomic remodelling. The within-person baseline method corrects for this partially — the individual's own trajectory is the reference — but age-related floor compression may reduce the dynamic range available for load detection in older populations.

**Baroreflex sensitivity:** Baroreflex gain modulates HRV independently of allostatic load. Individuals with inherently lower baroreflex gain will show compressed delta HRV responses at equivalent load levels. The framework's predictions about delta HRV decline hold within individuals across time, not across individuals with different baroreflex baselines.

**Medications:** Beta-blockers, antihypertensives, and stimulant medications directly alter HRV. Any study applying this framework must control for or stratify by medication status. The delta HRV response in a medicated individual reflects the combined effect of load and pharmacological autonomic modulation.

**Respiratory mechanics:** Breathing rate, tidal volume, and respiratory training status confound the relationship between HRV and load. The slow-breath protocol partially controls for this by standardising the respiratory input, but individuals with significantly different resting respiratory patterns require standardised protocol conditions to produce comparable delta HRV values.

**Fitness level:** Aerobic fitness independently elevates resting HRV and may confound the HRV baseline drift component. PREDICT-AL-02 tests whether CO₂ tolerance predicts HRV independently of fitness — this is the key disconfirmation criterion for the fitness confound hypothesis.

These confounds do not invalidate the framework. They specify the conditions under which the predictions hold most cleanly and identify the stratification variables required for confirmation studies.

---

# PART VI — VERSION HISTORY

## 23. This Specification

| Version | Date | Changes |
|---|---|---|
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
| **The Hallucination You Are Having Right Now** | — | Substrate-agnostic hallucination theory | 10.5281/zenodo.21922044 |
| **Physics as the Missing Component in Medical Science** | — | Physical substrate | 10.5281/zenodo.21512678 |
| **Unified Regulatory Model** | — | Implementation architecture | 10.5281/zenodo.20417459 |
| **The Context Oscillator** | — | Context window architecture | 10.5281/zenodo.21811408 |
| **The Profile of a Person That Is AGI** | — | AGI as system property | 10.5281/zenodo.21921714 |
| **Dual-Substrate Cognition Architecture** | — | Human-AI co-processing | 10.5281/zenodo.21362260 |
| **Hallucinations Are Not Random** | — | AI hallucination mechanism | 10.5281/zenodo.21244811 |
| **Regulatory-Engine Qualification for Complex Decision-Making** | — | Governance-facing REQT artifact | pending |

## 25. The Stack

Central Reference v1.5 is the single specification. The stack is:

```
                         Central Reference v1.5
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
```

**Reading order for a new reader:** Central Reference v1.5 first. It contains everything. The supporting papers are for depth on specific layers.

**Citation rule for future papers:** Cite Central Reference v1.5 alone. The supporting papers are domain projections and do not need separate citation unless the new paper is specifically extending one of their layers.

**Update rule:** Any new mechanism or variable must be added to Central Reference first. The supporting papers then reference Central Reference, not vice versa.

## 26. The One Line

> The brain is an energy budget allocation system operating on priors. The breath is the source. The geometry is the mechanism. The prior is the output. Every phenomenon in this document — flow, collapse, fear, trauma, savant capacity, clinical states, social fragmentation, AI hallucination — is one variable changing in one equation. The variable is geometry. The equation is the master equation.

---

*End of specification.*

**Version:** 1.5
**Date:** 2026-09-13
**Status:** Full stack convergence — single-document specification achieved
**Next version:** v1.6 — after first round of empirical testing, or v2.0 — if any mechanism requires revision
