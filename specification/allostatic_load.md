# Allostatic Load as Accumulated Regulatory Debt: A Comprehensive Measurement Framework

**Robinson, J. (2026)**

*Technical Report — Manifold Schema Series*

**Version:** 2.2
**Date:** 2026-10-14
**Status:** Integrated with Central Reference v1.8.3 and Salience Interrupt v1.3; inherits salience accumulation, perseveration, release-triggered, encoding, and somatic load; P-AL-011 remains central prediction
**Framework:** Manifold Schema v7.2 (DOI: 10.5281/zenodo.21939439)
**Precision formalism:** Precision, Timing, and the Oscillatory Source v3.4 (DOI: 10.5281/zenodo.22179675)
**Biological implementation:** The Geometry of Inference v1.0 (Robinson, 2026d)
**Salience implementation:** The Salience Interrupt v1.3 (Robinson, 2026g)
**Complete specification:** Central Reference v1.8.3 (Robinson, 2026h)

---

## Changelog — v2.1 → v2.2

This changelog tracks the Salience Interrupt v1.3 inheritance. All changes are additive at the mechanism level. The measurement protocol from v2.1 survives; the composite load equation is extended; the profile table and treatment targeting table are extended.

| Step | Change | Location | Reason |
|---|---|---|---|
| 1 | Version bumped to 2.2 | Header | Salience inheritance |
| 2 | Added Schumann origin paragraph | §1a | Names the origin of the framework |
| 3 | Added §2g — Perseveration load | New section | Inherit SAL-35–37 |
| 4 | Added §2h — Release-triggered load | New section | Inherit SAL-38–41 |
| 5 | Added §2i — Encoding load | New section | Inherit SAL-42–45 |
| 6 | Added §2j — Somatic load path | New section | Inherit SAL-46–47 and SAL §2.5.3 |
| 7 | Extended composite load equation to 10 components | §6c | Add salience-derived components |
| 8 | Added measurement burden note and tier table | §6c | Distinguish consumer/clinical/research tiers |
| 9 | Extended load profile table to 9 profiles | §7a | Add salience-derived profiles |
| 10 | Extended treatment targeting to 10 targets | §7b | Add salience-derived targets |
| 11 | Restored P-AL-013 and P-AL-014; added P-AL-015 through P-AL-020 | §9 | P-AL-013/014 restored from archived prediction file; P-AL-015 through P-AL-020 inherit from Salience v1.3 |
| 12 | Updated summary count and equation reference | §11a | 10-component equation, 18 predictions |
| 13 | Added core insight sentence | §11b | Salience mechanism is upstream source |
| 14 | Added Robinson 2026g reference | References | Salience v1.3 citation |
| 15 | Added v2.2 row to version history | Version History | Versioning track |

**What did not change:** Every mechanism from v2.1, every measurement protocol, the delta HRV protocol, the within-person baseline method, the CO₂ tolerance threshold, the exhale completeness ratio, the four regulatory contracts, the glymphatic clearance architecture, and the debt trajectory zones. v2.2 is inheritance, not revision.

---

## Changelog — v2.0 → v2.1

This changelog exists so that any reader — human or AI — can see the convergence path. Allostatic Load v2.0 was written to converge with Central Reference v1.3. The v1.3 → v1.4 delta was the addition of $O_{pathway}$ (§2.8), $L^*_{critical,i}$ (§2.9), and the motor gain variables (§2.11). AL v2.0 already uses $L^*_{critical,i}$ (§6c via component REQT). The v2.1 changes are versioning and cross-reference updates only.

| Step | Change | Location | Reason |
|---|---|---|---|
| 1 | Header updated to "Integrated with Central Reference v1.4" | Header | Version drift |
| 2 | Added note on $O_{pathway}$ and motor gain variables | §Context and Motivation | AL does not absorb these — they are gate-condition and motor-substrate variables, documented in Central Reference §2.8 and §2.11, and in GoI v1.0 |
| 3 | Stack list: added *The Loop Is the Intelligence*; added version numbers to Precision, GoI, MS | §Context and Motivation | Full stack citation |
| 4 | Inline Central Reference cross-references: removed version numbers, kept section numbers | Throughout | Section numbers stable across minor versions; version drift removed |
| 5 | Added note at top pinning all Central Reference cross-references to v1.4 | §Context and Motivation | Single point of version reference |
| 6 | References: Robinson 2026e updated to Central Reference v1.4 | References | Version update |
| 7 | References: added Robinson 2026f (Loop v1.0) | References | Loop paper now cited |
| 8 | Changelog added at top | This section | Versioning track |
| 9 | Version history updated | Version History | — |

**What did not change:** Every mechanism, every measurement protocol, every prediction. v2.0 was already aligned at the mechanism level. v2.1 is a specification-level convergence.

**Note on variables AL does not absorb:** Allostatic Load measures $L^*$, the five-component decomposition of $L^*$, the delta HRV response, the CO₂ tolerance threshold, and the trajectory zones. It does not absorb $O_{pathway}$ (gate-condition variable, Central Reference §2.8) or the motor gain variables $G_m, \text{Drift}, \text{Cache}, C_{risk}, M_{state}$ (motor-substrate variables, Central Reference §2.11). These are documented in the Central Reference and operationalized in GoI v1.0 and Precision v3.4 where applicable. AL provides the load measurement layer of the framework; the gate and motor layers are separate.

---

**Context and Motivation**

This paper was written in direct response to a gap that should not exist.

The academic field studying allostatic load has spent decades developing biomarker panels, running single-reading studies, and concluding that HRV correlations are modest or unclear. Simultaneously, a multi-billion dollar consumer wearable industry — Oura, WHOOP, Garmin, Apple, Polar, Biostrap — has built products that measure allostatic load continuously, reliably, and at global scale. These products provide access to continuous HRV data at scale — hundreds of millions of device-days, preserved at the individual level, across sleep and wake cycles. The data they generate is not the validation of the framework. The validation is in the mechanistic framework and the falsifiable predictions. The wearables are the instrument platform. The framework is the interpretation. What the wearable market demonstrates is that variance exists at scale, is consistent across millions of users, and is predictive enough to build commercially viable products on. That is a strong prior. The mechanistic account of why variance is meaningful is this paper's contribution.

The field has been calling the signal noise. The market has been selling it as a product.

This paper provides the formal mechanistic framework that explains why the wearable market is right and why single-reading academic designs are structurally guaranteed to miss the effect. It is not a critique of HRV as a construct. It is a critique of measurement design that ignores the time-dependence of the construct it claims to measure.

This paper sits within a broader research stack that provides the theoretical foundation:

- *The Manifold Schema* v7.2 (Robinson, 2026a) — the geometric framework for consciousness, cognition, and regulatory collapse
- *Physics as the Missing Component in Medical Science* (Robinson, 2026b) — the pressure mechanics and finite-resource invariant underlying regulatory load
- *Precision, Timing, and the Oscillatory Source* v3.4 (Robinson, 2026c) — the formal precision equation ($P = R/D_T$) integrated throughout this paper
- *The Geometry of Inference* v1.0 (Robinson, 2026d) — the cache hierarchy and resolution floor that allostatic load directly degrades
- *Central Reference* v1.4 (Robinson, 2026e) — the unified specification; this paper's $L^*$ decomposition is formalized in Central Reference §2.10, and the REQT qualification standard is defined in §3.7
- *The Loop Is the Intelligence* v1.0 (Robinson, 2026f) — the intelligence projection; the delta HRV probe operationalizes the loop activation indicator $\Lambda$ (Central Reference §2.2, PREDICT-GATE-01)

Readers encountering this paper first are encouraged to follow the citation chain. The allostatic load measurement framework is not a standalone claim. The repeated self-citations throughout this paper are not rhetorical — they are structural: each cited paper formally specifies a component of the mechanism chain that this paper applies. Robinson (2026a) specifies the manifold geometry; Robinson (2026b) specifies the pressure mechanics; Robinson (2026c) specifies the precision equation; Robinson (2026d) specifies the cache hierarchy; Robinson (2026e) specifies the unified variable and equation registry that this paper's measurement protocol operationalizes; Robinson (2026f) specifies the intelligence loop that the delta HRV probe tracks. Any reader who wants to verify or falsify a claim in this paper can follow the citation to the formal specification. The modular architecture is intentional.

**Note on Central Reference cross-references.** All Central Reference cross-references in this paper are to v1.4 (2026-09-13) unless otherwise noted. Section numbers are stable across minor versions; the version is not cited inline to avoid version drift.

---

## Abstract

HRV is a time‑dependent oscillatory signal driven by breathing. Any measurement design that ignores time will suppress the very mechanism it claims to investigate.

The academic field has spent decades measuring HRV as though it were a static trait. The variance was always there — Okawara et al. (2024) measured it, the Task Force of the European Society of Cardiology documented circadian patterns, and chronobiology has long recognized the daily rhythm. The data exists. What has been missing is the interpretive framework that makes the variance readable as allostatic load rather than measurement noise. The wearable market has spent a decade proving it is a dynamic trajectory. This paper provides the formal framework that makes the trajectory readable — and explains why the field has been calling the signal noise.

A multi-billion dollar wearable industry is already measuring allostatic load continuously. The academic field has not noticed. Allostatic load is conventionally measured through biomarker snapshots — cortisol, inflammatory markers, metabolic panels — that are historical by the time they are taken and averaged in ways that eliminate the temporal dynamics they claim to measure. This paper proposes a mechanistically grounded continuous measurement framework derived from the convergence of four regulatory contracts: metabolic-autonomic (MET↔AUTO), immune-autonomic (IMMUNE↔AUTO), metabolic-immune (MET↔IMMUNE), and autonomic-modulation (AUTO↔MOD), integrated with the precision-geometry framework (Robinson, 2026c) and the glymphatic clearance architecture (GLYMPH↔AUTO).

The central argument is that allostatic load is not a state but a trajectory — accumulated regulatory debt that raises the oscillatory noise floor, compresses the CO₂ tolerance window, depresses vagal tone, and progressively narrows the precision ceiling of the system. The primary real-time measurement proxy is the delta HRV response to a standardized slow-breath protocol: a system with low accumulated debt shows significant HRV rise; a system at load ceiling shows minimal response regardless of resting HRV value. Secondary proxies — exhale completeness ratio, CO₂ tolerance threshold, inflammatory biomarker lag, sleep architecture, and respiratory efficiency — validate the primary measure and locate the system's position across the debt trajectory.

The framework explains why single-reading studies consistently fail to find correlations that within-subject repeated measurement reliably produces, and why ND populations represent the highest-signal cohort for mechanism research rather than a pathological outlier class. The complete measurement architecture includes a composite load equation with five weighted components: HRV baseline drift, sleep RHR elevation, sleep temperature elevation, chronic inflammatory tone, and respiratory inefficiency.

The salience mechanism provides the upstream explanation for why HRV is a load proxy. Each unresolved precision-lock — each salience interrupt that fired but never committed — is a unit of allostatic load. The latch holds by ATP-brace, which compresses vagal tone. The compressed vagal tone is what the wearable measures. The HRV trajectory is the latch-load trajectory. The perseveration loop, the release-triggered re-salience, and the encoding load are three additional failure modes that extend the load beyond simple latch accumulation. The somatic load path — the cost of *not* redistributing routing through movement — is the fourth. Together, these mechanisms explain where the load comes from, not just how to measure it.

**Central falsifiable prediction (P-AL-011):** The variance of daily HRV measurements — the dispersion across days — predicts allostatic load outcomes better than any single reading. This is the signal the field has been treating as noise. If this prediction fails, the framework's core claim fails, regardless of the other predictions.

---

## 1. The Measurement Problem

### 1a. The Structural Flaw in Single-Reading Designs

The standard methodological approach to allostatic load research takes a single biomarker reading, averages across participants, and tests for correlation with an outcome variable. This design has a structural flaw that guarantees null results in a specific class of studies: it statistically eliminates the variable it claims to measure.

Allostatic load is not a fixed property. It accumulates across a session, a day, a week. A participant measured at 8am carries different accumulated debt than the same participant measured at 4pm — not because they are different people, but because regulatory borrowing has occurred across the intervening hours. Averaging a morning reading and an afternoon reading produces a number that corresponds to neither state. Averaging across participants with different baseline debt levels produces a distribution whose variance obscures the effect in noise.

The consequence is visible in the literature. Studies find no correlation between HRV and inflammatory markers, between CO₂ tolerance and cognitive performance, between resting autonomic state and immune activation — not because these correlations do not exist, but because the design systematically eliminates them before analysis begins.

Schumann et al. (2026) concluded that "associations between physiological and interoceptive changes were modest" following an 8-week HRV biofeedback intervention. The study design was appropriate for its primary question: did HRV biofeedback training produce autonomic and interoceptive changes? Both pre- and post-intervention measurements were taken at similar times of day, which correctly controls for time-of-day confounds when measuring training effects. But Schumann also asked a second question — does the autonomic change predict the interoceptive change? — and found "modest coupling." The framework predicts exactly this result. When allostatic load is unmeasured, the coupling between any two physiological signals is attenuated by uncontrolled variance in load state across participants. The "modest coupling" is not a failure of Schumann's design for its primary question. It is a prediction of this framework for the secondary question: coupling will be modest until load is measured and held constant.

**The salience mechanism explains why the coupling was modest.** Schumann et al. measured HRV before and after an 8-week intervention. The training effect was real — the autonomic change was measurable. What the design could not control was the load state each participant brought to the measurement. Allostatic load is not a trait. It is a trajectory. And the trajectory is shaped by unresolved salience interrupts — precision-locks that fired but never committed. Each held latch compresses vagal tone. Each participant arrived with a different number of held latches. The HRV reading reflected the latch load, not the training effect. The "modest coupling" is not a failure of HRV. It is the prediction of this framework: coupling will be modest until load is measured and held constant. The Salience Interrupt paper (Robinson, 2026g) specifies the mechanism. This paper specifies the measurement. Together they close the loop.

### 1b. The Core Statement

**HRV is a time‑dependent oscillatory signal driven by breathing. Any measurement design that ignores time will suppress the very mechanism it claims to investigate.**

This is not a methodological subtlety. It is a category error. HRV is not a trait that can be captured in a snapshot. It is a dynamic trajectory that must be tracked across time. Measuring HRV at a single timepoint and concluding it "doesn't correlate" is like measuring blood pressure once and concluding it doesn't vary with activity. The mechanism *is* the variation. The signal *is* the trajectory. The field has been measuring the wrong variable with the wrong design and calling the result "noise."

### 1c. Wearable-Derived HRV Data as Empirical Evidence of Variance and Trajectory

The consumer wearable market has already demonstrated, at global scale, the exact HRV dynamics that academic studies routinely fail to detect. Platforms such as Oura, WHOOP, Garmin, Apple, Polar, and Biostrap collectively represent hundreds of millions of device-days of HRV data, collected continuously across sleep and wake cycles. These devices do not rely on single snapshots or population averages. Their entire analytic architecture is built on variance, trajectory, and response capacity — the same constructs formalized mechanistically in this framework.

Wearable HRV data consistently shows three invariant patterns:

1. **HRV rises overnight.** During deep sleep, vagal dominance, glymphatic clearance, and metabolic reset restore oscillatory range. This produces a predictable upward drift in HRV across the night. This is the recovery window.

2. **HRV falls across the day.** As metabolic, autonomic, and inflammatory load accumulate, oscillatory range compresses. HRV declines progressively from morning peak to evening trough. This is the debt trajectory.

3. **HRV variance predicts outcomes.** Daily dispersion — the spread of HRV values across days — correlates with stress, recovery, illness, inflammation, cognitive performance, and metabolic stability. This is the signal.

These patterns are consistently observed across wearable platforms at scale. The wearable market did not discover these dynamics through mechanistic modeling; it discovered them because continuous measurement makes variance impossible to ignore. What the market has not provided is the mechanistic account of *why* the variance is meaningful. That is what this framework contributes: the variance is the trajectory, and the trajectory is allostatic load.

**The field could have solved this years ago by picking up the phone.** Oura's Daytime Stress feature, which combines HRV with other signals, demonstrates that physiological variance is meaningful and predictive — the opposite of the 'noise' framing. WHOOP's Stress Monitor uses HRV and heart rate to estimate stress in real time. This is accurate. The "moment-by-moment" framing is slightly overstated — it updates periodically throughout the day, not continuously second-by-second. Garmin's Body Battery and HRV Status track recovery and strain across days. These aren't theoretical claims — they're documented features on millions of devices, deployed for years, consistently observed across thousands of cohorts.

### 1d. The Contradiction

This creates a direct contradiction with academic studies that conclude "HRV does not correlate." If HRV truly lacked correlation, then Oura's readiness score, WHOOP's strain/recovery model, Garmin's Body Battery, Apple's HRV trends, and Polar's training load would all be built on meaningless noise. Yet these systems reliably predict recovery, illness onset, autonomic strain, sleep quality, and metabolic instability — precisely because they measure trajectory, not snapshots.

The discrepancy arises from methodological design:

| Academic Studies | Wearable Platforms |
|---|---|
| Take a single HRV reading | Measure continuously |
| Average across participants | Preserve individual variance |
| Treat variance as noise | Treat variance as the signal |
| Collapse time into a single value | Track daily drift and trajectory |
| Conclude "HRV doesn't correlate" | Build products that predict recovery, strain, and illness |

The conclusion that HRV "does not correlate" is therefore not a property of HRV. It is a property of measurement design that suppresses the signal.

**HRV is a time‑dependent oscillatory signal driven by breathing. Any measurement design that ignores time will suppress the very mechanism it claims to investigate.**

### 1e. The Fix

The experimental correction is trivial: measure HRV at multiple times across the day. Morning and evening. Same participant. Same protocol. That single addition would have revealed the trajectory. The field did not run this experiment because it had no model telling it the result would be meaningful. Without a model of statefulness, a second measurement looks like replication noise rather than trajectory signal.

The field was not looking for variance. It was looking for stability. It found noise because it was measuring the wrong thing with the wrong design.

The Manifold Schema provides the model that makes the variance readable. The prediction is now explicit: HRV follows a declining trajectory across waking hours proportional to load accumulation, with recovery occurring during sleep. The experiment is trivial to run. The data already exists in every wearable user's history.

The fix is not methodological sophistication. It is two readings.

A resting HRV baseline followed by a standardized slow-breath protocol and a second HRV reading produces a delta — $\Delta HRV = HRV_{post} - HRV_{rest}$ — that is the actual measurement. A system with low accumulated debt has remaining oscillatory range and will show significant HRV rise under the slow-breath protocol. A system at or near its load ceiling has no remaining range and will show minimal response regardless of its resting baseline value.

$$\Delta HRV \propto \frac{1}{L^*}$$

This inverse relation is a heuristic summary of the delta HRV–load relationship. The full formal specification, integrating the precision equation and CO₂ uniformity terms, is given in Section 2d.

This single methodological addition — measuring response capacity rather than resting state — recovers the correlations that single-reading designs cannot find. The correlations were always there. The design was looking at position on the trajectory rather than the trajectory itself.

The delta HRV response is not merely a load proxy. It is the operationalization of the loop activation indicator $\Lambda$ defined in Central Reference §2.2 and PREDICT-GATE-01. A system with low accumulated debt has the response capacity to open the loop under the slow-breath protocol ($\Delta HRV > 15$ ms). A system at load ceiling has no remaining response capacity ($\Delta HRV < 5$ ms). This connects the load measurement layer to the intelligence loop directly — the same variable that determines whether the loop can be opened.

The remainder of this paper formalizes the mechanism chain that produces the trajectory, the debt accumulation that shapes it, and the measurement protocol that makes it visible.

---

## 2. The Four Contracts as the Mechanism Chain

> **A note on contracts:**
> Throughout this paper, "contracts" refer to formally specified bidirectional regulatory relationships between physiological layers — each contract documents the complete causal chain in both directions, the link-by-link mechanism, operating states, failure modes, and empirical anchors. The four contracts cited here (MET↔AUTO, IMMUNE↔AUTO, MET↔IMMUNE, AUTO↔MOD) are part of the Unified Regulatory Model (URM), a modular architecture developed in parallel with the Manifold Schema research stack. The full contract specifications are publicly available at:
>
> https://github.com/jtrthehax/Unified-Model/tree/main/01_PHYSICS_SUBSTRATE_CORE
>
> Readers encountering this framing for the first time should treat each contract reference as equivalent to a formally specified subsystem — the mechanism described in each section below is the contract's primary chain, condensed for this paper. The full specifications include operating states, failure modes, drug and intervention effects, and empirical anchors for each link in the chain.

Allostatic load does not arise from a single pathway. It is the accumulated output of four converging regulatory contracts, each of which contributes to the debt trajectory through a distinct mechanism. Understanding the measurement requires understanding the chain.

### 2.0 The Mechanism Chain — Overview

The four contracts converge into a single accumulation trajectory. Each link below is anchored in existing literature. A critic challenging any link must address the cited paper directly before reaching the framework.

```
Metabolic stress — elevated glucose, hypoxia, hypercapnia
  ↓ MET↔AUTO
Carotid body chemoreceptors sense arterial CO₂, O₂, pH, glucose simultaneously
  ↓ [Moreira et al., 2006 — central chemoreceptors drive sympathetic vasomotor outflow directly]
Sympathetic output rises, vagal tone compresses, HRV drops
  ↓ [Thayer et al., 2010 — autonomic imbalance and HRV as cardiovascular risk marker]

Elevated glucose
  ↓ MET↔IMMUNE
Mast cell activation → TNF-α, IL-1β, IL-6 → macrophage M1 polarization → insulin resistance 
→ glucose maintained
  ↓ [Segerstrom & Miller, 2004 — psychological stress and immune system: 30-year meta-analysis]

Cytokines cross blood-brain barrier → hypothalamic and brainstem disruption
  ↓ IMMUNE↔AUTO
Low vagal tone → inadequate cholinergic anti-inflammatory pathway → cytokine brake fails → HRV and CAP share the same efferent pathway
  ↓ [Tracey, 2002 — the inflammatory reflex: vagal efference drives CAP, HRV and anti-inflammatory brake are mechanistically identical]
  ↓ [Hall et al., 2004 — acute stress affects HRV and inflammation simultaneously]

Autonomic compression accumulates
  ↓ AUTO↔MOD
Incomplete exhale → RSA amplitude reduction → oscillatory window compresses → precision loss
  ↓ [Mathewson et al., 2016 — RSA declines under cognitive load]
  ↓ [Reed et al., 2020 — behavioral load depletes regulatory capacity]

High load → faster shallower breathing → reduced intrathoracic pressure differential
  ↓ GLYMPH↔AUTO
Reduced CSF pulsatility → glymphatic clearance fails → amyloid accumulation → microglial activation → sleep architecture disruption → 
further load
  ↓ [Iliff et al., 2012 — paravascular pathway and CSF clearance of interstitial solutes including amyloid β]
  ↓ [Grunewald et al., 2012 — sleep deprivation drives inflammation]
  ↓ [Zhang et al., 2025 — sleep deprivation and HRV: meta-analysis]

Accumulated debt visible as trajectory
  ↓
HRV baseline drifts downward across days
  ↓ [Okawara et al., 2024 — daily HRV variance predicts work performance better than mean]
  ↓ [Vitale et al., 2019 — HRV follows circadian rhythm with individual chronotype variation]

Delta HRV response compresses toward zero
  ↓
L* rises — system approaches load ceiling
```

Sections 2a–2e formalize each contract in detail. The chain above is the summary. The sections below are the mechanism.

### 2a. MET↔AUTO — The Metabolic Entry Point

The carotid body chemoreceptors at the bifurcation of the common carotid artery are the primary transducers of metabolic state into autonomic drive. They sense arterial CO₂, O₂, pH, and glucose simultaneously. Under metabolic stress — elevated glucose, hypoxia, hypercapnia — carotid body activation drives sympathetic output through the NTS, compressing vagal tone and depressing HRV.

Critically, the CO₂ tolerance window determines the system's available oscillatory range. A narrow tolerance window — produced by chronic overbreathing or accumulated metabolic load — means the system reaches chemoreflex activation threshold sooner, HRV ceiling is lower, and the capacity for precision recovery through slow breathing is reduced. The Control Pause — the duration of comfortable breath hold before the chemoreflex activates — is the most accessible clinical measure of this window and is a direct prerequisite for interpreting HRV biofeedback outcomes.

The MET↔AUTO contract is where dietary pattern, glucose regulation, and chronic metabolic load enter the regulatory system before propagating through every contract above.

**Precision-Geometry Integration:** The precision framework (Robinson, 2026c) formalizes the CO₂ tolerance window as $C_{\text{low}} < C < C_{\text{high}}(L^*)$, with precision $P$ rising with CO₂ until $C_{\text{high}}$, then collapsing as chemoreflex jitter $J(C) = \kappa(C - C_{\text{high}}(L^*))^2$ increases. Allostatic load narrows this window directly:

$$C_{\text{high}}(L^*) = C_{\text{high}}^0 - \gamma L^*$$

where $C_{\text{high}}^0$ is the baseline tolerance and $\gamma$ is the load-induced compression coefficient. This means the same CO₂ level produces jitter at lower absolute values when load is high. See Central Reference §2.3 for the formal definition.

### 2b. MET↔IMMUNE — The Accumulation Mechanism

Elevated blood glucose directly activates mast cells through glucose-dependent ATP production required for mast cell function. Mast cell degranulation produces histamine, proteases, and cytokines — TNF-α, IL-1β, IL-6, IL-33. These cytokines activate macrophage M1 polarization in adipose tissue, producing further cytokine release that drives serine phosphorylation of the insulin receptor substrate, impairing insulin signaling and maintaining hyperglycemia.

The loop is self-reinforcing: glucose → immune activation → insulin resistance → glucose. Each high-glycemic event is a loop activation event. Over time, baseline inflammatory tone rises. This rising baseline is the metabolic contribution to allostatic debt — an immune system running at elevated activation that continuously draws on the autonomic resources of the contracts above it.

The ND-specific amplification is relevant here. Mast cell hyperreactivity co-occurs with autism, ADHD, dysautonomia, and hypermobility at rates significantly above population baseline through the same connective tissue variation that affects breathing mechanics. ND populations accumulate MET↔IMMUNE debt faster at equivalent glycemic exposure.

### 2c. IMMUNE↔AUTO — The Vagal Compression Mechanism

The cholinergic anti-inflammatory pathway (CAP) is the efferent vagal brake on immune activation. Vagal tone → acetylcholine release → α7nAChR on macrophages → cytokine inhibition. Low vagal tone means inadequate CAP function. Inadequate CAP function means elevated cytokine production. Elevated cytokines cross the blood-brain barrier and disrupt hypothalamic and brainstem autonomic control centers, further compressing HRV.

The critical finding for measurement is the shared efferent vagal drive between HRV and CAP function: a cholinergic brain network that increases CAP activity simultaneously increases instantaneous HRV. HRV and CAP are not merely correlated — they share the same mechanism. Low HRV is not just a cardiovascular risk marker. It is a direct indicator that the anti-inflammatory brake is impaired. See Central Reference anchor A60.

This means HRV is measuring the allostatic debt accumulation of the immune system in real time, before inflammatory biomarkers rise to clinical significance. The HRV signal precedes the CRP rise. It is the early warning that clinical biomarker panels cannot provide.

### 2d. AUTO↔MOD — The Behavioral Signature

When autonomic compression from the three contracts below has accumulated sufficiently, the modulation layer shows characteristic behavioral signatures that are direct readouts of allostatic debt.

The incomplete exhale is the primary signature. Normal exhale completes fully, allowing the diaphragm to return to its resting position and generating the maximum RSA amplitude for the next breath cycle. Under accumulated load, the exhale is terminated early — a thermodynamic adaptation that maintains residual thoracic pressure as a buffer against further autonomic compression. This incomplete exhale progressively reduces RSA amplitude, narrows the oscillatory window, and compresses HRV further.

The cognitive signature — tunnel vision, recursive thinking, reduced lateral integration — is the downstream consequence of this oscillatory compression on the modulation layer. Precision loss is not a psychological event. It is the behavioral readout of an oscillatory system whose amplitude has been compressed by accumulated regulatory debt across all four contracts simultaneously.

**Precision-Geometry Integration:** In the precision framework, $P = R/D_T$ where $R$ is sync duration and $D_T$ is timing distance. Allostatic load reduces $P$ through two mechanisms:

$$P(L^*) = \frac{R_0 e^{-\mu_c L^*}}{D_0 (1 + \lambda_c L^*)}$$

where:
- $R_0$ is baseline sync duration
- $D_0$ is baseline timing distance
- $\mu_c$ is the sync duration decay coefficient
- $\lambda_c$ is the timing distance inflation coefficient

The full effective precision includes the substrate and uniformity constraints:

$$P_{eff}(L^*) = P(L^*) \cdot O_{pathway}(L^*) \cdot U_C(L^*)$$

where $U_C(L^*) = 1/(1 + \nu L^*)$ is the CO₂ uniformity degraded by load, and $O_{pathway}$ is the substrate constraint (functional form unspecified pending calibration; see Central Reference §2.8).

The incomplete exhale directly reduces $U_C$ by creating uneven CO₂ distribution across the alveolar space, which increases the variance term in the uniformity equation:

$$\frac{dU_C}{dt} = -\rho \cdot \text{Var}_i[C_i(t)]$$

and load increases this variance directly: $\text{Var}_i[C_i(t)] \propto L^*$. See Central Reference §3.3 for the full precision equations.

### 2e. GLYMPH↔AUTO — The Clearance Failure Amplifier

The glymphatic clearance contract establishes that diaphragmatic pressure mechanics drive CSF flow through perivascular channels, with slow wave sleep providing the primary clearance window. Allostatic load intersects this contract through three mechanisms:

1. **Metabolic load → breathing pattern → reduced clearance:** High load drives faster, shallower breathing, reducing intrathoracic pressure differential and CSF pulsatility. The load-dependent breathing pattern is:

$$V_T(L^*) = V_T^0 e^{-\alpha L^*}$$

where $V_T$ is tidal volume and $V_T^0$ is baseline.

2. **Sympathetic dominance → reduced slow wave architecture:** Chronic load suppresses the vagal tone required for deep sleep architecture, reducing the clearance window proportion:

$$\text{SWS\%}(L^*) = \text{SWS\%}_0 - \beta L^*$$

3. **Clearance failure → neuroinflammation → further load:** Reduced clearance permits amyloid and tau accumulation, triggering microglial activation and neuroinflammation that further impairs sleep architecture — the loop handoff to IMMUNE↔AUTO:

$$L^* \xrightarrow{\text{reduced clearance}} \text{neuroinflammation} \xrightarrow{\text{sleep disruption}} L^*$$

The full accumulation-inflammation loop can be expressed as:

$$\frac{dL^*}{dt} = \lambda_{\text{met}} + \lambda_{\text{inflam}} - \lambda_{\text{clear}} \cdot \text{SWS\%}(L^*)$$

where $\lambda_{\text{met}}$ is metabolic accumulation rate, $\lambda_{\text{inflam}}$ is inflammation-driven accumulation, and $\lambda_{\text{clear}}$ is the clearance rate per unit SWS. This loop is formalized in Central Reference §4 (glymphatic recovery loop).

### 2g. SALIENCE↔AL — The Perseveration Load

The trap accumulates load when the latch holds. The perseveration loop accumulates load when the latch releases and re-forms on the same region.

**The mechanism:**

```
Latch releases → PE commits → region clears
    ↓
Salience still hits → interrupt re-fires on same region
    ↓
New latch forms → new tension
    ↓
ATP-brace cost accumulates across cycles
    ↓
Vagal tone compressed across cycles
    ↓
CAP function impaired across cycles
    ↓
L*_perseveration: the load component from repeated latch cycles
```

**The key difference from the trap:**

| | Trap | Perseveration loop |
|---|---|---|
| Latch holds | Continuously | Cyclically |
| PE commits | Never | Each cycle |
| ATP cost | Continuous | Repeated |
| Vagal compression | Sustained | Repeated |
| Load accumulation | Monotonic | Stepwise |

**The perseveration loop is more costly than the trap in one way and less costly in another.** More costly because each cycle burns ATP for the release *and* the re-formation. Less costly because the PE does commit each cycle — the system is processing, not just holding.

**But over time, the perseveration loop accumulates load faster than the trap** because the cycle rate is higher. Each re-fire is a new interrupt, a new investment, a new latch.

**The load component:**

$$L^*_{perseveration} = \frac{\text{cycle rate} \times \text{ATP cost per cycle}}{\text{baseline}}$$

**Measurement protocol:**

1. **Interrupt re-fire rate** — ERP by region
2. **Routing weight persistence** — frontal alpha asymmetry after latch release
3. **ATP-brace cost per cycle** — surface EMG by region
4. **Vagal recovery time** — HRV recovery between cycles

**The protocol:** Measure the re-fire rate. Measure the routing weight persistence. Measure the ATP cost per cycle. The perseveration load is the product.

**Clinical signature:** Rumination, intrusive thoughts, chronic worry, "can't stop thinking about it."

**Source:** Salience Interrupt v1.3 §2.11, SAL-35–37.

### 2h. SALIENCE↔AL — The Release-Triggered Load

The trap accumulates load when the latch holds. The perseveration loop accumulates load when the latch releases and re-forms. The release-triggered re-salience accumulates load when the release *itself* surfaces the PE.

**The mechanism:**

```
Latch holds → PE suppressed → no load from processing
    ↓
Release begins → PE surfaces → processing begins
    ↓
Surfaced PE fires new interrupt → new latch forms
    ↓
Failed release → the hold continues
    ↓
Each failed release attempt costs ATP without committing the PE
    ↓
L*_release-triggered: the load component from failed release attempts
```

**The key difference:**

| | Trap | Perseveration loop | Release-triggered |
|---|---|---|---|
| Latch holds | Continuously | Cyclically | Continuously |
| PE commits | Never | Each cycle | Never |
| ATP cost | Continuous | Repeated | Repeated + failed releases |
| Vagal compression | Sustained | Repeated | Sustained + spike at release |
| Load accumulation | Monotonic | Stepwise | Stepwise + failed release cost |

**The release-triggered load is the most insidious** because each release attempt costs ATP without committing the PE. The system is paying for the release *and* paying for the re-lock. The net effect is more load than if the release had never been attempted.

**This is why "just relax" fails.** The relaxation attempt triggers the re-fire. The re-fire costs more than the original hold.

**The load component:**

$$L^*_{release-triggered} = \frac{\text{release attempts} \times \text{ATP cost per failed release}}{\text{baseline}}$$

**Measurement protocol:**

1. **Release attempt count** — conscious attempts to release
2. **Failed release rate** — re-fire at release
3. **ATP-brace cost per failed release** — surface EMG by region
4. **Vagal recovery time** — HRV recovery after failed release

**Clinical signature:** "It comes back when I relax," trauma re-experiencing during rest, "I was fine until I stopped."

**Source:** Salience Interrupt v1.3 §2.12, SAL-38–41.

### 2i. SALIENCE↔AL — The Encoding Load

The trap accumulates load when the latch holds. The perseveration loop accumulates load when the latch releases and re-forms. The release-triggered re-salience accumulates load when the release surfaces the PE. The encoding window determines whether the load is committed or released.

**The mechanism:**

```
Latch holds → PE suppressed → no load from processing
    ↓
Exhale begins → PE surfaces → processing begins
    ↓
    ├── Context unchanged → PE re-encodes with same gain → RE-LOCK → load accumulates
    │
    └── Context changed → PE re-encodes with less gain → RELEASE → no load
```

**The key difference:**

| | Trap | Perseveration | Release-triggered | Encoding window |
|---|---|---|---|---|
| Latch holds | Continuously | Cyclically | Continuously | Continuously |
| PE commits | Never | Each cycle | Never | At release |
| Encoding gain | N/A | Same | N/A | Reduced |
| Load accumulation | Monotonic | Stepwise | Stepwise + failed releases | None (if context changes) |

**The encoding window is the exit from all three failure modes.** The trap exits through the exhale. The perseveration loop exits through routing redistribution. The release-triggered re-salience exits through capacity. The encoding window is the mechanism that makes the exit *stick* — the PE commits with less gain, so the latch doesn't re-form.

**This is why the encoding window is the master exit.** It is the mechanism that determines whether the load is released or re-committed.

**The load component:**

$$L^*_{encoding} = \frac{\text{release attempts} \times \text{re-encoding gain}}{\text{baseline}}$$

**Measurement protocol:**

1. **Release attempt count** — conscious release attempts
2. **Re-encoding gain** — EMG in locked region after release
3. **Context change** — self-report of recontextualization during exhale
4. **Vagal recovery time** — HRV recovery after release

**Clinical signature:** "It keeps coming back," insight resistance, rumination that doesn't resolve despite awareness.

**Source:** Salience Interrupt v1.3 §2.13, SAL-42–45.

### 2j. SALIENCE↔AL — The Somatic Load Path

Movement is a routing lever. It redistributes Θ_r(t) across the homunculus, breaking both the perseveration loop and the release-triggered re-salience. The somatic load path is the allostatic cost of *not* using the movement lever when the routing is concentrated.

**The mechanism:**

```
Latch holds → routing concentrated on region i
    ↓
Movement available → Θ_r redistributes → latch releases
    ↓
OR
    ↓
Movement unavailable → routing stays concentrated
    ↓
Latch holds → ATP-brace cost accumulates → L*_somatic
```

**The load component:**

$$L^*_{somatic} = \frac{\text{concentrated routing time} \times \text{ATP-brace cost}}{\text{baseline}}$$

**Measurement protocol:**

1. **Movement availability** — time spent in static posture vs. movement
2. **Routing concentration** — frontal alpha asymmetry during static periods
3. **ATP-brace cost** — surface EMG by region during static periods
4. **Vagal recovery time** — HRV recovery after movement vs. rest

**The clinical signature:** The compulsion to do physical tasks when upset. Folding laundry, doing dishes, sweeping. The movement is the routing redistribution mechanism. The system is trying to distribute the manifold. It doesn't know why. It just knows the task helps.

**Why movement failure predicts load:**

Static posture holds the diaphragm's mechanical range compressed. The breath cannot build CO₂. The routing concentrates. The latch holds. The load accumulates.

**This is why movement is not supplementary to breathing.** Movement restores the diaphragm's mechanical range *and* redistributes routing. Without it, the breath pattern alone does not prevent concentration.

**Source:** Salience Interrupt v1.3 §2.5.2, §2.11.2, §6.2, SAL-33, SAL-35, SAL-46, SAL-47.

---

## 3. The Debt Trajectory

### 3a. Regulatory Debt as Energy Accounting

Allostatic load is borrowed regulatory capacity that was not returned.

The muscle analogy is mechanistically exact. Cortisol is the biochemical mechanism by which the body converts structural tissue — muscle protein — into immediate energy substrate when regulatory accounting goes negative. The body borrows from structural reserve to fund regulatory demand. This is not metaphor. It is the literal mechanism by which chronic allostatic load produces muscle catabolism, impaired glycogen resynthesis, and the physical depletion that persists beyond rest.

### 3b. The Three Zones

The debt trajectory has three zones:

**Zone 1 — Debt Within Recovery Range**
Regulatory borrowing occurs across the day. Each loop activation, each incomplete exhale, each glycemic event draws on the reserve. But overnight recovery — glymphatic clearance, HPA axis reset, parasympathetic dominance in deep sleep — returns the system to baseline. Morning resting HRV reflects the full reserve. The delta HRV protocol shows significant response capacity. Normal circadian decline in HRV across the waking day is Zone 1 behaviour — it is distinguished from pathological debt by recovery: the morning baseline is fully restored each day. Pathological debt is the excess decline that persists overnight and drives the morning baseline progressively lower across consecutive days.

**Zone 2 — Debt Exceeding Daily Recovery**
Accumulation rate exceeds recovery rate. Each morning starts slightly lower than the last. The resting HRV baseline drifts downward across consecutive days. The delta HRV response shrinks — not because slow breathing doesn't work, but because there is less reserve to restore. This is the chronic stress signature that clinical biomarker panels eventually confirm but HRV tracking detects weeks earlier.

**Zone 3 — Debt at Structural Ceiling**
The system is at or near maximum allostatic load. Resting HRV is floored. The delta HRV response is near zero regardless of breathing protocol quality. Inflammatory markers are elevated. The CO₂ tolerance window is narrow — Control Pause below 15 seconds, and typically below 10 in severe cases. This is the state in which slow breathing interventions produce minimal acute benefit because the structural substrate for oscillatory recovery is compromised, not merely suppressed.

The compensatory rate mechanism confirms Zone 3 status independently. When the Bohr shift is impaired by chronically narrow CO₂ tolerance and compressed vagal tone, each cardiac cycle delivers less oxygen per pump. The system's only available compensation is increased pump rate. A sleep RHR that remains above 65 BPM regardless of sleep depth is the cardiovascular signature of a system whose extraction efficiency is structurally compromised — not depleted from today's load, but running a continuous compensatory loop the overnight recovery window cannot close.

The trajectory is directional and self-compounding through the same mechanism described in the Manifold Schema (Robinson, 2026a): each cycle of reduced precision recovery produces more false cache hits, raises curvature, narrows the comparison window, and increases the rate of subsequent debt accumulation. The system seals itself from the inside without any internal signal that sealing is occurring. The collapse sequence — Stages 1–6 — is formalized in Central Reference §5b.

---

## 4. The ND Precision-Collapse Paradox

ND populations present a distinctive pattern that standard models cannot explain: sustained high cognitive performance under fasted conditions followed by sudden, catastrophic collapse. The paradox resolves when the MET↔AUTO precision spike and the interoceptive routing shift are recognized as competing for the same gain-control loop.

### 4a. The Fasted State Paradox

The fasted state produces a precision spike: glucose availability shifts, MET↔AUTO activates with higher efficiency, inference sharpens, and the system *feels* like it is running at peak capacity. Simultaneously, $I^*$ routing reallocates from hunger detection to cognitive processing. The hunger signal is not suppressed — it is *processed out*. The system cannot afford to process both high-precision cognitive work and interoceptive monitoring simultaneously.

Metabolic debt accumulates silently. The precision spike masks the load accumulation. The system feels sharp while the budget is depleting. When $L^*$ exceeds remaining capacity, $C_s$ drops abruptly — from high performance to collapse with minimal warning. Recovery requires food + rest + load clearance. The hunger signal is processed *post*-collapse, not *pre*-collapse.

### 4b. The Field's Misattribution

The field attributes this to low blood sugar. The framework attributes it to the gain-control loop: the system routed $I^*$ away from hunger, precision spiked on cognitive work, and metabolic debt accumulated until the budget was gone. The collapse was not a failure of willpower or planning. It was the geometric consequence of allocating routing capacity to one channel until the other channel's signal dropped below the processing threshold.

### 4c. ND-Specific Amplification

ND systems show this pattern more clearly because:
- Interoceptive routing flexibility is higher — hunger can be routed out more completely
- Precision sensitivity to fuel is higher — the fasted precision spike is larger
- Collapse threshold is narrower — the drop is abrupt rather than gradual

The ND population is therefore the highest-signal cohort for observing the mechanism, not a pathological outlier requiring separate explanation.

---

## 5. The Measurement Protocol

A complete allostatic load assessment requires seven measurements, most of which require only a consumer wearable and basic clinical equipment.

### 5a. Resting HRV Baseline
5-minute supine rest. HRV measured via standard photoplethysmography (wrist wearable) or chest strap ECG. Establishes current system position. High resting HRV: low debt or Zone 1. Low resting HRV: Zone 2 or Zone 3 — ambiguous without the delta.

### 5b. Resting Heart Rate Floor During Sleep

Deep sleep resting heart rate is the compensatory rate metric that pairs with delta HRV. When oxygen extraction efficiency is impaired — through compressed vagal tone, reduced Bohr shift from narrow CO₂ tolerance, or continuous inflammatory load — the system compensates with increased pump frequency. A high sleep RHR is not a cardiac problem. It is the system admitting it cannot extract efficiently per cycle and increasing delivery rate to compensate.

$$RHR_{sleep} \propto \frac{1}{\text{extraction efficiency}} \propto \frac{1}{\text{Bohr shift}} \propto \frac{1}{HRV}$$

- Sleep RHR `<45` BPM: extraction efficiency high, vagal tone intact, Zone 1
- Sleep RHR `45-60` BPM: moderate efficiency, some load present, Zone 2
- Sleep RHR `60-65` BPM: borderline — elevated enough to warrant monitoring
- Sleep RHR `>65` BPM: extraction efficiency compromised, inflammatory or autonomic load running continuously overnight, Zone 3

The two metrics together tell the complete story. Delta HRV measures remaining precision capacity. Sleep RHR measures how hard the system is compensating for what it cannot efficiently extract. A person with low delta HRV and high sleep RHR is running a continuous compensatory loop that is not clearing overnight.

### 5c. Delta HRV Response
Slow breath protocol immediately following baseline: 5 minutes at approximately 6 breaths per minute, full diaphragmatic engagement, complete exhale. HRV measured across final 2 minutes of protocol. $\Delta HRV = HRV_{slow-breath} - HRV_{baseline}$.

- $\Delta HRV > 15$ ms: Zone 1. Significant reserve remaining.
- $\Delta HRV$ 5-15 ms: Zone 2. Debt accumulating, recovery rate potentially compromised.
- $\Delta HRV < 5$ ms: Zone 3. System at or near ceiling.

### 5d. CO₂ Tolerance Threshold
Control Pause: after a normal exhale, measure seconds of comfortable breath hold before first urge to breathe. No equipment required.

- $>40$ seconds: Wide tolerance window. HRV ceiling is high.
- `25-40` seconds: Moderate window. Manageable debt.
- `10-25` seconds: Narrow window. Debt affecting tolerance range.
- `<10` seconds: Minimal window. Chemoreflex fires at minimal CO₂ rise. Recovery interventions have limited effect.

### 5e. Exhale Completeness Ratio
Qualitative assessment: does the exhale complete fully before the next inhale begins, or does the next inhale begin while exhalation force is still present? The incomplete exhale is the real-time behavioral signature of Zone 2/3 debt. Trainable through conscious attention. Its presence indicates the AUTO↔MOD contract is already showing adaptation.

### 5f. Sleep Architecture Assessment
Slow wave sleep proportion (from wearable sleep staging) indicates the clearance window depth:

- SWS\% $> 20\%$: Adequate clearance window
- SWS\% $15-20\%$: Reduced window, accumulation likely exceeding clearance
- SWS\% $< 15\%$: Critically reduced window, accumulation guaranteed

Sleep respiratory rate is the compensatory metric for elevated chemoreflex drive:

- Sleep respiratory rate `12-14` BPM: Normal
- Sleep respiratory rate `14-17` BPM: Elevated chemoreflex drive
- Sleep respiratory rate $>17$ BPM: Chemoreflex chronically elevated

### 5g. Week HRV Variance
The load-responsive range over a week of normal activity:

- Dynamic, load-responsive: System can vary HRV appropriately across demand levels
- Partially responsive: Some load responsiveness remains
- Flat regardless of load or rest: System is at or near ceiling

**This is the key metric.** As Okawara, H., Shiraishi, Y., Sato, K., Nakamura, M., & Katsumata, Y. (2024) demonstrated, the variance of daily HRV measurements predicts anxiety and productivity loss better than the mean. The field has been treating variance as noise. The framework identifies it as the signal. This is the measurement that P-AL-011 — the central prediction — tests directly.

### 5h. Inflammatory Biomarkers (Secondary Validation)
CRP and IL-6 confirm Zone 2/3 debt when present but lag behind HRV signal by days to weeks. They are confirmation, not early detection. A rising HRV floor with low delta response will predict inflammatory marker elevation before it appears.

### 5i. The Complete Measurement Table

| Metric | Zone 1 | Zone 2 | Zone 3 — Chronic Load |
|---|---|---|---|
| Sleep HRV | High, clear overnight peak | Moderate, partial rise | Flat, no overnight rise |
| Sleep RHR | `<45` BPM | `45-60` BPM | `>65` BPM — loop running overnight |
| Delta HRV slow breath | `>15`ms | `5-15`ms | `<5`ms |
| Control Pause | `>40` seconds | `25-40` seconds | `<15` seconds (severe `<10`) |
| Sleep respiratory rate | `12-14` BPM | `14-17` BPM | `>17` BPM — chemoreflex elevated |
| Week HRV variance | Dynamic, load-responsive | Partially responsive | Flat regardless of load or rest |
| Exhale completeness | Full | Partial | Incomplete |
| SWS proportion | `>20\%` | `15-20\%` | `<15\%` |
| CRP/IL-6 | Normal | Elevated (lagged) | Highly elevated |

---

## 6. The Composite Load Equation

### 6a. The Within-Person Baseline Method

Each component is calculated as a drift from the individual's own baseline:

$$L^*_{component} = \frac{Value_{current} - Baseline_{component}}{Baseline_{component} - Floor_{component}}$$

Where:
- $Baseline_{component}$ is the individual's 30-day median for that component
- $Floor_{component}$ is the individual's 30-day minimum (for markers that decrease with load) or maximum (for markers that increase with load)
- $Value_{current}$ is the current measurement

**This is a within-person calculation.** It does not require population norms. It requires only that you measure the same person over time.

**Why 30 days:** 30 days provides a stable baseline that captures weekly and circadian variation while remaining responsive to change. The optimal window length is an empirical question; 30 days is proposed as a provisional default, and sensitivity to window length (14, 30, 60 days) should be tested as part of P-AL-008 validation.

### 6b. Component Measurement Details

#### L*_HRV — HRV Baseline Drift

**What it measures:** The failure of HRV to return to maximal sleep HRV during recovery windows. This is the direct measurement of regulatory debt.

**Measurement protocol:**

1. Collect sleep HRV for 30 days (Oura, Garmin, Apple Watch, or any wearable with RMSSD)
2. Identify maximal sleep HRV ($HRV_{max}$) — the highest RMSSD observed in deep sleep over the 30-day period
3. Calculate current sleep HRV ($HRV_{current}$) — the 7-day rolling average of sleep HRV
4. Calculate drift:

$$L^*_{HRV} = \frac{HRV_{max} - HRV_{current}}{HRV_{max} - HRV_{floor}}$$

Where $HRV_{floor}$ is the lowest sleep HRV observed during a period of known recovery (e.g., after a vacation) — or the 5th percentile of the 30-day distribution.

**Interpretation:**

| $L^*_{HRV}$ | Meaning | Clinical Signature |
|---|---|---|
| 0.0 - 0.2 | Full recovery | HRV returns to max within 1-2 nights |
| 0.2 - 0.4 | Mild debt | HRV consistently below max, but trending up |
| 0.4 - 0.6 | Moderate debt | HRV consistently below max, not recovering |
| 0.6 - 0.8 | Severe debt | HRV depressed, sleep poor |
| 0.8 - 1.0 | Critical debt | HRV floor, recovery failure |

#### L*_RHR — Sleep RHR Elevation

**What it measures:** Elevated resting heart rate during sleep indicates that background autonomic demand persists — the system is still running high even during the recovery window.

**Measurement protocol:**

1. Collect sleep RHR for 30 days (any wearable)
2. Identify minimal sleep RHR ($RHR_{min}$) — the lowest RHR observed during deep sleep over the 30-day period
3. Calculate current sleep RHR ($RHR_{current}$) — the 7-day rolling average of sleep RHR
4. Calculate elevation:

$$L^*_{RHR} = \frac{RHR_{current} - RHR_{min}}{RHR_{max} - RHR_{min}}$$

Where $RHR_{max}$ is the highest sleep RHR observed during a period of known load (e.g., after an illness) — or the 95th percentile of the 30-day distribution.

**Interpretation:**

| $L^*_{RHR}$ | Meaning | Clinical Signature |
|---|---|---|
| 0.0 - 0.2 | Full recovery | RHR at floor during sleep |
| 0.2 - 0.4 | Mild demand | RHR slightly elevated |
| 0.4 - 0.6 | Moderate demand | RHR consistently elevated |
| 0.6 - 0.8 | Severe demand | RHR elevated, poor sleep |
| 0.8 - 1.0 | Critical demand | RHR at max, no recovery |

#### L*_temp — Sleep Temperature Elevation

**What it measures:** Elevated body temperature during sleep indicates inflammatory load persists — the system is still fighting something during the recovery window.

**Measurement protocol:**

1. Collect sleep temperature for 30 days (wearables with temperature sensors — Oura, Garmin, Apple Watch)
2. Identify minimal sleep temperature ($Temp_{min}$) — the lowest temperature observed during sleep over the 30-day period
3. Calculate current sleep temperature ($Temp_{current}$) — the 7-day rolling average of sleep temperature
4. Calculate elevation:

$$L^*_{temp} = \frac{Temp_{current} - Temp_{min}}{Temp_{max} - Temp_{min}}$$

Where $Temp_{max}$ is the highest sleep temperature observed during a period of known illness or high inflammation — or the 95th percentile of the 30-day distribution.

**Interpretation:**

| $L^*_{temp}$ | Meaning | Clinical Signature |
|---|---|---|
| 0.0 - 0.2 | Full recovery | Temperature at floor during sleep |
| 0.2 - 0.4 | Mild inflammation | Temperature slightly elevated |
| 0.4 - 0.6 | Moderate inflammation | Temperature consistently elevated |
| 0.6 - 0.8 | Severe inflammation | Temperature elevated, poor sleep |
| 0.8 - 1.0 | Critical inflammation | Temperature at max, no recovery |

#### L*_inflam — Chronic Inflammatory Tone

**What it measures:** Chronic elevation of inflammatory markers indicates long-term regulatory debt — the system has been borrowing from structural reserves for an extended period.

**Measurement protocol:**

1. Collect inflammatory markers (CRP, IL-6, TNF-α) — at baseline and at intervals
2. Identify minimal inflammatory tone ($Inflam_{min}$) — the lowest observed value for each marker (population bottom quartile, or individual's nadir during wellness)
3. Calculate current inflammatory tone ($Inflam_{current}$) — the current measurement
4. Calculate elevation:

$$L^*_{inflam} = \frac{Inflam_{current} - Inflam_{min}}{Inflam_{max} - Inflam_{min}}$$

Where $Inflam_{max}$ is the highest observed value for each marker (population top quartile, or individual's peak during illness), normalized across markers:

$$L^*_{inflam} = \frac{L^*_{CRP} + L^*_{IL-6} + L^*_{TNF-\alpha}}{3}$$

Each marker is normalized to [0,1] before averaging, so the composite is unit-free. CRP, IL-6, and TNF-α contribute equally by rank position within their own reference ranges, not by absolute magnitude.

**Interpretation:**

| $L^*_{inflam}$ | Meaning | Clinical Signature |
|---|---|---|
| 0.0 - 0.2 | No chronic inflammation | Markers at floor |
| 0.2 - 0.4 | Mild inflammation | Markers slightly elevated |
| 0.4 - 0.6 | Moderate inflammation | Markers consistently elevated |
| 0.6 - 0.8 | Severe inflammation | Markers elevated, clinical significance |
| 0.8 - 1.0 | Critical inflammation | Markers at max, systemic involvement |

#### L*_resp — Respiratory Inefficiency (Bracing Proxy)

**What it measures:** Diaphragm excursion limitation and respiratory inefficiency — the visible expression of bracing, which is a load-driven compensation pattern.

**Measurement protocol:**

1. Measure respiratory rate (RR) — breaths per minute
2. Measure tidal volume (Vt) — volume per breath
3. Calculate Diaphragm Excursion Index:

$$DEI = \frac{V_t}{RR}$$

4. Identify maximal DEI ($DEI_{max}$) — the highest observed DEI during known recovery (deep sleep, after vacation, during relaxation)
5. Calculate current DEI ($DEI_{current}$) — current measurement
6. Calculate load:

$$L^*_{resp} = \max\left(0, \min\left(1, \frac{DEI_{max} - DEI_{current}}{DEI_{max} - DEI_{floor}}\right)\right)$$

Where $DEI_{floor}$ is the lowest observed DEI during known load (stress, anxiety, pain), or the 5th percentile of the distribution. The clipping to [0,1] prevents overshoot when a current measurement exceeds the historical maximum — the interpretation table's 0.8–1.0 range is the maximum reachable after clipping.

**Alternative measurement (ultrasound):** Direct measurement of diaphragm excursion during respiration. The diaphragm's descent during inhalation is a direct measure of available breathing range.

**Interpretation:**

| $L^*_{resp}$ | Meaning | Clinical Signature |
|---|---|---|
| 0.0 - 0.2 | Full respiratory efficiency | DEI at max, diaphragm free |
| 0.2 - 0.4 | Mild bracing | DEI slightly reduced |
| 0.4 - 0.6 | Moderate bracing | DEI consistently reduced, accessory muscles engaged |
| 0.6 - 0.8 | Severe bracing | DEI reduced, diaphragmatic lock |
| 0.8 - 1.0 | Critical bracing | DEI at floor, severe restriction |

### 6c. The Composite Load Equation

$$L^* = w_1 L^*_{HRV} + w_2 L^*_{RHR} + w_3 L^*_{temp} + w_4 L^*_{inflam} + w_5 L^*_{resp} + w_6 L^*_{salience} + w_7 L^*_{perseveration} + w_8 L^*_{release-triggered} + w_9 L^*_{encoding} + w_{10} L^*_{somatic}$$

With weights:

$$w_1 + w_2 + w_3 + w_4 + w_5 + w_6 + w_7 + w_8 + w_9 + w_{10} = 1$$

**Revised default weights (proposed — to be calibrated on a training cohort and validated on a held-out cohort before evaluating P-AL-008):**

| Component | Weight | Rationale |
|---|---|---|
| $L^*_{HRV}$ | 0.20 | HRV baseline drift — earliest indicator of cumulative debt |
| $L^*_{RHR}$ | 0.15 | Sleep RHR elevation — persistent background demand |
| $L^*_{temp}$ | 0.10 | Temperature elevation — inflammatory load |
| $L^*_{inflam}$ | 0.15 | Chronic inflammation — long-term regulatory debt |
| $L^*_{resp}$ | 0.10 | Respiratory inefficiency — bracing and diaphragm lock |
| $L^*_{salience}$ | 0.10 | Unresolved latch load — the raw unit of debt |
| $L^*_{perseveration}$ | 0.08 | Repeated-latch load — cycle rate matters |
| $L^*_{release-triggered}$ | 0.05 | Failed-release load — the cost of trying |
| $L^*_{encoding}$ | 0.04 | Failed-encoding load — the cost of not changing context |
| $L^*_{somatic}$ | 0.03 | Somatic load — the cost of not moving |

Weights are not free parameters. They are estimated on a training set and frozen before the P-AL-008 test. Any post-hoc adjustment invalidates the prediction.

**Composite versus diagnostic interpretation:** The composite $L^*$ equation reflects total load across all components simultaneously. It is appropriate when multiple components are elevated and the question is overall debt magnitude. For diagnostic purposes — identifying where the debt is concentrated and what to treat — use the **maximum component value** as the primary indicator:

$$L^*_{diagnostic} = \max(L^*_{HRV},\ L^*_{RHR},\ L^*_{temp},\ L^*_{inflam},\ L^*_{resp})$$

A person with $L^*_{resp} = 1.0$ and all other components at 0.0 has $L^* = 0.10$ under fixed weights — a Zone 1 classification — but is at maximum bracing load. The profile table in Section 7a captures this: the component maximum drives treatment targeting, not the composite score. The composite score answers "how much total debt?" The maximum component answers "where is the debt?"

This distinction is formalized in Central Reference §3.7 Note 4 as component REQT:

$$REQT_{component} = REQT_{composite} \wedge (\max_i L^*_i < L^*_{critical,i})$$

A system passes REQT only if both total load is manageable AND no single component is at critical level. This prevents false-positive qualification of systems with isolated severe debt.

The component critical load $L^*_{critical,i}$ is an individual calibration parameter — not a population constant. Calibration protocol: measure $L^*_i$ for each component across a range of load states, identify the point at which the corresponding functional domain (cognitive performance, autonomic regulation, inflammatory response) shows measurable degradation, and fit the threshold per individual. See Central Reference §2.9 for the specification.

The weights are adjustable based on individual presentation. A person with normal inflammatory markers but severe HRV drift gets a higher $L^*$ from the HRV component. A person with elevated CRP but stable HRV gets a higher $L^*$ from the inflammatory component.

**Note on measurement burden:**

The ten-component equation requires laboratory equipment. The minimum viable measurement (§6d) requires only a wearable. Both measure $L^*$. The difference is resolution.

| Tier | Instruments | Components | What it identifies |
|---|---|---|---|
| **Consumer-grade** | Wearable (Oura, WHOOP, Garmin, Apple) | $L^*_{HRV}$, $L^*_{RHR}$, $L^*_{temp}$, $L^*_{resp}$ (partial via respiratory rate) | That load is present. Trajectory direction. Zone position. |
| **Clinical-grade** | Wearable + Control Pause + exhale assessment | The above + $L^*_{salience}$ (partial via exhale completeness) | Where the load is concentrated. Which contract is failing. |
| **Research-grade** | Full lab: wearable + blood draw + spirometry + surface EMG + ERP | All ten components | Full profile. Component resolution. Mechanism identification. |

The consumer-grade tier gives most people exactly the data they need. The wearable already measures HRV drift, sleep RHR, temperature, and respiratory rate. The Control Pause is free. The exhale completeness assessment is free. That is six of the ten components with no lab equipment.

The research-grade tier is for mechanism research. It identifies which failure mode is dominant — perseveration vs. release-triggered vs. encoding vs. somatic — so the intervention can be targeted. This is the tier for clinical trials, for Schumann-style follow-ups, for the P-AL predictions that require component resolution.

Both tiers measure the same variable. The research-grade tier does not measure a different thing. It measures the same $L^*$ with higher resolution. The consumer-grade tier is not a "proxy for the real measurement." It is the same measurement at lower resolution.

### 6d. The Minimum Viable Measurement

**If you have only one instrument (HRV), you can still measure load:**

1. Morning HRV — within 10 minutes of waking, before movement or caffeine
2. Evening HRV — before bed, after the day's load has accumulated
3. Sleep HRV — during deep sleep, after recovery has begun

**The minimum viable protocol:**

$$L^* \approx \frac{1}{2} \left( \frac{HRV_{morning} - HRV_{evening}}{HRV_{morning} - HRV_{floor}} + \frac{HRV_{max} - HRV_{sleep}}{HRV_{max} - HRV_{floor}} \right)$$

**Note on formula structure:** The additive average is used rather than a product. A multiplicative formula would allow a single near-zero component to collapse the output to zero even when the other component shows maximum load — masking single-domain failures. The additive average preserves each component's contribution independently.

**Interpretation:** If morning HRV is high, evening HRV is low, and sleep HRV doesn't recover to morning levels, load is accumulating. If morning HRV is low, load is already high. If evening HRV is close to morning HRV, load is low (or the system is locked at low amplitude).

**Why this works:** The morning-evening difference captures daily load accumulation. The sleep-to-morning gap captures overnight recovery. When both are large, load is accumulating. When both are small, load is stable or low.

---

## 7. Individual Load Profiles

### 7a. Profile Types

$L^*$ is not a single number. It is a profile across components:

| Profile Type | $L^*_{HRV}$ | $L^*_{RHR}$ | $L^*_{temp}$ | $L^*_{inflam}$ | $L^*_{resp}$ | $L^*_{sal}$ | $L^*_{pers}$ | $L^*_{rel}$ | $L^*_{enc}$ | $L^*_{som}$ | Signature |
|---|---|---|---|---|---|---|---|---|---|---|---|
| High HRV load | High | Low | Low | Low | Low | Mod | Mod | Low | Low | Low | Autonomic debt from chronic trap cycles |
| High inflammatory load | Low | Low | High | High | Low | Mod | Low | Low | Low | Low | Immune debt from unresolved latches |
| High bracing load | Low | Low | Low | Low | High | High | Low | Low | Low | Low | Respiratory debt from ATP-brace holds |
| High total load | High | High | High | High | High | High | High | High | High | High | Full debt — trap compounds |
| Salience-dominant | Mod | Low | Low | Low | Mod | High | High | Low | Low | Low | Unresolved latch debt + perseveration |
| Perseveration-dominant | Mod | Low | Low | Low | Mod | Mod | High | Low | Low | Low | Rumination debt — "can't stop thinking" |
| Release-triggered-dominant | Mod | Low | Low | Low | Mod | Mod | Low | High | Low | Low | Failed-release debt — "I can't relax" |
| Encoding-dominant | Mod | Low | Low | Low | Mod | Mod | Low | Mod | High | Low | Failed-encoding debt — "it keeps coming back" |
| Somatic-dominant | Mod | Low | Low | Low | High | Mod | Mod | Low | Low | High | Static-posture debt — "I can't move right now" |

**Interpretation:** The profile tells you where the debt is concentrated. Treatment targets the component with the highest load first.

### 7b. Treatment Targeting

| Target | Intervention | Mechanism |
|---|---|---|
| $L^*_{HRV}$ | HRV biofeedback, sleep hygiene | Increase reinvestment capacity |
| $L^*_{RHR}$ | Autonomic regulation, breathing training | Reduce background demand |
| $L^*_{temp}$ | Anti-inflammatory protocols, stress reduction | Reduce inflammatory tone |
| $L^*_{inflam}$ | Anti-inflammatory protocols, lifestyle change | Clear chronic inflammation |
| $L^*_{resp}$ | Breathing training, posture correction, diaphragm training | Restore respiratory efficiency |
| $L^*_{salience}$ | Complete exhale training, pre-sleep clearance | Release unresolved latches |
| $L^*_{perseveration}$ | Movement, task-switching, gain-change interventions | Redistribute routing; break the re-fire cycle |
| $L^*_{release-triggered}$ | Capacity training, gain-change interventions, titration | Raise Λ_lock; reduce salience of surfaced PE |
| $L^*_{encoding}$ | Recontextualization during exhale, insight-oriented therapy | Change the gain vector before commit |
| $L^*_{somatic}$ | Movement (any), posture variation, standing desk | Restore routing distribution; raise diaphragm range |

**The protocol:**

1. Measure baseline $L^*$ profile (30 days)
2. Identify the highest component
3. Target that component with appropriate intervention
4. Re-measure after 30 days
5. Repeat until $L^*$ is in the low range

### 7c. Diagnostics

$L^*$ can be used diagnostically:

| $L^*$ Range | Diagnostic Interpretation | Clinical Action |
|---|---|---|
| 0.0 - 0.2 | Full recovery | Maintain |
| 0.2 - 0.4 | Compensated load | Monitor |
| 0.4 - 0.6 | Decompensated load | Intervene |
| 0.6 - 0.8 | Severe debt | Intervene aggressively |
| 0.8 - 1.0 | Critical debt | Emergency intervention |

---

## 8. Why Time of Day Is a Feature, Not Noise

### 8a. The Trajectory Is the Signal

A measurement taken at 8am and a measurement taken at 4pm on the same participant will produce different numbers. This is not measurement error. It is the trajectory being measured.

Debt accumulates across the day through session load — sustained cognitive effort, postural bracing, incomplete exhale cycles, glycemic events, social regulatory demand. A participant who is in Zone 1 at 8am may be in Zone 2 by 4pm. A participant who is in Zone 2 at 8am may reach Zone 3 by early afternoon.

Single-reading study designs that do not control for time of day are sampling randomly distributed positions on the trajectory and averaging them. The variance is the signal. Averaging it produces noise.

### 8b. The Evidence the Field Already Has

The field already has the data proving this. Vitale et al. (2019) conducted a comprehensive review demonstrating that HRV follows a circadian rhythm with significant chronotype-specific patterns. Evening-types show greater autonomic perturbation than morning-types. Li et al. (2024) found that sleep deprivation produces more pronounced HRV variations in evening-types.

But the strongest evidence comes from the wearable market itself. Every major HRV platform — Oura, WHOOP, Garmin, Apple, Polar — has built its entire analytic infrastructure around the fact that HRV varies across the day and across days. The apps show users their nightly HRV trends, their daily recovery scores, their strain-to-recovery ratios. The platforms exist because HRV data is useful precisely because it varies. If HRV were stable, the wearables would have nothing to report.

The field calls this variance "noise." The wearable market calls it "readiness," "recovery," and "strain." Same data. Different interpretation. The market has operationalized what the field has discarded.

Schumann et al. (2026) measured HRV at two timepoints separated by eight weeks, both taken at similar times of day. Their design was well-suited to detecting training effects, and it did. But the secondary finding — modest coupling between autonomic change and interoceptive change — is precisely what the framework predicts when load state is uncontrolled across participants. The variance in load state across participants attenuates any coupling that is load-dependent. If they had also measured participants at 8am and 4pm on the same day, they would have found the trajectory that Oura users see every morning. The signal was not absent. It was averaged away by unmeasured load variance.

### 8c. The Correct Design

The correct design registers the trajectory itself:

- Reading 1: morning baseline
- Reading 2: mid-session
- Reading 3: end of session
- Reading 4: following morning baseline

The slope of the delta HRV response across these readings is the debt accumulation rate — the most informative allostatic load metric available, because it captures both current position and trajectory direction simultaneously.

A system whose morning baseline is stable across consecutive days is recovering fully overnight. A system whose morning baseline drifts downward is accumulating faster than it recovers. These are categorically different allostatic states that any single reading conflates.

---

## 9. Falsifiable Predictions

**The central prediction of this framework is P-AL-011: the variance of daily HRV measurements predicts allostatic load outcomes better than any single reading. The remaining predictions are supporting and mechanistic. If P-AL-011 fails, the framework's core claim fails, regardless of the other predictions.**

#### 9a. P-AL-011 — The Central Prediction: HRV Dispersion Is the Signal, Not Noise

The variance of daily HRV measurements over 30 days will predict allostatic load outcomes (cognitive performance, inflammatory markers, self-reported stress) better than any single HRV reading. This is the direct test of the framework's central claim: the field has been treating the trajectory as noise.

| Field | Content |
|---|---|
| **IV** | HRV dispersion (variance across 30 days) vs. mean HRV |
| **DV** | Allostatic load outcomes (cognitive performance, inflammatory markers, self-reported stress) |
| **Operationalization** | 30-day wearable tracking with weekly outcome assessments. Compare predictive power of variance vs. mean using pre-registered model comparison. |
| **Confirmed if** | Dispersion predicts outcomes better than mean |
| **Disconfirmed if** | Mean HRV predicts outcomes better than dispersion, or neither predicts |
| **Status** | Partially supported — Okawara et al. (2024) |

**Why this is central:** If the variance is noise, the framework has no measurement target. If the variance is signal, the framework's entire measurement architecture is grounded. This single prediction separates the framework from the null-result literature it critiques.

### 9b. Supporting Predictions

#### P-AL-001 — Delta HRV Predicts Inflammatory Markers with Lag

Delta HRV response will predict CRP and IL-6 levels with a lag of 7-14 days. Low delta HRV precedes inflammatory marker rise. High delta HRV precedes inflammatory marker decline.

| Field | Content |
|---|---|
| **IV** | $\Delta HRV$ response |
| **DV** | CRP, IL-6 |
| **Operationalization** | Prospective within-subject study with daily HRV measurement and weekly inflammatory biomarker sampling. |
| **Confirmed if** | Delta HRV leads inflammatory marker changes by 7–14 days |
| **Disconfirmed if** | Delta HRV and inflammatory markers are simultaneous or delta HRV lags |
| **Status** | Untested |

#### P-AL-002 — CO₂ Tolerance Predicts Resting HRV Independently

CO₂ tolerance threshold will predict resting HRV independently of aerobic fitness level. Two participants matched for VO₂max will show different resting HRV if their Control Pause values differ significantly.

| Field | Content |
|---|---|
| **IV** | Control Pause |
| **DV** | Resting HRV |
| **Control** | VO₂max |
| **Operationalization** | Fitness-controlled cohort study with capnometry and HRV measurement. |
| **Falsification** | If CO₂ tolerance does not predict HRV after controlling for fitness, the mechanism is confounded. |
| **Status** | Untested |

#### P-AL-003 — Session Load Tracks Intraday Delta HRV

Morning versus afternoon delta HRV will track with independently measured cumulative session load. Participants with higher cognitive and social demand across the day will show greater delta HRV compression by afternoon than matched low-demand participants.

| Field | Content |
|---|---|
| **IV** | Session load (diary, experience sampling) |
| **DV** | Intraday delta HRV compression |
| **Operationalization** | Experience sampling design with session load diary and repeated HRV measurement. |
| **Status** | Untested |

#### P-AL-004 — ND Populations Show Compressed Tolerance

ND populations will show compressed CO₂ tolerance windows and faster intraday delta HRV decline at equivalent glycemic and cognitive load compared to NT controls.

| Field | Content |
|---|---|
| **IV** | Population (ND vs. NT) |
| **DV** | Control Pause, intraday delta HRV decline |
| **Operationalization** | Matched ND/NT cohort with continuous HRV monitoring and dietary logging. |
| **Status** | Untested |

#### P-AL-005 — ND Precision-Collapse Paradox

**P-AL-005a — Fasted precision spike:** ND populations will show higher cognitive performance scores (working memory, pattern recognition, or sustained attention) under fasted conditions (>12 hours) compared to matched NT controls under the same conditions. Operationalization: cognitive battery administered at 12h fast. Disconfirmation: ND performance equal to or below NT under fasted conditions.

**P-AL-005b — Interoceptive routing shift:** ND populations will show lower heartbeat detection accuracy (heartbeat counting task) during concurrent cognitive load compared to NT controls, and this reduction will be greater in ND populations than NT at equivalent load levels. Operationalization: heartbeat counting task with and without dual-task cognitive load. Disconfirmation: ND interoceptive accuracy drop ≤ NT drop under load.

**P-AL-005c — Abrupt collapse profile:** ND populations will show a lower coefficient of variation in performance across the trial — stable high performance followed by a single drop — while NT populations show a gradual decline. Operationalization: performance variability measured across 20-minute fasted cognitive task. Disconfirmation: ND variability profile indistinguishable from NT.

**P-AL-005d — Recovery signature:** ND populations will require longer recovery time (food + rest) before returning to pre-collapse performance than NT controls, consistent with debt clearance rather than simple glycaemic repletion. Operationalization: time-to-criterion post-collapse recovery with standardised meal. Disconfirmation: ND recovery time ≤ NT with glucose alone.

**P-AL-005e — Post-hoc hunger recognition:** ND populations will report hunger awareness post-collapse at higher rates than pre-collapse, while NT populations will show hunger awareness preceding cognitive decline. Operationalization: continuous hunger ratings on 0-10 VAS throughout task. Disconfirmation: ND hunger ratings rise before, not after, performance collapse.

**Combined confirmation:** Collapse predicted by HRV floor + hunger signal dropout preceding collapse event, not by blood glucose alone (blood glucose may remain in normal range at time of collapse). This is the critical distinction from simple hypoglycaemia framing.

#### P-AL-006 — Treatment Must Restore Delta HRV

Treatments that do not restore the delta HRV response are not restoring the system regardless of symptomatic improvement. Pharmaceutical interventions that suppress inflammatory biomarkers without improving vagal tone will show low delta HRV response despite normal CRP.

| Field | Content |
|---|---|
| **IV** | Treatment type (biomarker-suppressing vs. vagal-restoring) |
| **DV** | Delta HRV response pre/post treatment |
| **Operationalization** | Pre/post measurement of delta HRV in anti-inflammatory treatment cohorts. |
| **Status** | Untested |

#### P-AL-007 — Sleep Architecture Predicts Clearance Outcomes

Pre-sleep HRV will predict slow wave sleep proportion that night, which will predict glymphatic clearance outcome and next-day cognitive performance.

| Field | Content |
|---|---|
| **IV** | Pre-sleep HRV |
| **DV** | SWS proportion, next-day cognitive performance |
| **Operationalization** | Nighttime wearable tracking with morning cognitive assessment. |
| **Status** | Untested |

#### P-AL-008 — Composite Load Predicts Cognitive Capacity

The composite load equation $L^* = w_1 L^*_{HRV} + w_2 L^*_{RHR} + w_3 L^*_{temp} + w_4 L^*_{inflam} + w_5 L^*_{resp}$ will predict cognitive performance ($C_s$) better than any single component.

| Field | Content |
|---|---|
| **IV** | Composite $L^*$ vs. single components |
| **DV** | Cognitive performance (working memory, multi-hop reasoning, ambiguity tolerance) |
| **Operationalization** | Weights calibrated on a training cohort and frozen. Evaluation on a held-out validation cohort with weekly cognitive assessments over 30 days. |
| **Confirmed if** | Composite $L^*$ outperforms each individual component on the held-out set |
| **Disconfirmed if** | A single component predicts as well or better |
| **Status** | Untested |

**Note on calibration:** Weights are frozen after training and not adjusted during validation. Any post-hoc weight adjustment invalidates the prediction. This is what separates P-AL-008 from a curve-fitting exercise.

#### P-AL-009 — Load Profile Predicts Intervention Response

Different $L^*$ profiles will respond to different interventions: high $L^*_{HRV}$ will respond to HRV biofeedback; high $L^*_{inflam}$ will respond to anti-inflammatory protocols; high $L^*_{resp}$ will respond to breathing training.

| Field | Content |
|---|---|
| **IV** | Component load profile |
| **DV** | Intervention response (targeted vs. non-targeted) |
| **Operationalization** | Intervention trial with profile-matched assignment. |
| **Status** | Untested |

#### P-AL-010 — Glymphatic Clearance Load Amplifies Inflammation

Participants with reduced sleep SWS proportion and elevated sleep respiratory rate will show faster inflammatory marker accumulation over time, mediated by the glymphatic clearance failure → neuroinflammation loop.

| Field | Content |
|---|---|
| **IV** | SWS proportion, sleep respiratory rate |
| **DV** | Inflammatory marker accumulation rate |
| **Operationalization** | 6-month longitudinal tracking with wearable sleep staging and periodic inflammation panels. |
| **Status** | Untested |

#### P-AL-012 — Delta HRV Tracks Loop Activation $\Lambda$

The delta HRV response to the standardized slow-breath protocol is the operationalization of the loop activation indicator $\Lambda$ defined in Central Reference §2.2. A system with low accumulated debt shows significant HRV rise under the protocol ($\Delta HRV > 15$ ms) — the loop can open. A system at load ceiling shows minimal response ($\Delta HRV < 5$ ms) regardless of resting baseline — the loop cannot open.

| Field | Content |
|---|---|
| **IV** | Zone state (measured by composite $L^*$) |
| **DV** | $\Delta HRV$ response to standardized slow-breath protocol |
| **Operationalization** | Measure $\Delta HRV$ across Zone 1, 2, 3 participants. Test whether delta response is a valid proxy for $\Lambda$. |
| **Confirmed if** | Delta response differentiates zones with high sensitivity; is stable within individual across repeated sessions |
| **Disconfirmed if** | Delta response is uncorrelated with zone or is dominated by baseline HRV |
| **Status** | Untested — this is PREDICT-GATE-01 in Central Reference §16 |

#### P-AL-013 — Xue et al. Paradigm in ND Populations

The Xue et al. (2026) feature interference paradigm, run in ND populations, will show larger interference metrics ($IM$) at equivalent task uncertainty compared to NT controls. This reflects the higher baseline load and compressed CO₂ tolerance window in ND populations.

| Field | Content |
|---|---|
| **IV** | ND vs. NT status |
| **DV** | Interference metric $IM$, dimensionality drop |
| **Control** | Task uncertainty level |
| **Operationalization** | Run Xue et al. paradigm with ND and NT cohorts matched for age and education. Compare $IM$ trajectories. |
| **Falsification** | If ND and NT show equivalent $IM$ at equivalent uncertainty, P-AL-013 is disconfirmed. |
| **Status** | Untested |

#### P-AL-014 — Salience-Triggered Loop Access Is CO₂-Dependent

Individuals in Zone 2 (compressed but not collapsed CO₂ tolerance) will show measurable cognitive improvement after a salience trigger that forces a breath interruption, while individuals in Zone 1 (wide CO₂ tolerance) will show no difference. The improvement in Zone 2 will correlate with the size of the CO₂ rise the trigger produces.

| Field | Content |
|---|---|
| **IV** | Zone (1 vs. 2) and trigger condition (with vs. without) |
| **DV** | Performance on novel error-detection tasks |
| **Mediator** | CO₂ rise magnitude (capnometry) |
| **Operationalization** | Measure baseline CO₂ tolerance. Present novel tasks with and without preceding salience trigger. Measure performance difference and CO₂ rise. |
| **Falsification** | If Zone 2 does not show improvement after trigger, or if improvement does not correlate with CO₂ rise, P-AL-014 is disconfirmed. |
| **Status** | Untested |

#### P-AL-015 — Re-Fire Rate Predicts Load

The interrupt re-fire rate (ERP by region) will predict next-morning HRV baseline and next-day cognitive performance better than the total interrupt count.

| Field | Content |
|---|---|
| **IV** | Re-fire rate vs. total interrupt count |
| **DV** | Next-morning HRV baseline, next-day cognitive performance |
| **Operationalization** | Daytime ERP + overnight EMG + morning HRV |
| **Confirmed if** | Re-fire rate predicts better than total count |
| **Disconfirmed if** | Total count predicts as well or better |
| **Status** | Untested |

#### P-AL-016 — Movement Breaks Perseveration Load

Movement across the homunculus will reduce $L^*_{perseveration}$ by reducing the re-fire rate.

| Field | Content |
|---|---|
| **IV** | Movement vs. rest during perseveration |
| **DV** | $L^*_{perseveration}$ (re-fire rate, EMG by region) |
| **Operationalization** | Within-subject protocol with movement manipulation |
| **Confirmed if** | Movement reduces re-fire rate and EMG |
| **Disconfirmed if** | Movement does not reduce re-fire rate |
| **Status** | Untested |

#### P-AL-017 — Failed Release Attempts Predict Load

The number of failed release attempts (release attempts that re-fire) will predict next-morning HRV baseline and next-day cognitive performance better than the total release attempts.

| Field | Content |
|---|---|
| **IV** | Failed release attempts vs. total release attempts |
| **DV** | Next-morning HRV baseline, next-day cognitive performance |
| **Operationalization** | Daytime release-attempt log + morning HRV |
| **Confirmed if** | Failed release attempts predict better than total attempts |
| **Disconfirmed if** | Total attempts predict as well or better |
| **Status** | Untested |

#### P-AL-018 — Capacity Training Reduces Release-Triggered Load

Capacity training (breath range, CO₂ tolerance, Λ_lock training) will reduce $L^*_{release-triggered}$ by increasing the capacity to hold the surfaced PE without locking.

| Field | Content |
|---|---|
| **IV** | Capacity training vs. control |
| **DV** | $L^*_{release-triggered}$ (failed release rate, EMG by region) |
| **Operationalization** | Longitudinal within-subject protocol |
| **Confirmed if** | Capacity training reduces failed release rate |
| **Disconfirmed if** | Capacity training does not reduce failed release rate |
| **Status** | Untested |

#### P-AL-019 — Recontextualization Reduces Load

Recontextualization during the exhale will reduce $L^*_{encoding}$ by reducing the re-encoding gain of the surfaced PE.

| Field | Content |
|---|---|
| **IV** | Recontextualization during exhale vs. no recontextualization |
| **DV** | $L^*_{encoding}$ (EMG, re-fire rate, next-morning HRV) |
| **Operationalization** | Within-subject protocol with recontextualization manipulation |
| **Confirmed if** | Recontextualization reduces EMG and re-fire rate |
| **Disconfirmed if** | Recontextualization does not reduce EMG or re-fire |
| **Status** | Untested |

#### P-AL-020 — Insight Reduces Load

Insight experiences (sudden resolution with recontextualization) will reduce $L^*_{encoding}$ more than non-insight releases.

| Field | Content |
|---|---|
| **IV** | Insight vs. non-insight release |
| **DV** | $L^*_{encoding}$ (EMG, re-fire rate, next-morning HRV) |
| **Operationalization** | Within-subject protocol with insight identification |
| **Confirmed if** | Insight reduces load more than non-insight |
| **Disconfirmed if** | Insight does not reduce load more |
| **Status** | Untested |

### 9c. Confounds and Limitations

The delta HRV proxy is a composite signal. Several confounds must be acknowledged:

**Age:** Resting HRV declines with age through progressive autonomic remodelling. The within-person baseline method corrects for this partially — the individual's own trajectory is the reference — but age-related floor compression may reduce the dynamic range available for load detection in older populations.

**Baroreflex sensitivity:** Baroreflex gain modulates HRV independently of allostatic load. Individuals with inherently lower baroreflex gain will show compressed delta HRV responses at equivalent load levels. The framework's predictions about delta HRV decline hold within individuals across time, not across individuals with different baroreflex baselines.

**Medications:** Beta-blockers, antihypertensives, and stimulant medications directly alter HRV. Any study applying this framework must control for or stratify by medication status. The delta HRV response in a medicated individual reflects the combined effect of load and pharmacological autonomic modulation.

**Respiratory mechanics:** Breathing rate, tidal volume, and respiratory training status confound the relationship between HRV and load. The slow-breath protocol partially controls for this by standardising the respiratory input, but individuals with significantly different resting respiratory patterns require standardised protocol conditions to produce comparable delta HRV values.

**Fitness level:** Aerobic fitness independently elevates resting HRV and may confound the HRV baseline drift component. P-AL-002 tests whether CO₂ tolerance predicts HRV independently of fitness — this is the key disconfirmation criterion for the fitness confound hypothesis.

These confounds do not invalidate the framework. They specify the conditions under which the predictions hold most cleanly and identify the stratification variables required for confirmation studies.

---

## 10. Clinical Implications

### 10a. The Measurement Is Already Historical

The conventional allostatic load battery requires a clinical visit, blood draw, and processing time. By the time results are returned the system has moved position on the trajectory. The measurement is already historical.

The delta HRV protocol described here is:
- **Continuous** — measurable daily with a consumer wearable
- **Real-time** — reflects current system position, not a historical snapshot
- **Mechanistically grounded** — derived from the same causal chain that produces the inflammatory markers it predicts
- **Sensitive to trajectory direction** — not just position but rate of debt accumulation

### 10b. What Treatments Must Do

The clinical implication is direct. Treatments should be evaluated not by whether they suppress downstream biomarkers but by whether they restore delta HRV response capacity. A treatment that reduces CRP without restoring the vagal brake has suppressed a symptom of the contract failure without repairing the contract. Relapse is structurally guaranteed when treatment is withdrawn.

Interventions that restore delta HRV — slow breathing training, CO₂ tolerance conditioning, HRV biofeedback, dietary glycemic reduction — repair the contract. Interventions that do not are managing outputs of a system whose debt trajectory remains unchanged.

### 10c. The Gate-Lowering Failure Mode

As $L^*$ rises, $P_{threshold} = P_0 - \gamma L^*$ drops. The gate remains open but admits lower-quality signal. The decision-maker appears functional. The output is Path B dressed as Path A. This is the most dangerous failure mode — it is undetectable from behaviour alone (Central Reference §3.7 Note 2).

The clinical scenario this describes: patients with "normal biomarkers but subjective dysfunction" are in gate-lowering collapse. Their composite $L^*$ may be sub-threshold even while a single component (typically $L^*_{HRV}$ or $L^*_{inflam}$) is at critical load. Component REQT (Central Reference §3.7 Note 4) detects this. Composite REQT alone does not.

This is why the diagnostic $L^*_{diagnostic} = \max_i L^*_i$ matters. It is not a redundant calculation — it is the clinical readout that captures the failure mode where composite looks acceptable but the system is compromised.

### 10d. The Framework Already Exists

The wearable measurement of allostatic load is not a future technology. The protocol exists now. The mechanistic grounding exists in established contracts. The falsifiable predictions are testable with standard equipment.

What has been missing is the formal framework connecting them. That framework is this paper.

---

## 11. Summary of the Complete Measurement Architecture

### 11a. What the Framework Integrates

The complete allostatic load measurement framework integrates:

1. **Four regulatory contracts** (MET↔AUTO, IMMUNE↔AUTO, MET↔IMMUNE, AUTO↔MOD) as the mechanism chain
2. **Glymphatic clearance** (GLYMPH↔AUTO) as the recovery mechanism
3. **Salience accumulation** (SALIENCE↔AL) as the primary load source
4. **Perseveration load** ($L^*_{perseveration}$) as a load component
5. **Release-triggered load** ($L^*_{release-triggered}$) as a load component
6. **Encoding load** ($L^*_{encoding}$) as a load component
7. **Somatic load** ($L^*_{somatic}$) as a load component
8. **Precision geometry** ($P = R/D_T$) as the formal quantification of system capacity
9. **Effective precision** ($P_{eff} = P \cdot O_{pathway} \cdot U_C$) as the gate condition
10. **Two-factor pressure** (mechanical beneficial, cognitive harmful) as the load accumulation driver
11. **Seven measurement components** (HRV baseline, delta HRV, CO₂ tolerance, exhale completeness, sleep architecture, sleep RHR, inflammatory biomarkers)
12. **Composite load equation** with ten weighted components and individual baselines
13. **Three debt trajectory zones** (recovery, accumulating, ceiling)
14. **Individual load profiles** for treatment targeting
15. **Twenty falsifiable predictions** for clinical validation, with P-AL-011 (HRV dispersion is the signal) as the central prediction

### 11b. The Core Insight

**The core insight remains unchanged:** Allostatic load is cumulative regulatory debt — the portion of total demand that persists across recovery windows and is visible in standard physiological markers. The measurement framework makes it quantifiable. The predictions make it testable. The clinical applications make it actionable. **The salience mechanism is the upstream source of much of the load.** Each unresolved precision-lock is a unit of debt. Each re-fire is a unit of debt. Each failed release is a unit of debt. Each failed encoding is a unit of debt. Each static posture is a unit of debt. The AL paper measures the debt. The Salience paper explains where it comes from. The composition is the mechanism.

**The field already has the data. The Oura ring already shows the pattern. The only missing piece is the framework that makes the data readable.**

**HRV is a time‑dependent oscillatory signal driven by breathing. Any measurement design that ignores time will suppress the very mechanism it claims to investigate.**

**All of it is load. All of it is debt. All of it is persistent demand. And the measurement framework gives you the tools to quantify it.**

---

## References

Almeida, D. M., Piazza, J. R., Stawski, R. S., & Klein, L. C. (2011). The speedometer of life: Stress, health, and aging. In K. W. Schaie & S. L. Willis (Eds.), *Handbook of the psychology of aging* (7th ed., pp. 191–206). Academic Press. https://doi.org/10.1016/B978-0-12-380882-0.00012-7

Grunewald, T. L., Dillon, D. J., & Herrera, V. M. (2012). Sleep deprivation and inflammation: A systematic review. *Brain, Behavior, and Immunity*, *26*(8), 1205–1216. https://doi.org/10.1016/j.bbi.2012.06.004

Hall, M., Vasko, R., Buysse, D., Ombao, H., Chen, Q., Cashmere, J. D., Kupfer, D., & Thayer, J. F. (2004). Acute stress affects heart rate variability and inflammation. *Psychosomatic Medicine*, *66*(3), 409–415. https://doi.org/10.1097/01.psy.0000127415.32922.1b

Janicki-Deverts, D., Cohen, S., & Doyle, W. J. (2012). Sleep disturbance predicts IL-6 elevation. *Brain, Behavior, and Immunity*, *26*(6), 959–965. https://doi.org/10.1016/j.bbi.2012.05.005

Li, Y., Wang, X., Zhang, L., & Liu, Y. (2024). Effects of sleep deprivation on heart rate variability in different chronotypes. *Sleep Medicine*, *114*, 85–92. https://doi.org/10.1016/j.sleep.2024.01.015

Mathewson, K. J., Jetha, M. K., Drmic, I. E., Bryson, S. E., Goldberg, J. O., & Schmidt, L. A. (2016). High baseline respiratory sinus arrhythmia predicts more pronounced task-induced declines in respiratory sinus arrhythmia in children with autism spectrum disorder. *Psychophysiology*, *53*(10), 1541–1552. https://doi.org/10.1111/psyp.12696

Moreira, T. S., Takakura, A. C., Colombari, E., & Guyenet, P. G. (2006). Central chemoreceptors and sympathetic vasomotor outflow. *The Journal of Physiology*, *577*(1), 369–386. https://doi.org/10.1113/jphysiol.2006.119107

Okawara, H., Shiraishi, Y., Sato, K., Nakamura, M., & Katsumata, Y. (2024). Visually assessing work performance using a smartwatch via day-to-day fluctuations in heart rate variability. *Digital Health*, *10*, 20552076241239240. https://doi.org/10.1177/20552076241239240

Reed, A. E., Sayre-Carstairs, R., & Lindberg, M. (2020). Suppressing emotion depletes cognitive resources even when heart rate variability is stable. *Collabra: Psychology*, *6*(1), 28. https://doi.org/10.1525/collabra.273

Robinson, J. (2026a). *The Manifold Schema: A Unified Framework for Consciousness, Cognition, and Collapse* (v7.2). Zenodo. https://doi.org/10.5281/zenodo.21939439

Robinson, J. (2026b). *Physics as the Missing Component in Medical Science*. Zenodo. https://doi.org/10.5281/zenodo.21512678

Robinson, J. (2026c). *Precision, Timing, and the Oscillatory Source: Complete Formalism* (v3.4). Zenodo. https://doi.org/10.5281/zenodo.22179675

Robinson, J. (2026d). *The Geometry of Inference* (v1.0). Manifold Schema Technical Report Series.

Robinson, J. (2026e). *Central Reference: A Unified System Specification for the Loop Framework* (v1.4). Manifold Schema Technical Report Series.

Robinson, J. (2026f). *The Loop Is the Intelligence* (v1.0). Manifold Schema Technical Report Series.

Robinson, J. (2026g). *The Salience Interrupt: Routing, the Closed Loop, the Control Plane, and the Encoding Window* (v1.3). Manifold Schema Technical Report Series.

Robinson, J. (2026h). *Central Reference: A Unified System Specification for the Loop Framework* (v1.8.3). Manifold Schema Technical Report Series.

Sakakibara, M., Takeuchi, S., & Hayano, J. (1994). Effect of relaxation training on cardiac parasympathetic tone. *Psychophysiology*, *31*(3), 223–228. https://doi.org/10.1111/j.1469-8986.1994.tb02210.x

Schumann, A., Schmitt, L., Rieger, K., Caliskan, E., De la Cruz, F., Geisler, M., Gupta, Y., & Bar, K.-J. (2026). Physiological correlates of interoception and the effect of heart rate variability biofeedback. *Frontiers in Network Physiology*, *6*, 1846014. https://doi.org/10.3389/fnetp.2026.1846014

Segerstrom, S. C., & Miller, G. E. (2004). Psychological stress and the human immune system: A meta-analytic study of 30 years of inquiry. *Psychological Bulletin*, *130*(4), 601–630. https://doi.org/10.1037/0033-2909.130.4.601

Thayer, J. F., Yamamoto, S. S., & Brosschot, J. F. (2010). The relationship of autonomic imbalance, heart rate variability and cardiovascular disease risk factors. *International Journal of Cardiology*, *141*(2), 122–131. https://doi.org/10.1016/j.ijcard.2009.09.543

Tracey, K. J. (2002). The inflammatory reflex. *Nature*, *420*(6917), 853–859. https://doi.org/10.1038/nature01321

Trumpff, C., Acosta, C., & Picard, M. (2025). Daily axillary temperature ΔT and cognitive–autonomic patterns in free-living adults: Machine learning phenotyping of autonomic stress using the MiSBIE Brief-6. *medRxiv*. https://doi.org/10.1101/2025.01.15.25320654

Vitale, J. A., Weydahl, A., & Roveda, E. (2019). Chronotype and heart rate variability: A review. *Chronobiology International*, *36*(9), 1173–1182. https://doi.org/10.1080/07420528.2019.1626418

Yamamoto, S., Kitamura, Y., Yamada, N., Nakagawa, Y., & Kuroda, S. (2006). Meditative state correlates with interhemispheric EEG coherence and high-frequency heart rate variability. *International Journal of Psychophysiology*, *61*(2), 198–205. https://doi.org/10.1016/j.ijpsycho.2005.10.012

Zhang, X., Kvamme, T., Nagai, Y., & Silvanto, J. (2026). Cardio-respiratory coordination during memory encoding predicts performance. *bioRxiv*. https://doi.org/10.64898/2026.01.14.699577

Zhang, S., Niu, X., Ma, J., Wei, X., Zhang, J., & Du, W. (2025). Effects of sleep deprivation on heart rate variability: A systematic review and meta-analysis. *Frontiers in Neurology*, *16*, 1523456. https://doi.org/10.3389/fneur.2025.1523456

Iliff, J. J., Wang, M., Liao, Y., Plogg, B. A., Peng, W., Gundersen, G. A., & Nedergaard, M. (2012). A paravascular pathway facilitates CSF flow through the brain parenchyma and the clearance of interstitial solutes, including amyloid β. *Science Translational Medicine*, *4*(147), 147ra111. https://doi.org/10.1126/scitranslmed.3003748

*Contract references: contract_AUTO_MOD, contract_IMMUNE_AUTO, contract_MET_AUTO, contract_MET_IMMUNE — Unified Regulatory Model, publicly available at https://github.com/jtrthehax/Unified-Model/tree/main/01_PHYSICS_SUBSTRATE_CORE*

---

*Allostatic Load as Accumulated Regulatory Debt: A Comprehensive Measurement Framework*
*Robinson, J. (2026)*
*Manifold Schema Technical Report Series*
*Version: 2.2*
*Suggested citation: Robinson, J. (2026). Allostatic Load as Accumulated Regulatory Debt: A Comprehensive Measurement Framework with Delta HRV, CO₂ Tolerance, Sleep Architecture, Glymphatic Clearance, Salience Inheritance, and Composite Load Quantification. Manifold Schema Technical Report Series.*

---

## Version History

| Version | Date           | Changes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ------- | -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **2.2** | **2026-10-14** | **Integrated with Salience Interrupt v1.3 and Central Reference v1.8.3. Inherits salience accumulation, perseveration, release-triggered, encoding, and somatic load from Salience v1.3. Adds §2g–§2j (four new mechanism sections). Adds five new load components ($L^*_{perseveration}$, $L^*_{release-triggered}$, $L^*_{encoding}$, $L^*_{somatic}$, and explicit $L^*_{salience}$). Adds P-AL-015 through P-AL-020. Revised load profile table (nine profiles). Revised treatment targeting (ten targets). Updated composite load equation (ten components). Added Schumann origin paragraph to §1a. Added measurement burden note and tier table to §6c.**                                                                                                                                                                                                                                                                                        |
| **2.1** | **2026-09-13** | **Integrated with Central Reference v1.4. Versioning and cross-reference updates only: header updated; note added on $O_{pathway}$ and motor gain variables not being absorbed (gate-condition and motor-substrate variables, documented in Central Reference §2.8/§2.11 and GoI v1.0); stack list added *The Loop Is the Intelligence* v1.0 and version numbers for Precision v3.4, GoI v1.0, MS v7.2; inline Central Reference cross-references stripped of version numbers; note added pinning all cross-references to v1.4; references updated (Robinson 2026e → Central Reference v1.4, Robinson 2026f added for Loop v1.0); §2d precision integration updated with $P_{eff} = P \cdot O_{pathway} \cdot U_C$; §6c added $L^*_{critical,i}$ calibration note; §9b added P-AL-012 (delta HRV tracks $\Lambda$, cross-reference to PREDICT-GATE-01); §11a updated to include $P_{eff}$ and the substrate/uniformity split; changelog added at top.** |
| 2.0     | 2026-09-12     | Integrated with Central Reference v1.3. All residual fixes from integration memo applied: Control Pause thresholds reconciled (Zone 3 <15, severe <10); delta HRV ∝ 1/L* labeled as heuristic with cross-reference to §2d; weight calibration procedure replaced with held-out validation; 30-day baseline window flagged as provisional; wearable-market epistemic framing cleaned; P-AL-011 elevated to Central Prediction; RHR thresholds reconciled; L*_inflam unit-free normalization note added. Cross-references to Central Reference v1.3 added.                                                                                                                                                                                                                                                                                                                                                                                                |
| 1.8     | 2026-09-02     | Applied Gemini/Claude critique: formula fixes, composite vs diagnostic clarification, Okawara citation year corrected, Schumann framing softened, field-blindness reframed as reinterpretation, wearable evidence framed as access not validation, circadian vs pathological debt distinction, confounds section added, P-AL-005 broken into 5a-5e, self-citation note strengthened                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| 1.7     | 2026-09-01     | Added core statement to abstract, Section 1b, Section 11b; restructured section numbering; integrated wearable market data                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 1.6     | 2026-09-01     | Added wearable-market contradiction section; expanded Section 8 with wearable market evidence                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| 1.5     | 2026-09-01     | Added ND Precision-Collapse Paradox; expanded predictions to 11; integrated Vitale, Okawara, Li, MiSBIE references                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| 1.4     | 2026-08-30     | Added individual load profiles, treatment targeting, nine falsifiable predictions                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| 1.3     | 2026-08-30     | Added complete composite load equation with five components and individual baselines                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| 1.2     | 2026-08-30     | Added glymphatic clearance architecture with accumulation-inflammation loop                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| 1.1     | 2026-08-30     | Added precision-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
