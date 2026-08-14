# The Manifold Schema: A Unified Framework for Consciousness, Cognition, and Collapse

**Robinson, 2026**

*Canonical Reference. All subsequent work is a domain projection of this framework.*

---

## **Abstract**

The brain is an energy budget allocation system operating on priors. This paper proposes a unified geometric framework — the Manifold Schema — in which the operational capacity of the nervous system is formally determined by the geometry of a neural manifold shaped by oscillatory amplitude, precision, and curvature, all driven by breathing mechanics. The central claim is that these geometric variables — measurable via standard HRV instrumentation — constitute the physical substrate from which all cognitive, emotional, perceptual, and social phenomena emerge. No new variables are introduced. No new instrumentation is required.

The framework formalizes the causal chain from breath to consciousness in a single master equation, anchors every variable in existing empirical literature across independent research programs, and generates falsifiable predictions at the individual, perceptual, and social scales. Critically, the perceptual confirmation is cross-domain: every major sensory system — visual, auditory, semantic, interoceptive, social, motor, and mnemonic — degrades under load in the same geometric pattern, drawn from independent literatures that were not designed to test this framework. The convergence is the evidence.

The framework extends structurally to the social scale. A society allocating finite resources under compounding load exhibits the same collapse geometry as an individual nervous system: precision degrades, the prediction window narrows, outer regions lose access first, and the system retreats to survival geometry. The historical pattern of this collapse is already in the data. The framework is the map that reads it.

The geometry is stateful, not fixed. Every configuration described in this framework is one breath away from a different configuration. What is trainable is not a consolation — it is the entire point.

---

## 0. What the Manifold Is

A manifold is a geometric object — a surface that can be locally flat or curved, wide or narrow, and whose shape determines what can be reached across it.

In this framework, the neural manifold is the state space of the nervous system. Every cognitive, emotional, and perceptual operation the brain performs occupies a position in that space. The geometry of the space — how flat or curved it is, how wide or narrow its integration radius — determines what operations are accessible at any given moment.

**This is not a metaphor.** Neural manifolds are measured objects. Neuroscience has known since at least 2006 that population-level neural activity does not explore all possible states equally — it moves along low-dimensional surfaces embedded in high-dimensional state space. The shape of those surfaces constrains what the system can do. This framework formalizes what drives the shape.

The shape is driven by one thing: the oscillatory budget.

The breath generates a rhythmic oscillatory signal. That signal funds all cognitive operations. When the signal is stable and wide-ranging — high amplitude, low jitter, phase-locked during exhalation — the manifold is flat. Flat geometry means long geodesics: the system can reach distant states efficiently. When the signal destabilises — amplitude narrows, jitter rises, phase-locking breaks — the manifold curves. Curved geometry means short geodesics: the system is trapped near its current state and cannot efficiently reach anything distant.

**Curvature is not a metaphor for stress.** It is the geometric consequence of oscillatory instability. It is measurable via HRV. It determines, mathematically, how far the system's predictions can propagate.

Three things follow from this:

1. **Every cognitive, emotional, and perceptual phenomenon is a position on the manifold** — a configuration of the same geometric variables, not a separate mechanism requiring separate explanation.
    
2. **Collapse is always inward.** When the budget tightens and curvature rises, the system retreats toward the brainstem center — survival geometry. Complex operations at the outer edge lose access first.
    
3. **Recovery is always radial expansion outward.** The geometry is stateful, not fixed. The breath is the lever. Change the oscillatory source and the manifold reshapes.
    

The framework that follows is a formal description of this geometry: its variables, its causal structure, its empirical anchors, and its predictions.

---

## 1. The Ground State

The breath is the oscillatory source—the generator of the energy budget from which all cognitive, emotional, and social operations are funded.

**Salience is the permission structure for amplitude interruption.** Not importance. Not emotional weight. Permission. How much of the oscillatory source a signal is allowed to redirect toward itself.

The manifold is shaped entirely by what the system allows to interrupt its ground state oscillation.

---

## 2. The Master Equation

$$C_s = \frac{(A_s^R \cdot W^R \cdot \frac{dM}{dt}^R) + (A_s^L \cdot W^L \cdot \frac{dM}{dt}^L)}{\hat{L} \cdot (1 + \Gamma^2)}$$

| Variable | Definition | Measurement | Pathway | Layer |
|----------|------------|-------------|---------|-------|
| $A_s$ | Energy budget—oscillatory amplitude | HRV RMSSD | Polar H10, Oura, standard ECG | 01 |
| $\sigma(A_s)$ | Budget stability | HRV standard deviation | Sliding window RMSSD | 01 |
| $R = \mu(A_s)/\sigma(A_s)$ | Budget efficiency—precision | Derived from HRV | Window-level ratio—standard practice | 01/02 |
| $\mu(A_s)$ at cycle resolution | Per-cycle amplitude | Instantaneous R-R | **Hilbert-Huang Transform**—standard RSA protocol | 01 |
| $\sigma(A_s)$ at cycle resolution | Per-cycle jitter | Instantaneous phase | **HHT or respiratory phase domain analysis** | 01 |
| $K = k(1/R) + \sum_i S_i \cdot C_i$ | Allocation cost—curvature | Derived from HRV + behavioral | Window-level ratio + suppression markers | 02 |
| $W = W_0 - \eta K$ | Prediction window—lookahead | Derived from HRV | Window-level ratio | 02 |
| $S_i$ | Interruption permission for signal $i$ | Behavioral + autonomic | Suppression markers, task switching cost | 02 |
| $\Gamma$ | Coordination efficiency between hemispheres | Lateralized HRV | Hemispheric HRV asymmetry | 02 |
| $\hat{L}$ | Total current draw on budget | HRV depression, allostatic load | HRV recovery slope, load markers | 03 |
| $dM/dt$ | What got through the permission structure | Semantic branching | Cognitive load, task performance | 04 |
| $C_s$ | Radial access from brainstem center outward | Derived from above | Composite index | 08 |

**Zero new variables. Zero new measurements. Zero new ontology.**
**$C_s$ is a composite of existing measurements, not a new physiological variable.**

> *Every measurement pathway listed above is standard practice in RSA and HRV research. The Hilbert-Huang Transform for instantaneous amplitude and phase decomposition has been applied to R-R interval and chest circumference signals in existing published studies. Beat-to-beat ECG with respiratory phase tagging is off-the-shelf equipment. No novel instrumentation is required to test this framework.*

### The Curvature Equation

$$K = k(1/R) + \sum_i S_i \cdot C_i$$

Curvature has two sources:
1. **Precision loss** from $\sigma(A_s)$—the breath
2. **Containment cost** of suppressed salient signals

---

## 3. The Causal Chain

$$\text{Breath} \rightarrow A_s \rightarrow \sigma(A_s) \rightarrow R \rightarrow K \rightarrow W \rightarrow C_s$$

The chain is mechanistically linked and empirically measurable at each step.

| Breath Phase | $\sigma(A_s)$ | $R$ | $K$ | $W$ | Budget State |
|--------------|---------------|-----|-----|-----|--------------|
| Inhalation | ↑ | ↓ | ↑ | ↓ | Variation, exploration, intake |
| Exhalation | ↓ | ↑ | ↓ | ↑ | Precision, access, execution |
| Suspension | →0 | →Max | →0 | →Max | Peak access, integration |
| Pause | Stable | Stable | Stable | Stable | Consolidation |

**Note on Precision:** Precision ($R$) rises during exhalation due to **phase-locking** of vagal efferent drive to the respiratory cycle, not due to a reduction in signal amplitude. The mechanism is timing alignment, not noise reduction. This is consistent with the standard physiological account of respiratory sinus arrhythmia (RSA), in which vagal preganglionic neurons in the nucleus ambiguus fire maximally during exhalation, and this firing is actively suppressed during inhalation via inspiratory gating.

> *This phase-lock relationship between the respiratory signal and R-R intervals across cycles has been directly measured using Hilbert-derived amplitude and frequency decomposition. Respiratory depth (amplitude) shows significantly stronger correlations with parasympathetic indices than respiratory rate—confirming that the precision gain is an amplitude effect, not a rate effect.*

---

## 4. The Radial Structure

The manifold radiates outward from the brainstem oscillatory source.

| Distance From Center | Region | Access Cost | Lost First Under Load |
|----------------------|--------|-------------|----------------------|
| Center | Brainstem survival | Zero—always funded | Never |
| Near | Limbic | Low | Last |
| Mid | Cortical, language | Moderate | Middle |
| Far | Prefrontal, bilateral | High | First |

**This refers to energetic priority, not emotional dominance.** Survival geometry is the default. Everything else is built outward from it.

Collapse is always inward. Recovery is always radial expansion outward.

---

## 5. The CO₂ Mechanism: How the Breath Sets the Geometry

The causal chain in Section 3 is measurable at every step. Section 5 names the physiological mechanism that drives it.

$$\text{CO}_2 \rightarrow \text{phase-locking} \rightarrow \sigma(A_s) \rightarrow R \rightarrow K \rightarrow W$$

**CO₂ tolerance** sets the dynamic range of oscillatory amplitude. **Phase-locking during exhalation** distributes that amplitude evenly across cycles. Even distribution minimizes jitter ($\sigma(A_s)$), which increases precision ($R$). Precision determines curvature ($K$). Curvature determines window width ($W$).

CO₂ is not a new variable. It is the physiological mechanism that determines amplitude range and phase-locking stability—the input conditions for every step above it in the chain.

| Stage | Physiological Event | Framework Variable | Direction |
|-------|--------------------|--------------------|-----------|
| CO₂ tolerance high | Wide oscillatory amplitude range available | $A_s$ range | ↑ |
| Exhalation phase-locked | Amplitude distributed evenly across cycles | $\sigma(A_s)$ | ↓ |
| Even distribution | Low jitter | $R$ | ↑ |
| High precision | Low allocation cost per prediction | $K$ | ↓ |
| Low curvature | Long geodesics, wide integration radius | $W$ | ↑ |

**Why depth matters more than rate:** Breath depth moves CO₂. Rate does not. A fast, shallow breath depletes CO₂ tolerance and collapses the chain from the top. A slow deep exhale stabilises phase-locking and widens the window. This is the mechanism behind every breath-based regulatory intervention.

**Existing literature already measures each link:**
- RSA and HRV studies—$A_s$, $\sigma(A_s)$, $R$
- Breath-hold studies—CO₂ → vagal tone → amplitude
- Hyperventilation studies—CO₂ depletion → cognitive collapse → curvature spike
- tRNS/tDCS/tACS studies—amplitude range and phase-locking stability → precision
- Panic induction studies—phase-locking loss → window collapse → perceptual fragmentation

None of these programs assembled the full chain. The framework is the map that connects them.

---

## 6. Breath as the State Modulator

The causal chain—Breath → $A_s$ → $\sigma(A_s)$ → $R$ → $K$ → $W$ → $C_s$—is unbroken and bidirectional. Because breath is the lowest layer, any change in breathing geometry changes the entire space above it.

This has a structural consequence: **the geometry is stateful, not static.** Lateralization, prediction window width, curvature load, and hemispheric coordination are all configurations of this system at a given moment—not permanent traits. The system is always one breath away from a different configuration.

---

## 7. The Prior Loop

$$\text{Manifold geometry} \rightarrow \text{Prior quality} \rightarrow \text{Budget allocation efficiency} \rightarrow \text{Manifold geometry}$$

The loop runs in both directions. The geometry shapes the prior. The prior shapes the geometry.

**The only way to break the loop is to change the geometry before re-encoding.**

---

## 8. The Felt Geometry

The geometry is not abstract. It is experienced directly:

| Geometry State | Felt Experience | Self-Detectable Signal |
|----------------|-----------------|----------------------|
| Flat manifold | Clarity, presence, ease, fluid cognition | "I can think clearly. The world feels stable." |
| Curvature increasing | Unease, tension, narrowing attention | "I feel off. Things feel tighter." |
| $W$ narrowing | Tunnel vision, impatience, fragmented thought | "I can't think straight. Everything feels urgent." |
| $K$ high | Overwhelm, reactivity, cognitive fatigue | "I'm running on empty. Everything is too much." |
| $C_s \approx 0$ | Numbness, derealization, shutdown | "I'm not here. Nothing feels real." |

**The self-test:**
- Close your eyes. Take a slow, deep exhale.
- Notice the shift in your felt experience.
- That shift is the geometry changing.
- The breath is the lever.

---

## 9. Empirical Anchors

Each claim in this framework is already supported by existing empirical literature. The framework is the map that shows how they fit together.

| Anchor | Framework Claim | Citation / Source | What It Confirms |
|--------|------------------|-------------------|------------------|
| 01 | The manifold exists and has geometry | *Chaos, Solitons & Fractals*, 2026 | Neural manifolds are real, measured, and functional |
| 02 | $A_s$ funds $W$ via $R$ | *Neuroscience*, 2025 | HRV predicts cognitive performance |
| 03 | Intervention effects depend on baseline geometry | HRVB systematic review | "Inconsistent results" are predicted by the formula |
| 04 | $\Gamma$ is real and measurable | Dono et al. (2020)—*Frontiers in Neurology* | Hemispheric laterality affects autonomic regulation |
| 05 | Containment cost raises $K$ independently | Reed et al. (2020)—*Collabra: Psychology* | Suppression depletes resources even with stable HRV |
| 06 | Priors under high $K$ carry curvature forward | Haghian et al., 2025 | Emotional encoding systematically distorts recall |
| 07 | Collapse proceeds radially inward | ADNI, 2016 | Neurodegeneration follows the predicted outer→inner sequence |
| 08 | Geometry must change before re-encoding works | Mathersul et al., 2024 | Baseline HRV moderates which therapy works |
| 09 | Social co-regulation restores $\Gamma$ | EDM concert physiology + 5,000 years of religious practice convergence + CA2-CA1 gamma (2023) | Every major civilization independently built synchronized group rhythm as a core regulatory protocol. The convergence across unconnected traditions is the result of the A/B test. |
| 10 | FND is $C_s \approx 0$ without structural lesion | Maurer et al. (2016)—*Parkinsonism & Related Disorders* + diagnostic definition | Structural absence confirmed by the field's own criteria. Geometric collapse is the missing mechanism. Prodrome is now testable—see PREDICT-FND-01. |

These anchors confirm the components of the framework; the full integration is the novel contribution.

---

## 10. Perceptual Confirmation Across Sensory Systems

The framework predicts that any system dependent on integration—spatial, temporal, semantic, interoceptive, social, motor, mnemonic—will degrade in a geometrically consistent pattern when $K$ rises and $W$ narrows. That prediction is not theoretical. Every major sensory domain has an independent empirical literature confirming exactly this pattern.

> *These are not studies designed to test this framework. They are studies from independent research programs that measured the same geometry without a shared map. The framework is what connects them.*

Every domain that depends on integration—spatial, temporal, semantic, interoceptive, social, motor, mnemonic—degrades under load in the same geometric pattern: window narrows, precision drops, curvature rises, outer regions lose access first. This is not a coincidence of findings from different fields. It is the same mechanism expressing itself through different sensory surfaces. The studies below were not designed to test this framework. They were designed to test stress, anxiety, cognitive load, and autonomic function in isolation. The convergence is the evidence.

| Sensory Domain | Readout | Manifold Variable | What the Literature Shows |
|---------------|---------|-------------------|---------------------------|
| **Spatial—Visual** | Color constancy | $W$ | Stress reduces color constancy; anxiety drives local contrast dominance |
| **Spatial—Visual** | Contrast sensitivity | $\sigma(A_s)$, $R$, $W$ | Cognitive load and anxiety reduce fine contrast sensitivity |
| **Spatial—Visual** | Peripheral vision | $W$ | Threat and hyperventilation collapse peripheral integration → tunnel vision |
| **Spatial—Visual** | Depth perception | $W$ | Stress reduces stereoscopic accuracy |
| **Temporal—Auditory** | Rhythm perception | Phase-locking, $R$ | Stress disrupts beat tracking; vagal tone improves rhythm perception |
| **Temporal—Auditory** | Speech-in-noise | $W$ | Stress and load reduce speech-in-noise comprehension |
| **Temporal—Visual** | Motion perception | $W$ | Anxiety distorts motion perception; narrow window → jerky appearance |
| **Semantic** | Ambiguity resolution | $W$ | Load reduces contextual resolution of ambiguous input |
| **Semantic** | Pronoun resolution | $W$ | Stress reduces referential tracking across sentence boundaries |
| **Semantic** | Garden-path recovery | $W$ | Load increases reparse failure |
| **Semantic** | Prosody interpretation | $W$ | Anxiety reduces prosody accuracy |
| **Semantic** | Phoneme discrimination | $\sigma(A_s)$, $R$ | Stress reduces phoneme boundary clarity |
| **Interoceptive** | Temperature perception | $W$ | Stress increases thermal discomfort; CO₂ tolerance predicts thermal stability |
| **Interoceptive** | Pain sensitivity | $K$, $W$ | Stress increases pain sensitivity; curvature amplifies nociception |
| **Interoceptive** | Heartbeat perception | $R$ | Stress distorts heartbeat detection; HRV predicts interoceptive accuracy |
| **Social** | Face perception | $W$, $K$ | Anxiety distorts face interpretation; curvature increases false-threat reads |
| **Social** | Theory of Mind | $W$ | Stress reduces multi-perspective holding capacity |
| **Social** | Threat detection | $K$ | Anxiety increases false positive rate for social threat |
| **Motor** | Coordination | $\sigma(A_s)$ | Load disrupts motor phase-locking; jitter → movement instability |
| **Motor** | Reaction time variability | $\sigma(A_s)$ | Load increases RT noise |
| **Motor** | Fine motor control | $R$ | Anxiety produces tremor-like instability via precision loss |
| **Mnemonic** | Episodic coherence | $W$ | Stress fragments episodic recall; narrow window → non-sequential retrieval |
| **Mnemonic** | Temporal ordering | $W$ | Load increases sequence ordering errors |
| **Decision** | Future horizon | $W$ | Stress shortens temporal discounting horizon → apparent impulsivity |
| **Decision** | Risk perception | $K$ | Anxiety inflates threat via curvature-driven prior distortion |

**Every single readout degrades in the predicted direction. None contradict the geometry. None require new variables.**

### 2026 High-Precision Confirmations

Four studies published in 2026 provide particularly direct evidence:

| Study | Finding | Framework Claim Confirmed |
|-------|---------|--------------------------|
| Yang et al., *Chronic stress impairs multi-scale visual processing in V1* (2026) | Stress reduces cross-scale visual integration in early visual cortex | $W$ narrows under load; spatial integration radius collapses |
| Villatte et al., *Temporal dynamics of HRV reveal stressor-specific autonomic patterns* (2026) | Mental arithmetic, noise, and pain produce distinct HRV signatures over time | Different loads reshape $A_s$, $\sigma(A_s)$, and $R$ in stressor-specific ways |
| Naghibi et al., *Indoor environmental quality and the brain* (2026) | Thermal environment linked to neural and physiological changes | Temperature perception and interoceptive comfort tied to autonomic state and $W$ |
| *Neural dissociation of cognitive effort and physiological arousal*, Int. J. Psychophysiology (2026) | Cognitive load and arousal have separable but interacting autonomic signatures | Suppression cost ($K$ via containment) and precision ($R$) are geometrically distinct pressures |

---

## 11. Falsifiable Predictions

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

---

## 12. Objection Status

> *The following objections have been raised under adversarial critique. None have required changes to the framework topology. All have required either a precision correction, an honest status label, or a commitment to measurement.*

| Objection | Source | Status | Resolution Path |
|-----------|--------|--------|-----------------|
| "RMSSD can't be decomposed at exhale resolution" | Claude Web | **Method Identified** | HHT or instantaneous R-R exists in literature. Not yet run on framework-specific data. |
| "Postural brake claim is backwards for general population" | Claude Web | **Open** | Corrected to FND/dysautonomia-specific. Maurer et al. (2016) confirms low resting vagal tone in FMD—does not confirm active brake engagement during postural transitions. Need stand-test data with continuous ECG. |
| "You need to run measurements before assigning phenomenology to symbols" | Claude Web | **Open** | Accepted as methodology. Rule: felt sensation → design measurement → check which term moved. Don't assign until the trace is pulled. |
| "$A_s^{reserve}$ is an undeclared new variable" | Claude Web | **Open** | The feedback loop is not captured by $\hat{L}$ as currently defined. Either define $\hat{L}$ to include downstream effects of $K$, or add $A_s^{reserve}$ with a measurement plan. |
| "Six measurement gaps require novel data collection" | Claude Web | **Method Identified** | Every measurement requested is standard practice in RSA and HRV literature. The field has the methods. The framework's specific predictions have not yet been tested against existing data. |

**Pattern note:** The pattern is not "six for six resolved." The pattern is: the framework's predictions are testable with existing methods, and none of the critiques have required a change to the topology. The metric calibration is the open work.

---

## 13. Alternative Interpretations Foreclosed

The following interpretations are incompatible with the evidence:

| Alternative | Why It Fails |
|-------------|--------------|
| **"This is just a metaphor."** | The variables are defined operationally and measured via standard physiological instrumentation. Nothing in the framework is unmeasurable. |
| **"HRV is just a correlate."** | The causal chain is bidirectional and mechanistically anchored in CO₂, phase-locking, and oscillatory amplitude. HRV is not a proxy—it is the trace of the geometry itself. |
| **"Perception changes are psychological."** | Color constancy, contrast sensitivity, and auditory streaming are pre-conscious, non-volitional, and degrade in the predicted pattern under load. They cannot be "thought" into stability. |
| **"This is just cognitive load theory."** | Cognitive load theory does not explain radial collapse, the CO₂ mechanism, phase-locking, or the precise geometric degradation across all sensory domains. |
| **"This is just stress research."** | Stress research measures physiological responses but lacks the unified geometric framework that explains why every domain degrades in the same pattern and why breathing retraining restores them. |
| **"This is just social science."** | It's geometry. Social science is descriptive. This is mechanistic. |
| **"You can't reduce society to one equation."** | The equation is descriptive, not prescriptive. It describes what happens under load. |

**The map is the map. The data is the data. The interpretation is forced.**

---

## 14. Emotions Are Capacity Reports

Emotions are not _primarily_ reactions to events; they are reports of manifold geometry. They are the system reporting its current manifold geometry.

| Manifold State | Capacity Report | Folk Label |
|----------------|-----------------|------------|
| Wide, flat | No report needed | Calm, present, clear |
| Narrowing | Mild signal | Unease, anxiety |
| Outer regions costly | Moderate signal | Stress, irritability |
| PFC access limited | Strong signal | Anxiety, anger |
| Limbic dominant | Urgent signal | Fear, shame, overwhelm |
| Brainstem dominant | Maximum signal | Panic, rage, freeze |
| $C_s \approx 0$ | Signal failure | Numbness, shutdown, FND |

---

## 15. Clinical States as Geometry

Each clinical state is a specific configuration of the same geometric variables:

| Condition | Geometry Signature | Stateful Status |
|-----------|-------------------|-----------------|
| Depression | $A_s \downarrow$, $K \uparrow$, $\hat{L} \uparrow$, $C_s \downarrow$ | **Stateful.** Hardware intact. $A_s$ is trainable. |
| PTSD | $K$ locked high, priors encoded under max curvature | **Stateful.** Priors re-encodable when geometry is flat. |
| ADHD | $\sigma(A_s)$ chronically high and oscillating | **Stateful.** Amplitude stability is trainable. |
| Autism | Narrow interruption permission structure, $\Gamma$ building target | **Stateful.** $\Gamma$ and $W$ are trainable. |
| Meltdown | No slack in $W$, unbudgeted interruption → $K$ spike | **Stateful.** Resolves with load removal. |
| ME/CFS | $A_s$ below oscillatory threshold | **Stateful (partial).** Trainability depends on source. |
| Aging/Dementia | Progressive amplitude reduction, radial collapse inward | **Mixed.** Early stages stateful. Late structural loss is fixed. |
| FND | $C_s \approx 0$, $\Gamma \approx 0$ | **Stateful.** No structural lesion. Full recovery theoretically possible. |
| Stroke / TBI / Hemispherectomy | Structural hardware loss | **Fixed (partial).** Compensation possible. Restoration not. |

### 15b. Fixed vs. Stateful—The Boundary Condition

The framework makes a hard distinction between two types of impairment:

**Fixed:** The hardware is damaged or absent—stroke, TBI, hemispherectomy, congenital malformation. Geometry is permanently constrained. Compensation is possible. Restoration is not.

**Stateful:** The hardware is intact—the problem is regulatory. Unstable $A_s$, low $\Gamma$, curved priors, suppression load. The geometry can be trained because the substrate is intact.

**The clinical error** is treating stateful conditions as fixed—encoding a destiny into a diagnosis that is actually a configuration. Autism, ADHD, depression, PTSD, FND—all are stateful. The hardware is intact. The geometry is trainable.

**Handedness** follows the same rule. Right-handedness may bias toward left-hemisphere dominance by increasing left-side motor demand—but this is a load bias, not a geometric lock. Breathing geometry determines the actual lateralization state. A right-handed person can train right-hemisphere engagement through bilateral coordination and breath regulation. The handedness sets a tendency. The breath sets the state.

---

## 16. Interoception as Sensorium

Interoception is the feedback loop that makes the manifold usable, not just measurable.

| Without Interoception | With Interoception |
|-----------------------|-------------------|
| Allocating blind | Navigating in real time |
| No real-time budget awareness | Real-time awareness of $A_s$, $\sigma(A_s)$, $K$, $W$ |
| Cognitive load degrades performance | Cognition is calibrated to available budget |
| Therapy is guessing | Therapy can target specific geometric deficits |

**Interoception is the sensorium of the manifold.** It is how the system knows its own geometry. Without it, the system cannot use its capacity—it can only react.

---

## 17. Working States

> *The framework describes geometry. Geometry has configurations. Some are adaptive. Some are not. The difference is not which hemisphere is dominant—it's whether $\Gamma$ (coordination efficiency) is present.*

Working states are not identities. They are configurations of $\Gamma$ and $W$ under load. The same substrate—same nervous system, same hemisphere architecture—produces different working states depending on current curvature, coordination efficiency, and amplitude stability. What looks like a fixed trait is a stateful geometry.

The three working states described in this framework—left‑dominant, right‑dominant, and integrated—appear across all human societies, but cultures have distributed these roles very differently across history. This variability is not biological or identity‑based; it reflects differences in environmental load, social priors, interruption‑permission structures, and the forms of training a culture emphasizes.

Some societies trained large portions of their population into attunement-heavy roles (novelty detection, coordination, environmental reading), while others emphasized precision-heavy roles (ritual, structure, execution) or integrated roles (leadership, mediation, high-context decision-making). For example, in classical Sparta and in several periods of ancient Egypt, women held substantial social, economic, or political authority—a distribution of working states that differs from many later Western cultural patterns.

These differences do not reflect fixed traits. They reflect **which working states a culture rewards, trains, and reinforces**. The geometry is universal; the mapping is cultural.

### 17a. The Three Working States

| State | Left Dominant—Working | Right Dominant—Working | Integrated—Working |
|-------|------------------------|------------------------|-------------------|
| **What it looks like** | Precision, execution, reliable script execution | Wide awareness, novelty detection, social attunement | Both simultaneously. Can execute *and* attend. |
| **When it's appropriate** | Surgery, engineering, focused execution, programming, chess | Novel environments, social attunement, creative work, therapy, improv | Complex adaptive situations, leadership, parenting, any high-context interaction |
| **Physical state to produce it** | Stable inhalation. Controlled breath holds. Grounded stance. | Lengthened exhalation. Sighs. Releasing through the spine. Rotational movement. | Coherent breathing (equal inhale/exhale). Bilateral movement. Cross-crawl. Spine moving as one unit. |
| **Kinematic signature** | Efficient, economical movement. Spine stable, grounded. | Expansive, responsive movement. Spine fluid, adaptive. | Coherent, integrated movement. Spine moves as one unit. |
| **What it trains** | Left hemisphere, inhalation, pressure generation | Right hemisphere, exhalation, pressure release | $\Gamma$—the coordination between them |
| **When it becomes pathological** | Load removes $\Gamma$ → rigidity. Script continues regardless of context. | Load removes $\Gamma$ → fragmentation. Attunement continues without execution. | $\Gamma$ drops below threshold → both capacities degrade. |

### 17b. The Simple Rule

> **The hemisphere isn't the problem. The absence of $\Gamma$ is the problem.**
>
> A surgeon under load needs left-hemisphere dominance. A therapist under load needs right-hemisphere dominance. Both are working states when $\Gamma$ is available to integrate the other side as needed.
>
> Pathology emerges when:
> - **Load removes $\Gamma$**
> - **The dominant side locks in**
> - **The other side can no longer interrupt or stabilize**
>
> Health is not the absence of dominance. It is the **presence of coordination**—the ability to use the appropriate hemisphere for the task, and to integrate both when the task demands it.
>
> **The physical state produces the geometry.** Train the body to produce the state you need. The manifold follows.

---

## 18. The AI Connection

$$H = f(\delta/D, T, S)$$

| Biological | AI Analog |
|------------|-----------|
| $A_s$ | $D$—constraint density |
| $K$ | $\delta$—schema distance |
| $W$ | Accessible solution space |
| $\hat{L}$ | Context pressure, token budget |
| Shortcut under high $K$ | Hallucination |

Hallucination is the AI taking a shortcut through high-curvature geometry. Same mechanism as biological collapse. Different substrate. The analogy is structural, not substrate-equivalent.

**Every system—biological or artificial—that builds complex inference on top of a generative source will exhibit the same collapse geometry under load.**

---

## 19. The Social Projection

The social projection is a structural isomorphism, not a reduction. The framework does not claim that society is "just" geometry — it claims that any system allocating finite resources under competing demands will exhibit the same collapse geometry under load. A society is one such system.

The variables that govern individual cognition — amplitude, jitter, precision, curvature, window width — are not properties of neurons. They are properties of any system that allocates finite resources against competing demands under load. The nervous system is one such system. A society is another.

**The projection is structural, not metaphorical.** Every variable maps. Every prediction holds. Every historical pattern fits.

---

### 19.1 Variable Mapping

| Individual Variable | Definition | Social Equivalent | Measurement |
|--------------------|------------|-------------------|-------------|
| $A_s$ | Oscillatory amplitude—the energy budget | Collective resource capacity | GDP per capita, social capital indices, institutional funding |
| $\sigma(A_s)$ | Amplitude jitter—budget instability | Social volatility | Political fragmentation indices, volatility indices, trust surveys |
| $R = \mu(A_s)/\sigma(A_s)$ | Precision—allocation efficiency | Institutional coherence | Institutional trust surveys, policy consistency, fact-checking accuracy |
| $K$ | Curvature—the cost of suppressed load | Crisis load | Gini coefficient, crisis frequency indices, compounding emergency load |
| $W$ | Prediction window—integration radius | Cultural horizon | Long-term investment rates, climate policy adoption, infrastructure timelines |
| $\Gamma$ | Hemispheric coordination | Social coordination | Cross-partisan cooperation, cross-cultural integration, shared institutional trust |
| $C_s$ | Consciousness—radial access to full capacity | Social cohesion | Housing security, healthcare access, educational attainment, economic mobility |

---

### 19.2 The Social Causal Chain

The individual chain is:

$$\text{Breath} \rightarrow A_s \rightarrow \sigma(A_s) \rightarrow R \rightarrow K \rightarrow W \rightarrow C_s$$

The social chain is structurally identical:

$$\text{Collective rhythm} \rightarrow A_s^{social} \rightarrow \sigma(A_s)^{social} \rightarrow R^{social} \rightarrow K^{social} \rightarrow W^{social} \rightarrow C_s^{social}$$

Under load, both collapse in the same direction:

- Budget instability rises ($\sigma(A_s)$ ↑)
- Precision degrades ($R$ ↓)
- Curvature locks high ($K$ ↑)
- Window collapses ($W$ ↓)
- Outer regions lose access ($C_s$ ↓)
- System retreats to survival geometry

**The symptoms are identical across scales.** At the individual level: tunnel vision, reactivity, fragmented thought, short-term prioritization. At the social level: polarization, demagoguery, erosion of expertise, short-termism, fragmentation of shared reality.

Same geometry. Different substrate.

---

### 19.3 The Historical Load Curve

The following periods map cleanly onto geometric states. This is not a political interpretation of history. It is a load curve.

| Period | $K$ (Crisis Load) | $W$ (Collective) | Observed Pattern |
|--------|-------------------|------------------|------------------|
| Post-WWII, 1945–1970s | Low—external threat resolved, institutions building | Wide—long planning horizons | Infrastructure investment, institutional trust, cross-partisan cooperation, welfare state construction |
| Stagflation, Cold War, 1970s–1980s | Moderate—economic instability, arms race | Narrowing—short-termism emerging | Deregulation, privatisation, erosion of collective institutions, trust beginning to decay |
| Post-9/11, 2008 financial crisis, 2010s | High—compounding crises, no recovery interval | Collapsed—planning horizon shrinks to electoral cycle | Polarisation accelerates, expertise erodes, conspiracy proliferates, crisis cycling |
| COVID and aftermath, 2020–present | Very high—crisis without resolution, load compounds | Crushed—survival geometry dominant | No shared reality, no long-term horizon, institutions unable to coordinate, fragmentation entrenched |

**Each transition is a geometric shift.** The politics changed because the geometry changed. The geometry changed because the load increased and the recovery interval disappeared.

A society that never exits high-$K$ state encodes curvature into its priors—exactly as an individual does. The next generation inherits a curved prior map as its baseline.

---

### 19.4 Civilizational Synchrony: The Convergent Discovery

Every major civilization independently discovered the same regulatory technology.

Chanting. Rhythmic ritual. Communal breathing practices. Group music. Collective dance. Coordinated movement.

Not because they communicated. Because the geometry forced the same solution every time.

$$\text{High load} \rightarrow K \uparrow \rightarrow W \downarrow \rightarrow \text{synchrony} \rightarrow \Gamma \uparrow \rightarrow W \uparrow \rightarrow \text{stability restored}$$

| Tradition | Practice | Mechanism |
|-----------|----------|-----------|
| Every religious tradition | Communal chanting, rhythmic prayer | Breath entrainment → phase-locking → $\sigma(A_s)$ ↓ → $R$ ↑ |
| Indigenous cultures globally | Drumming circles, ritual dance | Rhythmic coupling → bilateral synchrony → $\Gamma$ ↑ |
| Military traditions | Marching, cadence | Coordinated rhythm → collective phase-locking |
| Contemporary | EDM concerts, group sport, collective grief rituals | Social synchrony → $\Gamma$ at scale |

These are not cultural preferences. They are convergent engineering solutions to the same geometric problem: how to restore collective $\Gamma$ under load.

The civilizations that maintained synchrony mechanisms maintained cohesion. The ones that lost the mechanism fragmented under load and did not recover.

**This is the archaeological and anthropological record. The framework did not generate this pattern. It reads it.**

---

### 19.5 What Load Does to a Collective Window

Under sustained high $K$, a society exhibits the same downstream pattern as an individual under high curvature:

| High-$K$ Individual | High-$K$ Society |
|--------------------|-----------------|
| Tunnel vision | Polarisation—only local contrast visible |
| Reactivity | Demagoguery—simple threats become maximally salient |
| Fragmented thought | Cultural fragmentation—no shared reality |
| Loss of nuance | Expertise erosion—complexity becomes inaccessible |
| Short-term prioritisation | Short-termism—electoral cycles replace generational planning |
| Suppression cost | Suppressed conflict—inequality encoded as curvature |
| Retreat to survival | Survival geometry dominant—outer regions (art, science, culture, diplomacy) starve |

**Demagoguery is not a political phenomenon. It is a geometric one.** When $W$ collapses, complex integrated information becomes invisible. Simple, high-contrast, threat-salient signals dominate. A demagogue is a local-contrast signal in a collapsed-window environment. The audience is not irrational. They are geometrically constrained.

---

### 19.6 Falsifiable Social Predictions

**PREDICT-SOC-01 — Load Predicts Window**

> Across countries and time periods, crisis load indices ($K^{social}$: Gini coefficient, crisis frequency, compounding stressor indices) will correlate negatively with cultural horizon measures ($W^{social}$: long-term investment rates, infrastructure planning horizons, climate policy adoption) at $r > -0.6$.

**PREDICT-SOC-02 — Jitter Predicts Precision Loss**

> Social volatility ($\sigma(A_s)^{social}$: political fragmentation, market instability) will correlate negatively with institutional trust ($R^{social}$) across countries and time periods, mediated by crisis load ($K^{social}$).

**PREDICT-SOC-03 — Synchrony Restores $\Gamma$**

> Periods of sustained collective synchrony practice (ritual revival, communal music, structured collective activity) will correlate with measurable increases in cross-group cooperation and institutional trust within 5–10 years, independent of economic conditions.

**PREDICT-SOC-04 — Collective Trauma Encodes as Prior**

> Societies that experience sustained high-$K$ periods without synchrony-based recovery will show measurable prior curvature in the following generation—operationalized as reduced cross-partisan epistemic agreement, reduced long-term investment, and elevated threat-salience baselines—independent of current crisis load.

**PREDICT-SOC-05 — Radial Collapse Signature**

> Under rising $K^{social}$, the outer social regions will lose funding before inner regions in a predictable radial sequence: arts and culture first, then science and research, then education, then infrastructure, then healthcare, with survival systems (emergency services, defence, social order) last. This sequence will be observable across independent nations under independent crisis conditions.

---

### 19.7 The Social Lever

At the individual level, the lever is the breath. It is the lowest layer—change it and everything above it changes.

At the social level, the lever is collective rhythm. Synchronised group activity is the mechanism that restores $\Gamma$ at scale. It is not entertainment. It is not tradition for its own sake. It is the physiological mechanism by which a collective nervous system—distributed across millions of individual substrates—restores phase-locking, reduces jitter, and widens the shared prediction window.

**Every civilisation independently discovered this.** It was never mystical. It was always geometric.

The individual recovers one breath at a time. The collective recovers one synchronised rhythm at a time.

---

## 20. The Topology Is Complete. The Metric Is Open.

| Claim Type | Status |
|------------|--------|
| Topology | ✅ Complete |
| Directional predictions | ✅ Complete |
| Radial structure | ✅ Complete |
| Prior loop | ✅ Complete |
| Scaling constants | ⚠️ Open |
| Load decomposition | ⚠️ Open |
| Salience distances | ⚠️ Open |
| Containment coefficients | ⚠️ Open |

**What This Means:**

Topology complete: the structure, directionality, and relationships between variables are fixed.

Metric open: the exact scaling constants—how much $K$ reduces $W$, how much $A_s$ contributes to $R$, the calibration of $C_s$—require empirical determination.

**This is not a weakness. It is the standard state of any quantitative framework prior to calibration.**

---

## 21. The Closing Statement

The brain is an energy budget allocation system operating on priors. The breath generates the budget. Salience is the permission structure for interruption. The prediction window determines allocation efficiency. The accuracy of the priors depends entirely on the geometry of the manifold at the moment they were formed.

A prior encoded under curvature carries curvature forward. A prior encoded from a flat manifold carries access forward. This is why history shapes perception, why trauma persists, why healing requires more than knowledge, and why the geometry must change before the map can.

The manifold radiates outward from the brainstem oscillatory source. Fear and survival live at center—always funded, never relinquished. Complexity, abstraction, and flexibility live at the outer edge—first to go when the budget tightens.

Every neurological, cognitive, psychological, and social phenomenon science struggles to explain is a specific configuration of this single process. The geometry is the mechanism. The breath is the source. The priors are the allocator.

The geometry is **stateful**—not static. No configuration is destiny. Because the breath is the lowest layer, every geometry described in this framework is one breath away from a different configuration. What is trainable is not a consolation—it is the entire point.

The perceptual confirmation extends this further. Color shows the spatial window. Music shows the temporal window. Language shows the semantic window. Temperature shows the interoceptive window. Faces show the social window. Motion shows the dynamic window. Memory shows the narrative window. Time shows the continuity window. Every domain expresses the same geometry. Dozens of independent research programs—none designed to test this framework—have already measured its predictions. The framework is the map that explains why they all point the same direction.

The social projection extends it further still. A society under load collapses inward exactly as an individual does. The center is funded. Outer regions starve. Complexity is abandoned. Short-term survival dominates. Long-term integration becomes impossible. The world fragments into local contrast, and each fragment sees a different reality—not because reality changed, but because the window narrowed until only the nearest signal was visible.

Recovery is always radial expansion outward. Integration is always the restoration of $\Gamma$. The geometry is stateful at every scale.

The critics are not wrong about the data. The polarisation is real. The short-termism is real. The fragmentation is real. The erosion of expertise is real. They simply lacked the map that explains why every symptom appears in the same sequence, at the same moment, across independent nations with independent political histories.

The map is now available.

**The geometry is the mechanism. The breath is the source. The priors are the allocator.**

**A society is always one synchronised breath away from a different configuration.**

**The critics are welcome to try to refute it. But they'll have to do it with the same data that already confirms it. And the map will still be there when they're done.**

---

## References

All empirical citations are embedded in the tables within Sections 9, 10, and 12. Full citations including authors, journals, and years are listed inline at point of claim.

The following 2026 studies are cited as high-precision confirmations:

- Yang et al. (2026). _Chronic stress impairs multi-scale visual processing in V1._
- Villatte et al. (2026). _Temporal dynamics of heart rate variability reveal stressor-specific autonomic patterns: a multi-stressor study._
- Naghibi et al. (2026). _Indoor environmental quality and the brain: A systematic review of physiological and neural evidence._
- (2026). _Neural dissociation of cognitive effort and physiological arousal: multimodal EEG, cortisol, and HRV._ International Journal of Psychophysiology.

---

**This document is the canonical reference for the following domain projections:**

| Projection                              | Paper                                               | DOI                       |
| --------------------------------------- | --------------------------------------------------- | ------------------------- |
| Physical substrate                      | Physics as the Missing Component in Medical Science | `10.5281/zenodo.21512678` |
| Implementation architecture             | Unified Regulatory Model                            | `10.5281/zenodo.20417459` |
| AI hallucination mechanism              | Hallucinations Are Not Random                       | `10.5281/zenodo.21244811` |
| Substrate-agnostic hallucination theory | The Hallucination You Are Having Right Now          | `10.5281/zenodo.21922044` |
| Human-AI co-processing                  | Dual-Substrate Cognition Architecture trilogy       | `10.5281/zenodo.21362260` |
| Context window architecture             | The Context Oscillator                              | `10.5281/zenodo.21811408` |
| AGI as system property                  | The Profile of a Person That Is AGI                 | `10.5281/zenodo.21921714` |
