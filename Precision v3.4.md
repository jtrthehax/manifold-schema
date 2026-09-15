# Precision, Timing, and the Oscillatory Source: Complete Formalism

## Integrating CO₂ Tolerance, Chemoreflex Jitter, Two-Factor Pressure, Cross-Frequency Coupling, and Operational Measurement Anchors

**Robinson, 2026**

*Technical Report — Manifold Schema Series*

**Version:** 3.4
**Date:** 2026-09-13
**Status:** Converged with Central Reference v1.4 — $P$ vs $P_{eff}$ distinction formalized, $O_{pathway}$ registered, header updated
**Framework:** Manifold Schema v7.2 (DOI: 10.5281/zenodo.21939440)
**Biological implementation:** The Geometry of Inference v1.0 (Robinson, 2026c)
**Complete specification:** Central Reference v1.4 (Robinson, 2026d)

---

## Changelog — v3.3 → v3.4

This changelog exists so that any reader — human or AI — can see the convergence path. Precision v3.3 was written to converge with Central Reference v1.3. The v1.3 → v1.4 delta added $O_{pathway}$ (§2.8), $L^*_{critical,i}$ (§2.9), and the motor gain variables (§2.11). Precision v3.3 already uses $L^*_{critical,i}$ (§1.12) and already has the motor gain variables (Part III). The three v3.4 changes are:

| Step | Change | Location | Reason | Central Reference anchor |
|---|---|---|---|---|
| 1 | Header updated to "Converged with Central Reference v1.4" | Header | Version drift | — |
| 2 | $P$ distinguished from $P_{eff}$ — $U_C$ removed from $P$ equation | §1.1, §2.3 | Central Reference v1.4 §3.6 and GoI v1.0 §3.0/§3.3 use $P_{eff} = P \cdot O_{pathway} \cdot U_C$. Precision v3.3 §2.3 folded $U_C$ into $P$. Align to majority form. | §3.6 |
| 3 | $O_{pathway}$ registered in mapping table with functional-form caveat | §1.10 | Central Reference v1.4 §2.8 declares $O_{pathway} = f(\Phi_{PV}, \Delta CBF/\Delta CMRO_2, CVR_{max})$ with form unspecified. Precision v3.3 did not register it. | §2.8 |
| 4 | $P$ as timing-coherence ratio clarified — $P_{eff}$ is the gate-condition variable | §1.1 | Notation consistency with Central Reference v1.4 | §3.6 |
| 5 | Changelog added at top | This section | Versioning track | — |
| 6 | Version history updated | Version History | — | — |

**What did not change:** The mechanisms. The precision equation, the CO₂ tolerance window, the two-factor pressure, the chemoreflex jitter, the collapse hysteresis, the resonance breathing, the cross-frequency coupling, the motor gain formalization, the temporal dynamics, the encoding window — every mechanism is unchanged from v3.3. Only the $P$ / $P_{eff}$ composition changed, and only to align with the Central Reference v1.4 form.

---

## Overview

Precision is the ratio of sync duration to timing distance between oscillatory streams: $P = R/D_T$. This paper formalizes that ratio and demonstrates that breath mechanics are its primary driver through a mechanistically grounded causal chain, each link of which is anchored in existing literature.

Nasal respiration directly entrains limbic oscillations in a phase-specific manner (Zelano et al., 2016). CO₂ — the primary output of respiratory mechanics — drives cerebral vasodilation and oxygen delivery (Raichle & Plum, 1972), with hypocapnia producing measurable cognitive and anxiety collapse through the same mechanism reversed (Meuret & Ritz, 2010). Slow breathing at resonance frequency produces simultaneous HRV increase and alpha/theta EEG coherence (Zaccaro et al., 2018), reflecting phase-locking between respiratory and cardiac oscillators that reduces timing distance $D_T$ and extends sync duration $R$. The result is a rise in $P$ that predicts cognitive performance (Pratap et al., 2026; Yamamoto et al., 2006).

The parameters of this chain — CO₂ tolerance window $C_{low}$ to $C_{high}(L^*)$, chemoreflex jitter threshold, resonance frequency — are individually determined, not population-constant. The Control Pause operationalizes $C_{high}$ as an individually measured and trainable variable (Cooper et al., 2003), and breathing training demonstrably shifts autonomic parameters from population baseline (Kox et al., 2014). Demanding standardized parameter values for this framework is equivalent to demanding that trained and untrained individuals show identical physiological responses to identical protocols. The existing literature already shows they do not.

The framework introduces two pressure components with opposite effects: mechanical pressure (breath-hold, resonance breathing) reduces $D_T$ and extends $R$; cognitive/metabolic pressure increases $D_T$ and compresses $R$. Above $C_{high}(L^*)$, chemoreflex activation injects quadratic jitter $J(C) = \kappa(C - C_{high}(L^*))^2$, collapsing $P$. Recovery after collapse is delayed by hysteresis. Ten falsifiable predictions are provided, each testable with standard capnometry, HRV, and EEG equipment.

The Phase Locking Value (PLV) is an operational approximation of the $P = R/D_T$ construct. The relationship is empirical rather than algebraic — future work should test whether $P$ predicts outcomes that PLV alone does not.

**Convergence note:** This paper is the precision measurement layer of the unified framework specified in Central Reference v1.4. The CO₂ tolerance window, the two-factor pressure decomposition, and the chemoreflex jitter mechanism are the operationalization of the precision variable $R^*$ in the master equation. Cross-references to the Central Reference appear throughout.

**Note on $P$ vs $P_{eff}$:** The variable $P$ in this paper is the raw timing-coherence ratio $P = R/D_T$. The gate condition in Central Reference §3.6 and GoI v1.0 §3.0 uses the effective precision:

$$P_{eff} = P \cdot O_{pathway} \cdot U_C$$

$P_{eff}$ applies the substrate constraint $O_{pathway}$ and the uniformity multiplier $U_C$ to $P$. $R^*$ in the master equation is normalized $P$ — not $P_{eff}$. See §1.1 and §1.10 for the full distinction.

---

## Part I: The Core Definition

### 1.1 Precision as a Timing-Coherence Ratio

Let two oscillatory streams have phase difference:

$$\Delta \phi(t)$$

Define **timing distance** as the average absolute phase difference over a measurement window:

$$D_T = \mathbb{E}_{t \in T} \big[|\Delta \phi(t)|\big]$$

Define **sync duration** as the proportion of time spent within a small phase band $\epsilon$:

$$R = \frac{T_{\text{in}}}{T_{\text{total}}}$$

Where $T_{\text{in}}$ is the time the phase difference remains below threshold $\epsilon$.

**Precision is the ratio of sync duration to timing distance:**

$$P = \frac{R}{D_T}$$

**Interpretation:** A system achieves high precision when two streams stay close together (low $D_T$) and stay close for long periods (high $R$). A system with low precision may have streams that are close briefly (low $D_T$, low $R$) or far apart consistently (high $D_T$, high $R$). Both produce low $P$.

**Normalized form.** The master equation in Central Reference §3.1 uses the normalized precision $R^*$, defined as:

$$R^* = \frac{P}{P_{baseline}} = \frac{R/D_T}{(R/D_T)_{baseline}}$$

$R^*$ is an intra-individual metric — it measures precision relative to the individual's own baseline, not relative to a population norm. When $P$ is high, $R^* > 1$; when $P$ is at baseline, $R^* = 1$; when $P$ is degraded, $R^* < 1$. All equations in the Central Reference master equation use $R^*$; the equations in this paper use $P$ where the absolute value matters and $R^*$ where the normalized value matters.

**Note on $P$ vs $P_{eff}$.** $P$ is the raw timing-coherence ratio — the ratio of sync duration to timing distance. It does not include the substrate constraint $O_{pathway}$ (oxygen pathway integrity) or the uniformity multiplier $U_C$ (CO₂ uniformity). The gate condition — the condition under which the loop can open — uses the effective precision:

$$P_{eff} = P \cdot O_{pathway} \cdot U_C$$

$P_{eff}$ is the precision that actually reaches the outer edge of the manifold, given that (a) the substrate pathway can carry the signal and (b) the CO₂ distribution is uniform enough to sustain phase coherence. The raw $P$ is what the timing-coherence measurement produces. The $P_{eff}$ is what the gate opens on. $R^*$ in the master equation is normalized $P$ — not $P_{eff}$, because the master equation measures bandwidth, not gate opening.

**Operational Measurement:** The Phase Locking Value (PLV) is the operational measurement of $P$. PLV ranges from 0 (no synchronization) to 1 (perfect synchronization), calculated as:

$$\text{PLV} = \left|\frac{1}{N}\sum_{n=1}^{N} \exp(i \times (\phi_{\text{resp}}(n) - \phi_{\text{hr}}(n)))\right|$$

PLV is an operational measure of phase-locking coherence — how consistently two oscillatory streams maintain phase proximity. We propose that $P = R/D_T$ is the formal theoretical construct that PLV approximates operationally. The relationship between $P$ and PLV is empirical rather than algebraic: PLV captures phase consistency through a different mathematical operation but reflects the same underlying phenomenon — sync duration and timing distance between oscillatory streams. Future work should test whether $P$ predicts outcomes that PLV alone does not (Pratap et al., 2026).

**Operational measurement of $P_{eff}$:** $P_{eff}$ requires three measurements: $P$ (via PLV or equivalent), $O_{pathway}$ (via the functional components $\Phi_{PV}, \Delta CBF/\Delta CMRO_2, CVR_{max}$ — functional form unspecified pending calibration per Central Reference §2.8), and $U_C$ (via capnometry multi-site variance). In practice, $P$ and $U_C$ are measurable with standard equipment; $O_{pathway}$ requires calibrated fMRI or equivalent, and its functional form is an open empirical question. This paper's equations use $P$ throughout, with $U_C$ applied where the composition matters (see §2.3). When the gate condition is being evaluated, $P_{eff}$ is the relevant variable — see Central Reference §3.6.

---

### 1.2 Cross-Frequency Coupling (CFC)

Timing distance $D_T$ and sync duration $R$ may be computed within a single frequency band or across multiple bands (cross-frequency coupling). CFC allows the precision ratio to capture interactions such as:

- Respiration–HRV coupling (0.1 Hz)
- Alpha–theta coupling during meditation
- Theta–HRV coupling during breath-hold
- Gamma–cardiac phase coupling during flow states

This makes the precision model compatible with multi-band EEG and HRV phenomena and explains why precision can be experienced across different cognitive and physiological states.

**Operational Measurement of Cross-Frequency Coupling:** CFC is measured using phase-amplitude coupling (PAC), phase-phase coupling (PPC), or n:m phase locking between oscillatory bands.

**Cross-reference:** Central Reference §2.1 defines $\Theta^*$ (integration efficiency) as the cross-frequency coupling component of the master equation. The CFC precision measurements specified here are the empirical operationalization of $\Theta^*$.

---

### 1.3 Individual Variability in CO₂ Tolerance

The CO₂ tolerance parameters $C_{\text{low}}$ and $C_{\text{high}}$ are individual-specific and trainable. Factors that shift the tolerance window include:

| Factor | Effect on Tolerance |
|---|---|
| Fitness/athletic training | Increases tolerance (higher $C_{\text{high}}$) |
| Anxiety | Decreases tolerance (lower $C_{\text{high}}$) |
| Altitude | Shifts tolerance (adaptation over days) |
| Hydration | Affects tolerance (dehydration lowers) |
| Sleep | Affects tolerance (poor sleep lowers) |
| Breathwork practice | Increases tolerance (trainable) |

The Control Pause (CP) — the duration of comfortable breath hold after a normal exhale before the first urge to breathe — is the clinical operationalization of $C_{high}$ as an individual parameter. Cooper et al. (2003) used CP as the primary individual measurement metric in a randomized controlled trial of Buteyko breathing for asthma, demonstrating both that CP varies substantially across individuals and that it shifts measurably with breathing training. A person with CP of 10 seconds has a narrow tolerance window — chemoreflex activates at minimal CO₂ rise. A person with CP of 40 seconds has a wide window — the system tolerates higher CO₂ before jitter threshold is reached. Same mechanism. Different parameters.

The frequency-dependence of slow breathing effects — demonstrated across multiple protocols in Zaccaro et al. (2018) — confirms that optimal breathing rate is individually determined. Prescribing a fixed breathing rate without individual calibration is physiologically equivalent to prescribing a fixed weight for a strength training program without measuring the individual's capacity. The substrate is universal. The parameters are not.

The trainability of breathing parameters is not theoretical. Kox et al. (2014) demonstrated in a controlled study that practitioners trained in the Wim Hof breathing method showed significantly different autonomic and immune responses to an endotoxin challenge compared to untrained controls following identical protocols. The mechanism was identical across groups. The parameters had shifted through training.

**Load-compressed tolerance.** The CO₂ tolerance window is not fixed. As allostatic load accumulates, the ceiling drops:

$$C_{high}(L^*) = C_{high}^0 - \gamma L^*$$

where $C_{high}^0$ is baseline tolerance and $\gamma$ is the load-compression coefficient. This means the same absolute CO₂ level produces chemoreflex jitter at lower values when load is high. The compression mechanism is what the Control Pause measures clinically: as load rises, CP drops. A person with CP of 40 seconds at baseline may show CP of 25 seconds after a period of accumulated debt. The mechanism is identical. The parameter has shifted.

**Cross-reference:** Central Reference §2.3 formalizes this. The load decomposition $L^*$ is specified in Central Reference §2.10 and operationalized in Allostatic Load v2.1 §6.

---

### 1.4 The CO₂ Tolerance Window

CO₂ tolerance defines the upper bound of the precision window. Precision increases only while CO₂ remains within the individual tolerance band:

$$C_{\text{low}} < C < C_{\text{high}}(L^*)$$

Where:
- $C_{\text{low}}$ is the minimum CO₂ needed to raise HRV, reduce jitter, and allow precision to rise
- $C_{\text{high}}(L^*)$ is the maximum CO₂ the system can sustain before chemoreflex activation injects jitter, given current allostatic load

**Above $C_{\text{high}}(L^*)$, chemoreflex activation produces involuntary diaphragm and intercostal spasms that inject timing noise into the oscillatory loop.** This jitter is modeled as:

$$J(C) = \begin{cases}
0 & C \le C_{\text{high}}(L^*) \\
\kappa (C - C_{\text{high}}(L^*))^2 & C > C_{\text{high}}(L^*)
\end{cases}$$

Where $\kappa$ is the chemoreflex jitter gain. Jitter grows quadratically once tolerance is exceeded.

**Note on load dependence.** $C_{high}$ is load-dependent: $C_{high}(L^*) = C_{high}^0 - \gamma L^*$. When load is high, the ceiling drops. The window compresses. Jitter onset occurs at lower CO₂. This is the mechanism by which allostatic load degrades precision even when breathing mechanics are unchanged.

The cognitive consequence of operating below $C_{low}$ is documented in established physiology. Raichle & Plum (1972) demonstrated that hyperventilation — chronic low CO₂ — produces direct cerebral vasoconstriction, reducing cerebral blood flow despite normal arterial oxygen saturation. The brain receives less oxygen not because blood oxygen is low but because CO₂-driven vasodilation is absent. This is the physiological mechanism of brain fog: reduced oxygen delivery to neural tissue from hypocapnia, not hypoxia. Raising CO₂ toward $C_{peak}$ restores vasodilation, restores oxygen delivery, and restores precision.

**Operational Measurement of Jitter:** Jitter is approximated using EEG phase jitter, HRV beat-to-beat variability (RMSSD), and respiration–ECG phase slip.

**Interpretation:** This matches the phenomenology — CO₂ initially increases precision, but excessive CO₂ triggers spasms that add jitter and break coherence. The system flips from coherence to jitter because of chemoreflex-induced spasms.

---

### 1.4a Cognitive and Anxiety Signatures of Hypocapnia

Operating chronically below $C_{low}$ produces measurable cognitive and anxiety consequences through the cerebral blood flow mechanism identified by Raichle & Plum (1972). Meuret & Ritz (2010) demonstrated that panic disorder is characterized by measurably low CO₂ levels during attacks and that interventions raising CO₂ reduce panic symptoms. The cognitive narrowing, anxiety, and perceptual distortion of panic are not primarily psychological events — they are the precision collapse signature of a system operating below $C_{low}$ with insufficient CO₂ to maintain oscillatory coherence.

This connects the precision framework to anxiety, panic, and cognitive impairment through a single shared mechanism: hypocapnia reduces cerebral blood flow, reduces oxygen delivery, raises jitter $J(C)$ through chemoreflex instability at the lower bound, and collapses $P$. The subjective experience differs across individuals — some report fog, some report anxiety, some report perceptual narrowing — but the underlying mechanism is identical. Individual $C_{low}$ determines the threshold at which these symptoms emerge.

---

### 1.4b The Salience-Triggered Loop Access

Baseline CO₂ tolerance determines whether the loop is available at rest or only under salience-induced breath interruption.

**The mechanism.** Salience halts breathing → CO₂ rises → cerebral blood flow increases → jitter drops → $P$ rises → $K$ drops → $W^*$ widens → orthogonality restored → $\Theta^*$ rises → loop becomes available.

**The individual difference.**

| Profile | Breath pattern | Baseline CO₂ | Baseline $P$ | Loop access |
|---|---|---|---|---|
| Chronic hypocapnic | Rapid, shallow, chest | Low | Low | Requires salience trigger |
| Stable CO₂ | Slow, diaphragmatic | Within window | High | Available at baseline |

**The prediction.** Baseline CO₂ tolerance predicts whether an individual requires salience-induced breath interruption to enter deep inference. See PREDICT-PREC-10.

**The clinical implication.** CO₂ tolerance training raises baseline $P$, lowering the salience threshold required to access the loop. This is a trainable substrate parameter, not a fixed trait.

**Connection to the framework.** The loop (Path A) is expensive. Path B (prior retrieval) is always available and always cheaper. The system defaults to Path B under load unless precision is high enough to open the gate. For chronic hypocapnic individuals, precision is rarely high enough at baseline — the gate stays closed until a salience event forces a breath interruption that temporarily restores CO₂. For stable-CO₂ individuals, the gate is available at baseline. This is not a difference in intelligence — it is a difference in substrate parameters.

**Cross-reference:** Central Reference §5 specifies the Path A/B branch condition. Central Reference §6 specifies the four qualification profiles.

---

### 1.5 The Two-Factor Pressure Variable

Pressure must be split into two components with opposite effects:

| Component | Symbol | Source | Effect on Precision |
|-----------|--------|--------|---------------------|
| **Mechanical pressure** | $\Pi_{\text{mech}}$ | Breath-hold, closed-loop pressure, thoracic pressure, baroreflex coherence | **Beneficial** — reduces timing distance, extends sync duration |
| **Cognitive/metabolic pressure** | $\Pi_{\text{cog}}$ | Load, sympathetic activation, cognitive demand, allostatic load | **Harmful** — increases timing distance, reduces sync duration |

**Total pressure is the sum:**

$$\Pi = \Pi_{\text{mech}} + \Pi_{\text{cog}}$$

But they operate with opposite signs in the precision equations.

**Mechanical Pressure Onset Condition:** Mechanical pressure becomes beneficial when the respiratory loop is closed (end-exhalation breath-hold) and thoracic motion drops below threshold. This condition enforces bilateral symmetry and reduces timing drift.

**Operational Measurement of Pressure Components:** Mechanical pressure is approximated using thoracic pressure amplitude (respiration belt), baroreflex phase coherence (ECG–BP coupling), and intracranial pulse pressure proxies (PPG). Cognitive/metabolic pressure is approximated using sympathetic markers (LF/HF ratio), pupillometry (task-evoked dilation), and performance-capacity mismatch (error rate under load).

**Interpretation:** This resolves the paradox in the original framework. Breath-hold pressure (mechanical) improves precision by enforcing bilateral symmetry and phase coherence. Cognitive load pressure (metabolic) degrades precision by injecting noise and increasing jitter. The same word — "pressure" — carries opposite meanings depending on its source.

**Note on $\Pi_{cog}$ vs. $L^*$:** These are distinct. $\Pi_{cog}$ is *instantaneous* cognitive pressure — the current draw on the budget. $L^*$ is *cumulative* allostatic load — the integral of $\Pi_{cog}$ over time minus recovery:

$$L^*(t) = \int_0^t \Pi_{cog}(\tau) \, d\tau - \text{recovery}(t)$$

Both appear in the framework. $\Pi_{cog}$ enters the precision equation directly (through $D_T$ and $R$). $L^*$ enters the master equation as the denominator drag, and now also compresses $C_{high}(L^*)$. This prevents double-counting: acute load affects precision; chronic load affects bandwidth and the CO₂ ceiling.

**Cross-reference:** Central Reference §2.3 formalizes this distinction. The load decomposition is specified in Central Reference §2.10.

---

### 1.6 CO₂ Uniformity and Dynamics

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

**Operational Measurement of CO₂ Uniformity:** CO₂ uniformity is approximated using end-tidal CO₂ (capnometry), multi-site PPG variance, and respiration–HRV coupling stability.

**Cross-reference:** Central Reference §3.3 specifies the full precision equations including $U_C(L^*)$.

---

### 1.7 Collapse Hysteresis

After precision collapse, recovery is delayed due to residual jitter and sympathetic activation. This is modeled as:

$$P_{\text{recover}} = P(t) - \delta_{\text{hyst}}$$

Where $\delta_{\text{hyst}}$ is the hysteresis penalty. This explains post-collapse fog and delayed clarity.

**Hysteresis Decay:** The hysteresis penalty decays exponentially:

$$\frac{d\delta_{\text{hyst}}}{dt} = -\sigma \delta_{\text{hyst}}$$

**Interpretation:** The system does not recover from collapse at the same rate it entered it. Once jitter is injected and coherence is lost, residual sympathetic activation and lingering phase noise prevent immediate return to precision lock. Recovery requires sustained conditions — not just a brief return to the precision window.

---

### 1.8 Resonance Breathing

Resonance breathing occurs when the respiratory oscillator and the cardiac baroreflex oscillator phase-lock at ~0.1 Hz (≈6 breaths/min). This is not a theoretical prediction — it is a systematically reviewed empirical finding.

Zaccaro et al. (2018) conducted a systematic review of slow breathing protocols and found that breathing at ~6 breaths/min consistently produces increased HRV (HF power), increased alpha and theta EEG activity, and increased baroreflex sensitivity simultaneously. The autonomic and central nervous system effects co-occur because they share the same mechanism: the respiratory and cardiac oscillators are phase-locking, reducing timing distance $D_T$ and extending sync duration $R$ across both systems at once.

Critically, Zaccaro et al. found these effects are frequency-dependent — the optimal breathing rate is not universal. Different individuals show peak HRV and EEG coherence responses at slightly different rates within the ~0.1 Hz band. This frequency-dependence is direct evidence that the parameters of the precision window are individually determined, not population-constant. The mechanism is universal. The individual expression of it is not.

Formally:

$$\Pi_{\text{mech}} \propto \text{PLV}(f_{\text{resp}}, f_{\text{baro}})$$

When $f_{\text{resp}} = f_{\text{baro}}$, drift drops, jitter remains low, and precision rises without entering the CO₂ tolerance window. This produces stable clarity and flow without spasms or collapse.

**Operational Measurement of Resonance:** Resonance is measured as phase-locking between respiration and baroreflex at ~0.1 Hz, using respiration belts and ECG–BP coupling.

**Interpretation:** Resonance breathing is a third precision mechanism — distinct from CO₂-driven precision and breath-hold precision lock. It operates through frequency entrainment of the respiratory and cardiac oscillators, producing sustained precision at moderate CO₂ levels without the risk of exceeding tolerance.

---

### 1.9 The Streams Being Measured

The "two oscillatory streams" in this definition correspond to specific measurable phenomena. The respiratory oscillator is not merely correlated with neural oscillation — it directly entrains it.

Zelano et al. (2016) demonstrated that nasal breathing entrains oscillations in piriform cortex, hippocampus, and amygdala in a phase-specific manner: memory recall was significantly better during inhalation than exhalation, fear discrimination was faster during inhalation, and both effects disappeared entirely during mouth breathing. The respiratory rhythm was setting the neural oscillatory phase directly. Removing nasal airflow removed the entrainment and the cognitive effect simultaneously.

This is the $P = R/D_T$ mechanism observed in vivo. The breath sets the phase. Neural streams synchronize to it. When synchronization is high — sync duration $R$ is long, timing distance $D_T$ is small — cognitive performance improves. The Zelano findings are not a correlation between breathing and cognition. They are a direct observation of oscillatory coupling producing measurable cognitive outcome, with a natural experimental control that isolates the mechanism.

| Stream | Neural Correlate | Measurement |
|--------|------------------|-------------|
| Left hemisphere oscillation | Language-dominant network | EEG phase, MEG |
| Right hemisphere oscillation | Contextual/competitive network | EEG phase, MEG |
| Cardiac oscillation | Heart rate rhythm | ECG/HRV |
| Respiratory oscillation | Breath rhythm | Respiration belt |

Precision can be measured between any pair of these streams. The most relevant for the framework is the **inter-hemispheric phase coherence** ($C_{LR}$ in *The Geometry of Inference*), which determines whether the gate opens.

**Operational Measurement of Timing Distance:** Timing distance $D_T$ is operationalized as EEG phase difference variance between oscillatory streams (PLV jitter).

**Literature Support:** During Zen meditation, researchers observed increases in slow alpha interhemispheric EEG coherence in the frontal region alongside increases in high-frequency (HF) power (parasympathetic index of HRV). Trait anxiety was negatively correlated with the percent change in slow alpha interhemispheric coherence — lower anxiety → greater increase in bilateral coherence → higher precision (Yamamoto et al., 2006).

---

### 1.10 Relationship to Existing Variables

| This Framework | Manifold Schema | Central Reference | Geometry of Inference |
|---|---|---|---|
| Timing distance $D_T$ | Phase coherence deficit | — | $\Delta \phi$ |
| Sync duration $R$ | Phase-locking stability | — | $C_{LR}$ coherence duration |
| Precision $P$ | $R^*$ (normalized form) | $R^* = P/P_{baseline}$ | $P$ (raw); gate uses $P_{eff}$ |
| Effective precision $P_{eff}$ | — | $P_{eff} = P \cdot O_{pathway} \cdot U_C$ | Gate condition (§3.3) |
| Oxygen pathway integrity $O_{pathway}$ | — | $f(\Phi_{PV}, \Delta CBF/\Delta CMRO_2, CVR_{max})$ — form unspecified | Floor condition (§3.0) |
| $P$ at encoding | $\mathcal{U}$ write quality | $W_{enc} \leftrightarrow \mathcal{U}$ | Prior update success |
| Jitter $J(C)$ | contributes to $\eta$ | $\eta_{effective} = \eta_{baseline} + J(C)$ | contributes to $\eta$ |
| Mechanical pressure $\Pi_{mech}$ | Breath coherence | — | Symmetry enforcer |
| Cognitive pressure $\Pi_{cog}$ | Load | $L^*$ (cumulative) | $L^*$ (allostatic load) |
| Resonance breathing | $A_s^*$ stability | — | $C_{LR}$ maintenance |
| Collapse hysteresis $\delta_{hyst}$ | Recovery cost | $\delta_{hyst}$ | $\delta_{hyst}$ |
| CFC (multi-band) | $\Theta^*$ integration | — | Cross-frequency coupling |
| — | — | $C_{high}(L^*)$ | — |
| — | — | REQT | — |
| — | — | Collapse sequence | — |

**Note on $P$ vs $P_{eff}$.** This paper defines $P$ as the raw timing-coherence ratio $P = R/D_T$. The gate condition in Central Reference §3.6 and GoI v1.0 §3.0 uses $P_{eff} = P \cdot O_{pathway} \cdot U_C$ — the precision that actually reaches the outer edge given the substrate and uniformity constraints. $R^*$ in the master equation is normalized $P$. The distinction matters because a system can have high $P$ while having low $P_{eff}$ — for example, high phase coherence between two streams (high $P$) combined with poor substrate perfusion (low $O_{pathway}$) produces low effective precision, and the gate stays closed despite the coherence. Conversely, a system with moderate $P$ and excellent $O_{pathway}$ and $U_C$ can open the gate when a system with higher $P$ cannot. $P_{eff}$ is the gate variable; $P$ is the timing-coherence variable.

**Note on $O_{pathway}$.** The precision framework does not itself constrain the substrate pathway that carries the signal. $O_{pathway}$ is the substrate constraint — oxygen pathway integrity — that determines whether the precision computed here can actually reach the outer edge. The functional form is declared in Central Reference §2.8 as $f(\Phi_{PV}, \Delta CBF/\Delta CMRO_2, CVR_{max})$ with the combination unspecified pending calibration. Precision v3.4 does not measure $O_{pathway}$ directly — it measures $P$ and $U_C$, which are two of the three factors in $P_{eff}$. The third factor ($O_{pathway}$) is a substrate constraint documented in the Central Reference and operationalized in the metabolic pathway papers.

**Note on $J(C)$.** Chemoreflex jitter $J(C)$ is not identical to amplitude jitter $\sigma(A_s)$. It is a *contributor* to the effective noise floor. When CO₂ exceeds $C_{high}(L^*)$, chemoreflex activation injects timing noise that raises the effective $\sigma(A_s)$ and the effective $\eta$:

$$\eta_{effective} = \eta_{baseline} + f(J(C))$$

The functional form of $f$ is assumed linear for simplicity: $\eta_{effective} = \eta_{baseline} + J(C)$. This is why jitter degrades signal detectability without changing the geometric structure of existing representations — the manifold's shape is unchanged, but what can be detected through it is reduced.

**Note on $R^*$.** Central Reference uses $R^* = P/P_{baseline}$ throughout the master equation. When this paper uses $P$, the absolute precision value is intended. When the master equation is being referenced, $R^*$ is the normalized form.

**Note on the master equation exponents.** The Cobb-Douglas exponents (0.15, 0.30, 0.25, 0.15) in Central Reference §3.1 are provisional. They reflect the empirical collapse sequence (precision degrades first, window second, amplitude and integration third) but have not been formally calibrated.

---

### 1.11 Independent Empirical Confirmation of $K$

Xue et al. (2026) demonstrated that under task uncertainty, the neural representations of task-relevant and task-irrelevant features become non-orthogonal in V1. Cross-decoding (p = 0.006, p = 0.036), noise correlation (p < 0.0001), and microstimulation (p = 0.009) all confirm the entanglement.

**This is the $K$ mechanism measured directly.** Under load, representations that were orthogonal become entangled — the manifold curves, and the effective dimensionality drops. The paper calls it "feature interference." The framework calls it "$K$ rising under load."

**Mapping:**

| Xue et al. | This Framework |
|---|---|
| Task uncertainty | $L^*$ (allostatic load) |
| Feature interference | $K$ (curvature) |
| Enhanced irrelevant encoding | $W^*$ narrowing |
| Non-orthogonal feature axes | $\Theta^*$ degradation |
| Dimensionality loss | $W^* \times \Theta^*$ collapse |
| Perceptual accuracy drop | $C_s$ reduction |

**Why this matters for the framework.** Xue et al. is an independent confirmation of the curvature mechanism from a completely different research program. It uses different vocabulary, different methods, and different anatomical targets (V1, not PFC). The convergence is the evidence: the same geometric mechanism appears whether you call it "feature interference" or "curvature."

**Cross-reference:** Central Reference anchor A28 specifies this connection.

---

### 1.12 REQT — The Qualification Threshold

Precision is necessary for the loop to run, but not sufficient. The system must also be qualified — the substrate must be in a state where the loop can be sustained. REQT is the condition under which Intelligence > 0 is sustained. When REQT ≤ 0, $\Lambda \to 0$ and the intelligence product collapses regardless of $n_{hops}$, $R^*$, or $\Theta^*$.

$$REQT = \left(\frac{A_s^*}{A_{s,0}^*} \cdot \frac{R^*}{R_0^*} \cdot \frac{W^*}{W_0^*} \cdot \frac{\Theta^*}{\Theta_0^*} \cdot \frac{I^*}{I_0^*}\right) - L^* > 0$$

**Note on weighting.** REQT uses equal weights as a conservative qualification default — any component falling significantly below baseline is treated as a disqualifier regardless of compensating strength in other components. The master equation uses unequal weights because they reflect the empirical collapse sequence (precision degrades first). REQT weights reflect minimum viable threshold — a different question.

**Requalification condition:**

$$REQT > 0 \quad \text{after} \quad L^* < L^*_{threshold} \quad \text{AND} \quad \Lambda > 0 \quad \text{for} \geq 48h$$

**The gate-lowering failure mode.** As $L^*$ rises, $P_{threshold} = P_0 - \gamma L^*$ drops. The gate remains open but admits lower-quality signal. The decision-maker appears functional. The output is Path B dressed as Path A. This is the most dangerous failure mode — it is undetectable from behaviour alone.

**Component REQT.** Composite REQT can be passed while a single component is at critical load:

$$REQT_{component} = REQT_{composite} \wedge (\max_i L^*_i < L^*_{critical,i})$$

A system passes REQT only if both total load is manageable AND no single component is at critical level.

**Connection to precision.** The precision framework determines the $R^*$ component of REQT. Low precision means the $R^*$ term is below baseline, which lowers the composite REQT score. The CO₂ tolerance window determines the ceiling on $R^*$. The load-compressed ceiling $C_{high}(L^*)$ determines how much precision is available at any given load.

**Cross-reference:** Central Reference §3.7 formalizes the full REQT equation. The load decomposition is specified in Central Reference §2.10.

---

### 1.13 The Collapse Sequence

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

**Connection to precision.** Stage 1 is precision collapse. The entire sequence begins with $P$ dropping. This is why the precision framework is the measurement layer for the collapse sequence. The CO₂ tolerance window determines when precision collapses. The load-compressed ceiling $C_{high}(L^*)$ determines how close the system is to that collapse at any given moment.

**Cross-reference:** Central Reference §5b specifies the full sequence with zone correspondence. Allostatic Load v2.1 §3b connects the zones to the stages.

---

### 1.14 The Four Profiles

The branch condition is determined by the interaction of PE sensitivity, PE tolerance, encoding curvature, and routing capacity. Four profiles are distinguishable:

| Profile | $\sigma_{PE}$ | $\tau_{PE}$ | $K_{enc}$ | $I^*$ | Qualification Status |
|---|---|---|---|---|---|
| **High-gain, high-tolerance** | High | High | Low | High | **Qualified** — detects PE, gate stays open, loop runs, prior updates |
| **High-gain, low-tolerance** | High | Low | Low | High | **Conditionally qualified** — detects PE but cascade fires |
| **Standard-gain, high $K_{enc}$** | Low | Any | High | Moderate | **Disqualified for novel domains** — doesn't detect PE, or suppresses it |
| **Low $I^*$ (any gain)** | Low | Low | Any | Low | **Disqualified** — ambiguity unresolvable regardless of gain or tolerance |

**The fourth profile is the most clinically important.** When $I^*$ collapses — through dissociation, chronic interoceptive avoidance, or interoceptive load — the system cannot resolve ambiguity regardless of its gain or tolerance. Avoidance becomes the default behavior.

**Connection to precision.** The CO₂ tolerance window determines which profile a person can access. Low $C_{high}$ means the system is closer to jitter onset. High $C_{high}$ means the window is wide and the gate can stay open longer. Precision lock is the physiological signature of the qualified profile.

**Cross-reference:** Central Reference §6 specifies the full profile table. Allostatic Load v2.1 §7a describes the load profiles, which are orthogonal to the qualification profiles described here.

---

### 1.15 The Load Decomposition

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

**Connection to precision.** $L^*$ enters the precision framework through two pathways: (1) it compresses the CO₂ ceiling $C_{high}(L^*)$, and (2) it raises $P_{threshold}$ via $P_{threshold} = P_0 - \gamma L^*$. High load means a narrower CO₂ window and a higher gate threshold. The system must work harder to achieve the same precision.

**Cross-reference:** Central Reference §2.10 specifies the full decomposition. Allostatic Load v2.1 §6 specifies the measurement protocols.

---

### 1.16 Why Prior Studies Failed — Structural Account

The framework has a specific response to the null-result literature: prior studies measured the wrong variable with the wrong design.

Standard HRV allostatic load research takes a single reading, averages across participants, and tests for correlation with an outcome. This design structurally eliminates the variable it claims to measure:

- **Allostatic load is a trajectory, not a state.** A participant at 8am and the same participant at 4pm carry different accumulated debt. Averaging morning and afternoon readings produces a number that corresponds to neither state.
- **Variance is the signal.** Averaging across participants with different baseline debt levels produces a distribution whose variance obscures the effect.
- **Unmeasured load state attenuates coupling.** When load is uncontrolled across participants, any coupling between two physiological signals is attenuated by uncontrolled variance in load state.

This is not a critique of individual study designs — it is a structural account of why a specific design class produces null results. The framework predicts exactly the results observed: "modest coupling" between autonomic and interoceptive changes is exactly what the framework predicts when load state is uncontrolled. The effect was not absent. It was averaged away.

**The fix is trivial:** measure HRV at multiple times across the day, same participant, same protocol. Two readings. The wearable market has been doing this for a decade. The field was not looking for variance — it was looking for stability. It found noise because it was measuring the wrong thing with the wrong design.

**Connection to precision.** The precision framework's central prediction — that the CO₂ tolerance window determines precision peak — has been tested in studies that average across participants and across time. The window is individually determined. The peak is individually determined. Averaging produces a curve that fits no one. The null results are the expected output of the wrong design.

**Cross-reference:** Allostatic Load v2.1 §1a and §22b specify the full structural account for HRV measurement specifically.

---

## Part II: The Complete Dynamic Precision Model

**Note on Individual Parameters.** Every parameter in the dynamic model — $C_{low}$, $C_{high}$, $\Pi_{threshold}$, $\lambda_m$, $\lambda_c$, $\mu_m$, $\mu_c$, $\nu$, $\rho$, $\sigma$, $k_1$, $k_2$, $k_3$ — is an **individual transfer function**, not a population constant. These parameters are anchored by genetic substrate (dopamine clearance, HPA axis resilience, muscle fiber distribution) and modulated by training (breathwork, fitness, CO₂ tolerance conditioning). Two individuals under identical external conditions will follow distinct precision trajectories because their underlying parameter vectors differ. Empirical calibration requires individual system identification rather than population-level averaging. This is consistent with the Central Reference §2d calibration-constants note and Allostatic Load v2.1 §6a baseline method.

---

### 2.1 HRV as a Function of CO₂

Within the tolerance window, HRV increases with CO₂ via vagal activation:

$$H(C) = k_1 \cdot C \quad \text{for } C_{\text{low}} < C < C_{\text{high}}(L^*)$$

Above $C_{\text{high}}(L^*)$, HRV collapses as chemoreflex activation introduces sympathetic override:

$$H(C) = k_1 \cdot C_{\text{high}}(L^*) \cdot e^{-\nu (C - C_{\text{high}}(L^*))} \quad \text{for } C > C_{\text{high}}(L^*)$$

**Literature Support:** Voluntary apnea produces decreased theta waves at all cortical sites and increased LF/HF ratio, interpreted as hypercapnia causing depressed cortical activity (Sakakibara et al., 1994). Theta activities are significantly correlated with measures of parasympathetic activity (pNN50, HF) and negatively with sympathetic activity (LF/HF, LF) — the EEG-HRV link is confirmed.

---

### 2.2 The Two-Factor Pressure Equations

**Mechanical pressure** (breath-hold, closed-loop, resonance breathing) reduces timing distance and extends sync duration:

**Timing distance reduction:** Mechanical pressure enforces bilateral symmetry, reducing phase drift:

$$D_T \propto \frac{1}{1 - \lambda_m \Pi_{\text{mech}}}$$

**Sync duration extension:** Mechanical pressure stabilizes phase alignment:

$$R \propto 1 + \mu_m \Pi_{\text{mech}}$$

**Cognitive/metabolic pressure** (load, sympathetic activation) increases timing distance and reduces sync duration:

**Timing distance increase:** Cognitive pressure injects noise and disrupts phase alignment:

$$D_T \propto 1 + \lambda_c \Pi_{\text{cog}}$$

**Sync duration reduction:** Cognitive pressure disrupts sustained coherence:

$$R \propto e^{-\mu_c \Pi_{\text{cog}}}$$

**Resonance breathing contribution:** When respiratory and cardiac oscillators phase-lock:

$$\Pi_{\text{mech}} \propto \text{PLV}(f_{\text{resp}}, f_{\text{baro}})$$

---

### 2.3 The Complete Precision Equation with Two-Factor Pressure

**Timing distance with both pressure components and jitter:**

$$D_T = \frac{k_2}{H(C)} \cdot \frac{1 + \lambda_c \Pi_{\text{cog}}}{1 - \lambda_m \Pi_{\text{mech}}} + J(C)$$

**Sync duration with both pressure components and jitter:**

$$R = k_3 H(C) \cdot (1 + \mu_m \Pi_{\text{mech}}) \cdot e^{-\mu_c \Pi_{\text{cog}}} \cdot e^{-\nu J(C)}$$

**Raw precision:**

$$P = \frac{R}{D_T}$$

**Effective precision (gate condition):**

$$P_{eff} = P \cdot O_{pathway} \cdot U_C$$

**The full raw precision equation with two-factor pressure:**

$$P(C, \Pi_{\text{mech}}, \Pi_{\text{cog}}) = \frac{k_3}{k_2} \cdot H(C)^2 \cdot \frac{(1 + \mu_m \Pi_{\text{mech}}) \cdot e^{-\mu_c \Pi_{\text{cog}}} \cdot e^{-\nu J(C)}}{\frac{1 + \lambda_c \Pi_{\text{cog}}}{1 - \lambda_m \Pi_{\text{mech}}} + \frac{k_2}{H(C)} J(C)}$$

**Note on the change from v3.3.** In v3.3, the equation was written as $P = \frac{R}{D_T} \cdot U_C$ — the uniformity multiplier was folded into $P$. The v3.4 form keeps $U_C$ separate: $P$ is the raw timing-coherence ratio, and $P_{eff} = P \cdot O_{pathway} \cdot U_C$ is the gate-condition variable. This aligns with Central Reference §3.6 and GoI v1.0 §3.0/§3.3. The two forms are equivalent in the limit where $O_{pathway}$ and $U_C$ are equal to 1, but they differ when either constraint is not saturated — and the difference matters because a system with high $P$ but low $O_{pathway}$ will not open the gate (see §1.1 note).

**With hysteresis:**

$$P_{\text{recover}} = P(t) - \delta_{\text{hyst}} \quad \text{(post-collapse)}$$

**Interpretation:** Mechanical pressure (breath-hold, resonance) and cognitive pressure (load) have opposite signs. Mechanical pressure improves precision by reducing timing distance and extending sync duration. Cognitive load degrades precision by doing the opposite. The chemoreflex jitter term $J(C)$ operates independently on both, injecting noise when CO₂ exceeds tolerance. Hysteresis delays recovery after collapse.

**Load-dependent summary form:**

$$P(L^*) = \frac{R_0 e^{-\mu_c L^*}}{D_0 (1 + \lambda_c L^*)}$$

where $R_0$ is baseline sync duration and $D_0$ is baseline timing distance. This is a compact summary — the full equation above is the primary specification.

**Effective precision with load:**

$$P_{eff}(L^*) = P(L^*) \cdot O_{pathway}(L^*) \cdot U_C(L^*)$$

**Cross-reference:** Central Reference §3.3 specifies the full precision equations. Central Reference §3.6 specifies the gate condition using $P_{eff}$.

---

### 2.4 The CO₂ Tolerance Curve with Two-Factor Pressure

The precision-CO₂ relationship follows a specific curve, modulated by the balance of mechanical and cognitive pressure:

| CO₂ Level | HRV $H(C)$ | Jitter $J(C)$ | Mech Pressure | Cog Pressure | Precision $P$ | Phenomenology |
|-----------|------------|---------------|---------------|--------------|---------------|---------------|
| $C < C_{\text{low}}$ | Low | 0 | Low | Variable | Low | Poor coherence, fog |
| $C \approx C_{\text{low}}$ | Rising | 0 | Rising | Low | Rising | Improving clarity |
| $C \approx C_{\text{peak}}$ | Peak | 0 | Moderate | Low | Maximum | **Precision lock** — clarity, presence, flow |
| $C \approx C_{\text{high}}(L^*)$ | Peak | 0 → small | High | Rising | Declining | Fading clarity, effort |
| $C > C_{\text{high}}(L^*)$ | Collapsing | $\kappa(C - C_{\text{high}}(L^*))^2$ | Collapsing | High | Collapsing | Spasms, jitter, coherence loss |

**Precision lock is the peak of this curve.** It occurs when:
- CO₂ is high enough and uniform ($C \approx C_{\text{peak}}$)
- Mechanical pressure is sufficient to enforce symmetry ($\Pi_{\text{mech}} > \Pi_{\text{threshold}}$)
- Cognitive pressure is low ($\Pi_{\text{cog}} < \Pi_{\text{threshold}}$)
- CO₂ is below tolerance ($C < C_{\text{high}}(L^*)$)
- Substrate pathway is intact ($O_{pathway} > O_{min}$)

**Individual Variability:** The values of $C_{\text{peak}}$, $C_{\text{low}}$, and $C_{\text{high}}$ vary across individuals and are trainable through breathwork, fitness, and CO₂ tolerance conditioning. The ceiling $C_{\text{high}}$ also compresses with allostatic load: $C_{\text{high}}(L^*) = C_{\text{high}}^0 - \gamma L^*$.

---

## Part III: Motor Gain and the Limb with Gain

### 3.1 Formal Motor Gain Equation

Define **motor gain** $G_m$ as the amplification of motor intention:

$$G_m = \alpha P - \beta \eta$$

Where:
- $\alpha$ is the precision-to-gain conversion coefficient
- $P$ is precision (timing coherence)
- $\beta$ is the noise sensitivity coefficient
- $\eta$ is the neural noise floor

**Operational Measurement of Motor Gain:** Motor gain is approximated using EMG amplitude, movement overshoot, and tremor amplitude.

**Interpretation:** When precision is high, motor gain is high — intentions transmit cleanly and movements are amplified. When noise is high, motor gain is reduced — intentions are degraded.

### 3.2 Motor Gain → Movement Stability

Define **movement stability** as the inverse of movement drift:

$$\text{Stability} = \frac{1}{G_m \cdot \text{Drift}}$$

Where Drift is the variance in motor output relative to intention:

$$\text{Drift} = \text{Var}(X_{intended} - X_{actual})$$

**Interpretation:** High gain increases the impact of any drift, reducing stability. This is why "the limb requires control" — gain is high, so any drift is amplified.

### 3.3 Motor Gain → Collapse Risk

Define **collapse risk** as the probability of precision loss during movement:

$$C_{risk} = \frac{\gamma \cdot G_m}{1 + \text{Cache}}$$

Where Cache is the availability of cached movement patterns (from the motor encoding layer):

$$\text{Cache} = \frac{N_{cached}}{N_{total}}$$

**Interpretation:** When gain is high and cached patterns are limited, collapse risk increases. The system defaults to cached patterns because uncached patterns are risky.

### 3.4 The Complete Motor-Precision State

The motor system's state at any moment is:

$$M_{state} = \begin{cases}
\text{Stable} & \text{if } G_m < G_{threshold} \text{ and Cache} > \text{Cache}_{min} \\
\text{Unstable} & \text{if } G_m > G_{threshold} \text{ or Cache} < \text{Cache}_{min} \\
\text{Collapsed} & \text{if } C_{risk} > C_{threshold}
\end{cases}$$

**The limb with gain requiring control is the unstable state** — gain is high but control is sufficient to maintain stability. Collapse occurs when gain exceeds control capacity.

**Calibration note.** The thresholds $G_{threshold}$, $\text{Cache}_{min}$, and $C_{threshold}$ are individual calibration parameters, not population constants. Central Reference §2.11 and §22 (open question 15) specify this. No current prediction calibrates them directly.

---

## Part IV: Temporal Dynamics

### 4.1 Precision as a Function of Time

$$P(t) = \frac{k_3}{k_2} \cdot H(t)^2 \cdot \frac{(1 + \mu_m \Pi_{\text{mech}}(t)) \cdot e^{-\mu_c \Pi_{\text{cog}}(t)} \cdot e^{-\nu J(C(t))}}{\frac{1 + \lambda_c \Pi_{\text{cog}}(t)}{1 - \lambda_m \Pi_{\text{mech}}(t)} + \frac{k_2}{H(t)} J(C(t))}$$

**Effective precision as a function of time:**

$$P_{eff}(t) = P(t) \cdot O_{pathway}(t) \cdot U_C(t)$$

### 4.2 Rate of Precision Change

$$\frac{dP}{dt} = \frac{\partial P}{\partial H}\frac{dH}{dt} + \frac{\partial P}{\partial \Pi_{\text{mech}}}\frac{d\Pi_{\text{mech}}}{dt} + \frac{\partial P}{\partial \Pi_{\text{cog}}}\frac{d\Pi_{\text{cog}}}{dt} + \frac{\partial P}{\partial J}\frac{dJ}{dt}$$

### 4.3 Uniformity Dynamics

$$\frac{dU_C}{dt} = -\rho \cdot \text{Var}_i[C_i(t)]$$

### 4.4 Precision Lock Dynamics

Precision lock is a dynamic state characterized by:

$$\frac{dP}{dt} \approx 0 \quad \text{AND} \quad P_{eff}(t) > P_{threshold}$$

The duration of precision lock is:

$$T_{lock} = \int_{t_{onset}}^{t_{offset}} \mathbf{1}_{P_{eff}(t) > P_{threshold}} dt$$

### 4.5 Flow as Sustained Precision Lock

$$Flow(t) = P_{eff}(t) \quad \text{for } t \in T_{lock}$$

Flow maintenance requires:

$$\frac{dP}{dt} \approx 0 \quad \text{AND} \quad C_{\text{low}} < C(t) < C_{\text{high}}(L^*) \quad \text{AND} \quad \Pi_{\text{mech}}(t) > \Pi_{\text{threshold}} \quad \text{AND} \quad \Pi_{\text{cog}}(t) < \Pi_{\text{threshold}} \quad \text{AND} \quad O_{pathway}(t) > O_{min}$$

Flow collapse occurs when:

$$\frac{dP}{dt} < 0 \quad \text{OR} \quad C(t) > C_{\text{high}}(L^*) \quad \text{OR} \quad \Pi_{\text{mech}}(t) < \Pi_{\text{threshold}} \quad \text{OR} \quad \Pi_{\text{cog}}(t) > \Pi_{\text{threshold}} \quad \text{OR} \quad O_{pathway}(t) < O_{min}$$

### 4.6 Encoding Window Dynamics

The encoding window is:

$$W_{enc} = \int_{t_{enc}} \mathbf{1}_{P(t) > P_{threshold}} dt$$

**Interpretation.** Prior quality is determined by the duration and intensity of precision during encoding. A brief moment of high precision produces a high-quality prior. Sustained precision produces lasting prior updates.

**Connection to Central Reference §3.8.** The encoding window $W_{enc}$ is the temporal integral of precision during encoding. The prior update rate $\mathcal{U}$ is the instantaneous rate at each moment within that window:

$$\mathcal{U} = \frac{A_s^* \cdot R^* \cdot \Theta^*}{1 + \gamma K_{enc}}$$

The two are related: $\mathcal{U}$ is the rate, $W_{enc}$ is the interval over which the rate applies. The total prior update magnitude is approximately:

$$\text{Update} \approx \int_{t_{enc}} \mathcal{U}(t) \cdot \mathbf{1}_{P(t) > P_{threshold}} dt$$

High $W_{enc}$ with high $\mathcal{U}$ produces the strongest prior update. This is why the intervention sequence in Central Reference §3.8 specifies: change the geometry first (raise $P$, widen $W_{enc}$), then introduce the signal (run $\mathcal{U}$ at flat $K_{enc}$).

### 4.7 Collapse Hysteresis Dynamics

After precision collapse, recovery is delayed:

$$P_{\text{recover}}(t) = P(t) - \delta_{\text{hyst}} \quad \text{for } t > t_{\text{collapse}}$$

Where $\delta_{\text{hyst}}$ decays exponentially:

$$\frac{d\delta_{\text{hyst}}}{dt} = -\sigma \delta_{\text{hyst}}$$

**Interpretation:** The system does not recover immediately even when conditions return to the precision window. Residual jitter and sympathetic activation require time to clear. The hysteresis penalty captures the "sticky" nature of collapse recovery.

---

## Part V: The Complete Causal Chain (Dynamic Version)

```
Breath pattern
  ↓ [Zelano et al., 2016 — nasal respiration directly entrains limbic oscillations]
CO₂ level rises toward C_peak
  ↓ [Raichle & Plum, 1972 — CO₂ drives cerebral vasodilation and oxygen delivery]
Cerebral blood flow increases
  ↓ [Meuret & Ritz, 2010 — hypocapnia collapses this link; raising CO₂ restores it]
HRV rises, sympathetic tone drops
  ↓ [Zaccaro et al., 2018 — slow breathing at ~6 BPM produces HRV increase and alpha/theta EEG coherence simultaneously]
Respiratory and cardiac oscillators phase-lock
  ↓ [Yamamoto et al., 2006 — Zen meditation increases interhemispheric EEG coherence alongside HF HRV increase]
Timing distance D_T drops, sync duration R rises
  ↓ [Pratap et al., 2026 — cardiorespiratory coupling during encoding predicts cognitive performance]
P = R/D_T rises
  ↓
P_eff = P · O_pathway · U_C
  ↓
Cognitive performance improves

Individual C_high determines where this chain 
peaks and where chemoreflex jitter terminates it
  ↓ [Cooper et al., 2003 — Control Pause operationalizes C_high as individually measured and trainable]
  ↓ [Kox et al., 2014 — breathing training shifts autonomic parameters measurably from population baseline]

Load compresses C_high: C_high(L*) = C_high^0 - γL*
  ↓ [Central Reference §2.3]
Window narrows, jitter onset occurs at lower CO₂
  ↓
Precision ceiling drops even when breathing mechanics are unchanged
```

**The chain is now mathematically complete.** Every arrow is a mechanism. Every variable is defined. Every relationship is specified. The two-factor pressure variable resolves the conceptual contradiction. The load-compressed ceiling connects precision to the allostatic load framework. The $P$ vs $P_{eff}$ distinction connects the raw precision measurement to the gate condition.

---

## Part VI: The Conceptual Gaps — Closed

| Gap                          | Solution                                                                    | Formalism                                                                                                                                                                                                        |
| ---------------------------- | --------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Pressure–Timing**          | Two-factor pressure with opposite signs                                     | $D_T = \frac{k_2}{H} \cdot \frac{1 + \lambda_c \Pi_{\text{cog}}}{1 - \lambda_m \Pi_{\text{mech}}} + J(C)$; $R = k_3 H \cdot (1 + \mu_m \Pi_{\text{mech}}) \cdot e^{-\mu_c \Pi_{\text{cog}}} \cdot e^{-\nu J(C)}$ |
| **CO₂ Uniformity**           | Distributional CO₂ variable with chemoreflex jitter and uniformity dynamics | $U_C = \frac{1}{\text{Var}_i[C_i] + \epsilon}$; $J(C) = \kappa(C - C_{\text{high}}(L^*))^2$; $\frac{dU_C}{dt} = -\rho \cdot \text{Var}_i[C_i(t)]$                                                          |
| **Motor Gain**               | Formal gain equation with stability and collapse risk                       | $G_m = \alpha P - \beta \eta$; Stability $= \frac{1}{G_m \cdot \text{Drift}}$; $C_{risk} = \frac{\gamma \cdot G_m}{1 + \text{Cache}}$                                                                      |
| **Temporal Dynamics**        | Time derivatives for precision, flow, encoding, uniformity                  | $P(t)$; $\frac{dP}{dt}$; Precision lock as $\frac{dP}{dt} \approx 0$ AND $P_{eff} > P_{threshold}$; $\frac{dU_C}{dt}$                                                                                   |
| **Collapse Hysteresis**      | Recovery delay after collapse                                               | $P_{\text{recover}} = P(t) - \delta_{\text{hyst}}$; $\frac{d\delta_{\text{hyst}}}{dt} = -\sigma \delta_{\text{hyst}}$                                                                                         |
| **Resonance Breathing**      | Frequency entrainment precision mechanism                                   | $\Pi_{\text{mech}} \propto \text{PLV}(f_{\text{resp}}, f_{\text{baro}})$                                                                                                                                        |
| **Cross-Frequency Coupling** | Multi-band precision measurements                                           | $D_T$, $R$, $P$ computed across frequency bands                                                                                                                                                             |
| **Individual Variability**   | Trainable CO₂ tolerance parameters                                          | $C_{\text{low}}$, $C_{\text{high}}$ are individual-specific and trainable                                                                                                                                     |
| **Load-Compressed Ceiling**  | CO₂ window compresses with allostatic load                                  | $C_{\text{high}}(L^*) = C_{\text{high}}^0 - \gamma L^*$                                                                                                                                                         |
| **$\Pi_{cog}$ vs. $L^*$** | Instantaneous vs. cumulative distinction                                    | $L^*(t) = \int_0^t \Pi_{cog}(\tau) d\tau - \text{recovery}(t)$                                                                                                                                                  |
| **$P$ vs. $P_{eff}$**    | Raw precision vs. gate-condition form                                       | $P = R/D_T$; $P_{eff} = P \cdot O_{pathway} \cdot U_C$                                                                                                                                                        |

---

## Part VII: Falsifiable Predictions

### PREDICT-PREC-01 — CO₂ Tolerance Window Produces Precision Peak

> Precision $P(t)$ will follow the CO₂ tolerance curve: rising with CO₂ until $C_{\text{high}}(L^*)$, peaking at $C_{\text{peak}}$, then collapsing as jitter $J(C) = \kappa(C - C_{\text{high}}(L^*))^2$ increases. The peak precision will occur before $C_{\text{high}}(L^*)$ — not at maximum CO₂.

| Field | Content |
|-------|---------|
| Test | Continuous measurement of HRV, CO₂ (capnometry), EEG phase coherence during breath-hold protocol |
| Outcome if confirmed | Precision trajectory matches the CO₂ tolerance curve — peak at uniformity maximum, collapse at chemoreflex threshold |
| Outcome if disconfirmed | Precision continues to rise with CO₂ until hypercapnia collapse — the chemoreflex jitter mechanism is incorrect |
| Status | Untested — standard capnometry, HRV, and EEG equipment sufficient |

### PREDICT-PREC-02 — Mechanical and Cognitive Pressure Have Opposite Effects

> Mechanical pressure (breath-hold) will increase precision as $\frac{1}{1 - \lambda_m \Pi_{\text{mech}}}$, while cognitive pressure (load) will decrease precision as $(1 + \lambda_c \Pi_{\text{cog}})$. The same pressure source with different origins produces opposite effects.

| Field | Content |
|-------|---------|
| Test | Measure precision under (a) breath-hold (mechanical pressure) and (b) cognitive load (math task) with matched subjective effort. Compare $P$ across conditions. |
| Outcome if confirmed | Mechanical pressure increases precision; cognitive pressure decreases it — the two-factor model is confirmed |
| Outcome if disconfirmed | Both pressure sources decrease precision — the beneficial mechanical effect is not supported |
| Status | Untested — standard capnometry, HRV, EEG, and cognitive load equipment sufficient |

### PREDICT-PREC-03 — Jitter Tracks CO₂ Above Tolerance

> Jitter $J(t)$ will be zero below $C_{\text{high}}(L^*)$ and will grow as $\kappa(C - C_{\text{high}}(L^*))^2$ above $C_{\text{high}}(L^*)$, measured as increased phase jitter in EEG and increased variability in HRV.

| Field | Content |
|-------|---------|
| Test | Measure phase jitter (EEG) and HRV variability during breath-hold. Correlate with capnometry. |
| Outcome if confirmed | Jitter is chemoreflex-driven — the quadratic growth is confirmed |
| Outcome if disconfirmed | Jitter does not track CO₂ above tolerance — other mechanisms dominate |
| Status | Untested — standard capnometry, HRV, and EEG equipment sufficient |

### PREDICT-PREC-04 — Resonance Breathing Produces Stable Precision

> Resonance breathing (≈6 breaths/min) will produce stable precision $P(t)$ with low jitter $J(C)$ and low collapse risk, independent of CO₂ tolerance. The precision peak will be lower but more sustained than breath-hold.

| Field | Content |
|-------|---------|
| Test | Compare precision, jitter, and flow duration under resonance breathing vs. breath-hold. Measure EEG phase coherence, HRV, and self-reported flow. |
| Outcome if confirmed | Resonance breathing produces stable, sustainable precision without collapse risk |
| Outcome if disconfirmed | Resonance breathing does not produce measurable precision increase beyond normal breathing |
| Status | Untested — standard EEG, HRV, and capnometry equipment sufficient |

### PREDICT-PREC-05 — Collapse Hysteresis Delays Recovery

> After precision collapse, recovery will be delayed by $\delta_{\text{hyst}}$ which decays exponentially. Recovery time will be longer than the time spent in collapse, and the delay will correlate with residual sympathetic activation.

| Field | Content |
|-------|---------|
| Test | Induce precision collapse through hypercapnia or cognitive load. Measure precision recovery rate and correlate with HRV recovery and sympathetic markers. |
| Outcome if confirmed | Hysteresis is confirmed — recovery is slower than collapse |
| Outcome if disconfirmed | Recovery is symmetric — no hysteresis effect |
| Status | Untested — standard HRV, capnometry, and cognitive load equipment sufficient |

### PREDICT-PREC-06 — Precision Predicts Motor Gain

> Motor gain $G_m = \alpha P - \beta \eta$ will correlate with precision $P$ during movement tasks. Higher precision produces higher motor gain and higher movement stability until gain exceeds control capacity.

| Field | Content |
|-------|---------|
| Test | Measure EEG phase coherence (precision) and motor gain (EMG amplitude, movement amplification) during precision movement tasks |
| Outcome if confirmed | Precision predicts motor gain — the limb with gain requiring control is formalized |
| Outcome if disconfirmed | Motor gain is independent of precision — the motor-precision link is not supported |
| Status | Untested — standard EEG, EMG, and motion capture equipment sufficient |

### PREDICT-PREC-07 — Encoding Quality is Precision-Weighted Time

> Memory encoding quality correlates with $\int_{t_{enc}} P(t) dt$ — the integral of precision during encoding — independent of exposure time.

| Field | Content |
|-------|---------|
| Test | Measure precision $P(t)$ during memory encoding. Test recall at 1-day and 1-week follow-up. |
| Outcome if confirmed | The geometry at encoding is the active variable — precision-weighted time predicts memory quality |
| Outcome if disconfirmed | Exposure time alone predicts memory quality — precision does not add predictive value |
| Status | Untested — standard EEG, HRV, and memory task equipment sufficient |

### PREDICT-PREC-08 — Cross-Frequency Coupling Predicts Integration

> Precision measured across frequency bands (CFC) will predict $\Theta^*$ (integration efficiency) better than single-band precision. Flow states will show characteristic CFC profiles (alpha–theta, theta–HRV).

| Field | Content |
|-------|---------|
| Test | Measure multi-band EEG and HRV during flow-inducing tasks. Compute precision across band pairs. Correlate CFC precision with integration task performance. |
| Outcome if confirmed | CFC precision predicts integration — the multi-band model is confirmed |
| Outcome if disconfirmed | Single-band precision is sufficient — CFC does not add predictive value |
| Status | Untested — standard EEG and HRV equipment sufficient |

### PREDICT-PREC-09 — CO₂ Tolerance Is Trainable

> $C_{\text{low}}$ and $C_{\text{high}}$ will shift with breathwork training. $C_{\text{high}}$ will increase, $C_{\text{peak}}$ will shift upward, and precision lock duration will extend.

| Field | Content |
|-------|---------|
| Test | Measure CO₂ tolerance and precision before and after 4-week breathwork training. Track changes in $C_{\text{low}}$, $C_{\text{high}}$, and precision lock duration. |
| Outcome if confirmed | CO₂ tolerance is trainable — the tolerance window shifts with practice |
| Outcome if disconfirmed | CO₂ tolerance is fixed — no training effect |
| Status | Partially supported — Kox et al. (2014) confirms parameters shift; direct capnometry-level window shift untested |

### PREDICT-PREC-10 — Baseline CO₂ Tolerance Predicts Salience Dependence

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

## Version History

| Version | Date | Changes |
|---|---|---|
| v3.4 | 2026-09-13 | Converged with Central Reference v1.4. $P$ vs $P_{eff}$ distinction formalized — $U_C$ removed from $P$, $P_{eff} = P \cdot O_{pathway} \cdot U_C$ added as gate-condition variable. $O_{pathway}$ registered in §1.10 with functional-form caveat. Header updated. Changelog added. Cross-references verified at v1.4 section numbers. |
| v3.3 | 2026-09-12 | Converged with Central Reference v1.3. Added §1.4b (salience-triggered loop access), §1.11 (Xue et al. confirmation), §1.12 (REQT), §1.13 (collapse sequence), §1.14 (four profiles), §1.15 (load decomposition), §1.16 (why prior studies failed). §4.6 updated with $W_{enc} \leftrightarrow \mathcal{U}$ mapping. PREDICT-PREC-10 added. |
| v3.2 | 2026-09-11 | Added Part IV (Temporal Dynamics), Part III (Motor Gain), collapse hysteresis dynamics, encoding window dynamics. |
| v3.1 | 2026-09-11 | Added two-factor pressure, CO₂ uniformity, resonance breathing, individual variability. |
| v3.0 | 2026-09-11 | Complete precision equation with CO₂ tolerance window and chemoreflex jitter. |

---

## References

*(Unchanged from v3.3. All references verified.)
*I'm noting here there used to be a references section. I don't feel like gathering it right in this moment, but I need to upload this regardless*
