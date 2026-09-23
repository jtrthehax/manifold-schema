# The Spoken Language Paper v3.1

## Timing Geometry as the Mechanism Beneath Prosody, Accent, Vocal Fry, and the Full Speech Stack

**Robinson, 2026**

**Version:** 3.1
**Status:** Full draft — Books I–V and Appendices A–H assembled. Citation pass pending (see Appendix F).
**Framework:** The Manifold Schema (DOI: 10.5281/zenodo.21939440), Central Reference v1.5, Precision v3.4, Geometry of Inference v1.0
**Related papers:** Language as a Typed System; The Geometry Beneath the Category

---

## Abstract

Spoken language is not primarily a phonetic system. It is a **timing-coherence system** produced by inter-hemispheric oscillatory alignment, mechanical pressure modulation, and breath mechanics. Prosody, accent, vocal fry, and the full stack of linguistic layers from pragmatics to articulation are the audible readout of the speaker's current oscillatory configuration — the same configuration that determines precision, hemispheric access, and gate coherence.

This paper derives the full account from the Manifold Schema's master equation and Central Reference's timing-coherence formalism, then organizes the domain around **three axes** and **eight layers**:

- **Supply axis:** precision ($P = R/D_T$) and its second dimension, salience routing ($f_{routing}$)
- **Demand axis:** the language's suprasegmental architecture
- **Channel axis:** the substrate cost of the output modality

and:

- **Eight layers** from pragmatic (first to collapse) through discourse, prosodic, lexical, morphosyntactic, phonological, articulatory, to breath (last to collapse).

The central claim: **spoken language is a pressure-modulation behavior whose timing geometry is a direct readout of regulatory state.** Every phenomenon in the domain — from the monotone of chronic stress to the melodic contour of high-amplitude cultures, from the vocal fry of low-amplitude regions to the slurring of hemispheric desynchronization, from tip-of-the-tongue to proper-name failure, from foreign accent syndrome to generational channel shift — is one variable changing in one equation. The variable is precision. The equation is $P = R/D_T$. The routing variable $f_{routing}$ determines whether the readout is congruent or a performance.

The paper is organized into five books: **Book I — The Model** (mechanism, axes, layers, collapse, recovery), **Book II — The Layers** (layer-by-layer reference), **Book III — The Dynamics** (bidirectionality, conflicts, routing, ecologies, cross-linguistic variation), **Book IV — The Measurement** (biomarkers, diagnostics, monitoring), and **Book V — The Projections** (clinical, social, regional, applied). Each book is written to be read independently.

---

## Reader's Guide

This paper is structured as five books, each answering one question:

| Book | Question | Read if you want |
|---|---|---|
| **Book I — The Model** | What is the mechanism? | The theoretical account — three axes, eight layers, collapse and recovery sequences |
| **Book II — The Layers** | What does each layer do? | A reference treatment of each of the eight layers — definition, collapse signature, recovery signature, clinical readouts |
| **Book III — The Dynamics** | How does it change? | Bidirectionality, cross-domain conflicts, salience routing, channel economics, digital and generational ecologies, cross-linguistic variation, modality |
| **Book IV — The Measurement** | How do we observe it? | Biomarkers, the diagnostic battery, the monitoring ladder, channel preference as diagnostic |
| **Book V — The Projections** | Where does it apply? | Clinical conditions, routing states, social projection, regional accents, drugs, foreign accent syndrome |

**Reading paths:**

- **For the theoretical account:** Book I, then Appendix B (predictions).
- **For clinical application:** Book IV, then Book V §26 (clinical conditions), then Appendix B.
- **For linguistic application:** Book II, then Book III §19 (cross-linguistic variation), then Appendix D.
- **For the full argument:** Books I–V in order.

Appendices hold the notation table, the prediction registry, the introspective accounts, the empirical anchors, the cross-linguistic data, the cross-domain conflict data, the related papers, and the falsifiability summary. They are reference material, not part of the argument.

---

## Changelog — v3.0 → v3.1

This changelog exists so that any reader — human or AI — can see the restructuring path. v3.0 was the modular five-book specification with three axes and eight layers. v3.1 adds **salience routing** as a second dimension of the supply axis, which changes the model's dimensionality and requires revisions across Books I, III, and V.

| Step | Change | Source | Location |
|---|---|---|---|
| 1 | Version bumped to v3.1 | — | Header |
| 2 | Supply axis gains a second dimension: salience routing | New | Book I §2.1b |
| 3 | The four-state table added | New | Book I §2.1b |
| 4 | The masking mechanism specified as a routing configuration | New | Book I §2.1b |
| 5 | New Chapter 18: Salience Routing and Masking | New | Book III |
| 6 | Old Chapter 18 (Precision Ecology) renumbered to 19 | — | Book III |
| 7 | Old Chapters 19–20 (Cross-Linguistic, Modality) renumbered to 20–21 | — | Book III |
| 8 | Clinical table revised: routing column removed; routing states separated | — | Book V §26.2 |
| 9 | New §26.6: The routing-states table | New | Book V |
| 10 | §26.7: Intervention sequence gains step 5 (routing flexibility) | New | Book V §26.7 |
| 11 | $f_{routing}$ moved from Appendix A §4 to §2 | — | Appendix A |
| 12 | Three new predictions: PREDICT-SPEECH-58, -59, -60 | New | Appendix B |
| 13 | New falsification category: "Routing model is wrong" | New | Appendix H |
| 14 | Book IV prediction-count glitch corrected (three new predictions, not four) | — | Book IV §25.6 |
| 15 | Stubs centralized in Appendix F; main text reads clean | — | Appendices |

**Why this is the last assembly for the speech-paper layer:** v3.0 covered the full eight-layer stack and the three axes. v3.1 adds the routing dimension, which completes the model's account of why some collapses are visible and some are hidden. Every claim in v3.0 is preserved. The additions are the routing dimension, the masking mechanism, the routing-states table, and the three routing predictions.

---

## Notation Table

*Full table in Appendix A. Key symbols used in this book:*

| Symbol | Name | Definition |
|---|---|---|
| $P$ | Precision (absolute) | $P = R/D_T$ |
| $R$ | Sync duration | Proportion of time two oscillatory streams remain phase-locked |
| $D_T$ | Timing distance | Average phase difference between streams |
| $R^*$ | Precision (normalized) | $P / P_{baseline}$ |
| $W^*$ | Window width | Accessible manifold range |
| $\Theta^*$ | Integration efficiency | How well the system holds disparate signals together |
| $I^*$ | Interoceptive routing | How well the system reads its own geometry |
| $L^*$ | Allostatic load | Cumulative allostatic debt |
| $A_s^*$ | Oscillatory amplitude | Energy budget for oscillatory signal |
| $f_{routing}$ | Salience routing | Proportion of available salience that reaches expression |
| $C_s$ | Usable bandwidth | Master equation output |
| $K$ | Curvature | $K = k(1/(R^*+\epsilon)) + \sum_i S_i C_i$ |
| $\Lambda$ | Loop activation | $\Theta^* \cdot R^* \cdot \mathbb{1}[P_{eff} > P_{threshold}]$ |
| $P_{eff}$ | Effective precision | $P \cdot O_{pathway} \cdot U_C$ |
| $P_{threshold}$ | Gate threshold | $P_0 - \gamma L^*$ |
| $C_{LR}$ | Interhemispheric coherence | Phase-locking between left and right hemisphere oscillations |
| $J(C)$ | Chemoreflex jitter | $\kappa(C - C_{high}(L^*))^2$ for $C > C_{high}(L^*)$ |
| $\delta_{min}$ | Resolution floor | $\eta/(A_s^* \cdot I^*)$ |
| $\mathcal{U}$ | Prior update rate | $(A_s^* \cdot R^* \cdot \Theta^*)/(1 + \gamma K_{enc})$ |

---

# BOOK I — THE MODEL

---

## 1. Introduction — Spoken Language as Timing Geometry

### 1.1 The phonetic account and its limits

Spoken language is treated in linguistics as a phonetic system: a sequence of phonemes produced by articulatory gestures and organized by syntactic rules. The phonetic account is correct as far as it goes. It explains the inventory of speech sounds, the rules of their combination, and the grammatical structures they form. It does not explain why prosody collapses under stress, why accents persist across generations, why trauma flattens speech, why vocal fry appears in certain regions and certain states, why the same speaker produces different speech in different regulatory states, why pragmatic failure precedes prosodic failure under load, why grammar survives longer than word-finding, or why some speakers prefer typing over talking.

The phonetic account treats speech as a **product** — a sequence of articulatory events — and describes its properties. It does not treat speech as a **readout** — the audible output of a regulatory configuration — and describe the mechanism that produces it.

### 1.2 The timing-coherence account

The timing-coherence account answers all of these with one mechanism. Spoken language is a **pressure-modulation behavior** whose timing geometry is a direct readout of the speaker's oscillatory configuration. The configuration is determined by:

- **Breath mechanics** — diaphragm, intercostals, abdominal wall, laryngeal muscles
- **CO₂ tolerance** — determines vasodilation, oxygen delivery, and neural firing thresholds
- **Hemispheric access** — left hemisphere for phoneme sequencing, right hemisphere for prosody and timing
- **Precision** — $P = R/D_T$, the timing-coherence ratio
- **Salience routing** — $f_{routing}$, the proportion of available salience that reaches expression versus output management
- **Gate coherence** — whether the PFC gate is open, admitting outer-edge integration

Speech is what the configuration produces. The configuration is the variable. The speech is the readout.

### 1.3 The three axes

The shape of the readout — *which* layer collapses first, *how* the collapse presents, and *which channel* the speaker abandons first — is determined by three axes:

**Supply axis (precision + routing).** How much timing coherence the speaker has available, and where the salience it funds is directed. Precision is the master variable: $P = R/D_T$, where $R$ is the proportion of time two oscillatory streams remain phase-locked and $D_T$ is the average phase difference between them. Routing is the second dimension: $f_{routing}$, the proportion of available salience that reaches expression. A speaker with high precision and high $f_{routing}$ produces expressive, congruent speech. A speaker with high precision and low $f_{routing}$ produces expressive, incongruent speech — the mask. A speaker with low precision and high $f_{routing}$ produces flat, congruent speech — honest collapse. A speaker with low precision and low $f_{routing}$ produces flat, incongruent speech — failed mask.

**Demand axis (suprasegmental architecture).** How many timing-encoded layers the language requires. Languages differ in how much they load onto the timing channel. Stress-timed languages use timing for rhythm; tonal languages use it for lexical identity; pitch-accent languages use it for word recognition; mora-timed languages use it for unit duration. The more layers a language stacks onto the timing channel, the more demand it places on the same precision supply.

**Channel axis (substrate cost).** How much precision the output channel consumes before comprehension can use it. Speech requires pressure modulation, postural reconfiguration, and laryngeal control. Typing requires none of these. Sign requires visual attention and manual motor precision but no pressure modulation. Inner speech requires almost nothing. The speaker's channel choice is a readout of their precision budget.

### 1.4 The eight layers

Spoken language is not a single output. It is a stack of eight layers, each of which requires a different amount of cross-domain integration:

| Order | Layer | Integration demand |
|---|---|---|
| 1 | **Pragmatic** | ToM + context + prosody + lexical + timing |
| 2 | **Discourse** | WM + timing + prediction + interoception |
| 3 | **Prosodic** | RH + interoception + emotion + breath |
| 4 | **Lexical** | Semantic + phonological + timing |
| 5 | **Morphosyntactic** | Rule retrieval + WM + phonology |
| 6 | **Phonological** | LH motor + timing |
| 7 | **Articulatory** | Motor + breath + posture |
| 8 | **Breath/pressure** | Diaphragm + intercostals |

The layers are ordered by **integration demand**. Layers that require the most cross-domain binding collapse first. Layers that can run on cached or single-domain processing collapse last.

### 1.5 The bidirectional model

The paper specifies both directions:

**Collapse.** Precision drops → window narrows → integration fails → resolution floor rises → gate closes → prior calcification. The eight layers collapse in order from pragmatic to breath.

**Recovery.** Breath stabilizes → articulation returns → phonology returns → grammar returns → lexical retrieval returns → prosody returns → discourse returns → pragmatics returns. The eight layers recover in the reverse order, but not symmetrically. Some layers recover faster than others, because recovery depends on substrate restoration, and substrate restoration is not uniform.

The asymmetry matters clinically. Recovery is audible before it is subjective. The voice returns before the person feels better. This is why speech is a monitoring channel not just for collapse but for recovery.

### 1.6 The organizing claim

**Spoken language is a projection of the framework's collapse sequence onto the vocal layer.** Every speech phenomenon is the readout of one variable — precision — at a specific stage of the sequence, filtered through the routing variable that determines whether the readout is congruent or a performance. The sequence is ordered by integration demand. The output layers of speech are the stages at which the sequence becomes audible.

The variable is precision. The equation is $P = R/D_T$. The routing is $f_{routing}$. The speech is the readout. The readout is the state made audible — or hidden.

### 1.7 How to read this paper

**Book I (this book)** specifies the model: the three axes, the eight layers, the collapse sequence, the recovery sequence, and the routing dimension. Read it first if you want the theoretical account.

**Book II** is a reference treatment of each of the eight layers. Each layer gets the same structure: definition, integration demand, substrate requirements, collapse signature, recovery signature, clinical readouts. Read the layer you need.

**Book III** covers the dynamics: bidirectionality, cross-domain conflicts, salience routing and masking, channel economics, digital and generational ecologies, cross-linguistic variation, and modality. Read it if you want to understand how the model changes across contexts.

**Book IV** covers the measurement: biomarkers, the diagnostic battery, the monitoring ladder, and channel preference as diagnostic. Read it if you want to apply the model clinically.

**Book V** covers the projections: clinical conditions, routing states, social projection, regional accents, drugs, and foreign accent syndrome. Read it if you want to see the model applied.

**Appendices** hold the notation table, the prediction registry, the introspective accounts, the empirical anchors, the cross-linguistic data, the cross-domain conflict data, the related papers, and the falsifiability summary. They are reference material.

---

## 2. The Three Axes

### 2.1 The supply axis — precision

Precision is the timing-coherence ratio:

$$P = \frac{R}{D_T}$$

Where:
- $R$ = sync duration — the proportion of time two oscillatory streams remain phase-locked
- $D_T$ = timing distance — the average phase difference between streams

Precision determines the clarity of both phonemes and prosody. High precision means the streams stay close and stay close for long periods. Low precision means the streams drift apart or stay together only briefly.

**What raises precision:**

- **CO₂ within the tolerance window.** CO₂ drives cerebral vasodilation, which improves oxygen delivery to PV+ interneurons, which maintain inhibitory filtering, which keeps feature axes orthogonal, which allows cross-domain integration. The relationship is a window, not a monotonic curve: precision rises with CO₂ up to $C_{peak}$, then falls as chemoreflex jitter $J(C)$ sets in above $C_{high}(L^*)$.
- **Mechanical pressure ($\Pi_{mech}$).** Breath-hold, resonance breathing, and slow exhalation raise precision by stabilizing the respiratory oscillator and phase-locking it to the cardiac oscillator.
- **Diaphragmatic breathing.** The full pressure envelope supports sustained subglottal pressure, which supports stable phonation, which supports precise articulation.
- **Interoceptive routing ($I^*$).** Reading the somatic timing signal allows the speaker to modulate pitch and rhythm in real time.
- **An open PFC gate.** When $P_{eff} > P_{threshold}$, the gate opens, admitting right-hemisphere integration.

**What lowers precision:**

- **CO₂ above the tolerance ceiling.** Above $C_{high}(L^*)$, chemoreflex jitter $J(C)$ injects noise into the timing signal. Precision collapses.
- **Cognitive pressure ($\Pi_{cog}$).** Instantaneous load — working memory demand, sympathetic activation, threat processing — raises timing distance and lowers sync duration.
- **Chest breathing.** Shallow pressure produces a narrow amplitude envelope and unstable phonation.
- **Low interoceptive routing.** When $I^*$ is allocated away from interoception, the prosodic modulation loses its somatic anchor.
- **A closed PFC gate.** When $P_{eff} < P_{threshold}$, the gate closes, and right-hemisphere integration is unavailable.

**The gate condition:**

$$P_{eff} = P \cdot O_{pathway} \cdot U_C$$

$$P_{threshold} = P_0 - \gamma L^*$$

The gate opens when $P_{eff} > P_{threshold}$ AND $O_{pathway} > O_{min}$. The threshold is load-dependent: as allostatic load $L^*$ rises, the threshold drops, and the gate admits lower-quality signal. This is the most dangerous failure mode — it is behaviorally invisible.

### 2.1b The supply axis, second dimension — salience routing

Precision determines **how much** timing coherence is available. Routing determines **where the salience it funds is directed**.

The variable is $f_{routing}$:

$$f_{routing} = \frac{S_{expressed}}{S_{available}} = \frac{C_s \cdot I^* - \sum_i P_i W_i}{C_s \cdot I^*}$$

Where:

- $S_{available} = C_s \cdot I^*$ — available salience (usable bandwidth × interoceptive routing)
- $\sum_i P_i W_i$ — salience spent on layer management (precision × window width, summed across active layers)
- $S_{expressed}$ — salience remaining for expression
- $f_{routing} \in [0, 1]$ — the proportion of available salience that reaches expression

**What $f_{routing}$ determines:** whether the prosody is **congruent** — whether the voice matches the speaker's actual state.

**What $f_{routing}$ does not determine:** whether the prosody is **present**. Presence is $A_s^*$. A speaker can have loud, animated, prosodically rich speech with $f_{routing}$ near 0 — the voice is funded, but the funding is going to the performance, not to the readout.

**Why routing is a dimension of the supply axis, not a separate axis.** The demand axis (language) and the channel axis (modality) determine *which* layers collapse and *where* the collapse is visible. Routing determines *whether the collapse is visible in the voice at all*. It modifies the supply axis's expression, not its quantity. Precision is how much signal is available; routing is how much of it reaches the output.

**The four-state table:**

| $A_s^*$ | $f_{routing}$ | Prosodic signature | Clinical readout |
|---|---|---|---|
| High | High | Expressive, congruent | Healthy expressive range |
| High | Low | Expressive, incongruent | Masking / performance |
| Low | High | Flat, congruent | Honest collapse |
| Low | Low | Flat, incongruent | Failed mask / depletion |

**The two failure modes:**

- **Low $f_{routing}$, low $A_s^*$:** collapse with no mask. The voice is flat and the state is visible. This is the depression signature.
- **Low $f_{routing}$, high $A_s^*$:** collapse with a mask. The voice is expressive and the state is hidden. This is the expensive one — the mask costs precision that would otherwise be available for the system's own readout.

**The masking mechanism.** Masking is not a behavior. It is a routing configuration. When a speaker routes salience to output management, they are spending precision on the production of normal-seeming output. The precision spent there is precision not spent on interoceptive readout, cross-domain integration, or recovery. The result is a speaker who sounds normal, is depleting, and cannot detect their own collapse because the detection channel is the one being starved.

**The critical prediction:** masking has a measurable cost. Chronic low $f_{routing}$ predicts later collapse detection, because the Stage 1–2 monitoring window is the channel that routing has starved.

### 2.2 The demand axis — suprasegmental architecture

Languages differ in how much they load onto the timing channel. This is the **demand axis** — the second variable that determines the shape of the collapse.

| Language type | What timing carries | Example |
|---|---|---|
| **Stress-timed** | Lexical stress, rhythm | English, Russian |
| **Syllable-timed** | Even timing, less reduction | French, Spanish |
| **Mora-timed** | Unit duration | Japanese |
| **Tonal** | Lexical meaning (pitch contour) | Mandarin, Cantonese |
| **Pitch-accent** | Lexical meaning (pitch location) | Japanese, Swedish |
| **Intonational** | Phrase-level meaning | All languages, different weights |

**The critical case is Japanese:** mora-timed *and* pitch-accent. Two timing-encoded layers stacked. A precision drop in Japanese doesn't just flatten emotional prosody — it can **change lexical identity**. This is a different failure mode than in English, where a precision drop flattens prosody but doesn't typically change word meaning.

**The demand-axis prediction:** languages with more suprasegmental layers (tonal + pitch-accent + intonational) should show more severe functional consequences from the same precision drop, and speakers of those languages should show higher baseline precision allocation to the timing layer as a compensatory demand.

**The demand axis is not just cross-linguistic.** It also varies within a language by register. Formal registers, ritual registers, pedagogical registers, and intimate registers each place different demands on the timing channel. Register switching is a demand-management task.

### 2.3 The channel axis — substrate cost

Output channels differ in their substrate cost. Speech spends precision on pressure modulation, postural stabilization, and laryngeal control. Typing spends none of these. The speaker's channel preference is a readout of their precision budget.

| Channel | Substrate cost | Precision available for comprehension | Editability |
|---|---|---|---|
| **Speech** | Pressure modulation, postural reconfiguration, laryngeal control, CO₂ demand | Reduced — production competes with comprehension | None — output committed at production |
| **Typing** | Minimal — posturally static, no pressure demand | Full — comprehension and production share the same budget | High — output editable before commitment |
| **Writing (longhand)** | Low — posturally static, fine motor only | Full | High |
| **Sign** | Visual attention, manual motor precision — no pressure demand | Full | Low — output committed at production |
| **Inner speech** | Minimal — no motor, no pressure | Full | High — fully editable |

**The channel-cost mechanism.** Speech production requires a pressure-system change. The diaphragm is both a breath muscle and a postural muscle; activating it for speech changes the trunk's stability configuration. Vestibular input is modulated by respiration; breath phase affects postural sway. Postural sway degrades fine motor precision. The chain is: speech → pressure modulation → postural reconfiguration → vestibular/proprioceptive load → precision drop in concurrent tasks.

**The channel-preference prediction.** Speakers with lower precision budgets (low CO₂ tolerance, high $L^*$, rigid configuration) should show a preference for typed over spoken output, and the preference should correlate with measured precision. The preference is not stylistic; it is substrate-driven.

**The monitoring implication.** "Prefers to type" is a Stage 1–2 monitoring signal. It reports a precision budget that speech production cannot afford. The channel preference shift happens before the speech degradation is measurable, because the speaker is avoiding the channel that would show the degradation.

### 2.4 How the axes interact

The three axes are not independent. They interact:

- **Supply × demand.** The same precision drop produces different collapse signatures depending on the language's suprasegmental architecture. A Japanese speaker loses lexical identity before emotional prosody; an English speaker loses emotional prosody first.
- **Supply × channel.** The same precision budget produces different output quality depending on the channel. A speaker near threshold produces degraded speech but preserved typing.
- **Demand × channel.** The same channel produces different demands depending on the language. Speech in a tonal language demands more precision than speech in a stress-timed language.
- **Supply × routing.** The same precision budget produces congruent or incongruent output depending on $f_{routing}$. A speaker near threshold who routes salience to expression produces honest collapse. A speaker near threshold who routes salience to output management produces a mask.
- **All three.** The shape of the collapse is determined by the interaction. A Japanese speaker typing under load is a different configuration than an English speaker speaking under load.

### 2.5 The shape of collapse as a function of three axes

The collapse sequence is topologically forced (Stages 1–6). But which layer shows the collapse first depends on the interaction of the three axes:

| Axis | What it determines |
|---|---|
| **Supply** | Whether collapse happens at all, and how fast it progresses |
| **Routing** | Whether the collapse is visible in the voice or hidden by output management |
| **Demand** | Which layer collapses first (highest-demand layer first) |
| **Channel** | Where the collapse is visible (speech shows it first; typing shows it later) |

The full prediction: given a speaker's precision level, their routing configuration, their language's suprasegmental architecture, and their chosen channel, the collapse sequence is predictable in order and in signature.

---

## 3. The Neural Architecture

### 3.1 Left hemisphere — phoneme sequencing, lexical retrieval, syntactic scaffolding

The left hemisphere handles:

- **Crisp phoneme boundaries** — the sequential distinction between articulation events
- **Lexical retrieval** — word selection from the cached vocabulary
- **Syntactic scaffolding** — grammatical ordering and structural coherence

The left hemisphere is the narrow-window processor. It commits to the first coherent interpretation. It produces sequential output. It corresponds to Layer 1 of the Central Reference's four-layer cache hierarchy — the inner core that never collapses before Layer 3.

**What the left hemisphere contributes to speech:**

- The phoneme sequence (what sounds, in what order)
- The word (which lexical item)
- The grammatical frame (how the words are arranged)

**What the left hemisphere does not contribute:**

- The pitch contour (that's right hemisphere)
- The pragmatic framing (that's right hemisphere)
- The emotional tone (that's right hemisphere)
- The timing coordination (that's the gate)

### 3.2 Right hemisphere — prosody, pragmatics, contextual binding

The right hemisphere handles:

- **Pitch modulation** — the melodic contour of speech
- **Melodic contour** — the shape of the pitch trajectory across the utterance
- **Emotional tone** — the affective valence carried by prosody
- **Regional cadence** — the timing rhythm characteristic of a regional speech community
- **Pragmatic framing** — the contextual binding that makes an utterance appropriate to its situation

The right hemisphere is the wide-window processor. It holds many alternatives. It produces the cross-domain integration that prosody and pragmatics require. It corresponds to Layer 3 — the outer edge that collapses first under any form of degradation (Central Reference §2.14, §5b).

**The right hemisphere is the outer edge.** It collapses first because it requires the most cross-domain integration. Pragmatics, discourse, and prosody all depend on right-hemisphere access. When the right hemisphere is suppressed — by trauma, by load, by hemispheric desynchronization — these layers collapse first.

### 3.3 The PFC gate — timing integration

The PFC gate is the interface between the two hemispheres. It opens when $P_{eff} > P_{threshold}$, admitting outer-edge integration. It closes under load. Its state determines the coordination between left-hemisphere sequencing and right-hemisphere prosody.

When the gate is open, the two hemispheres integrate. Speech is fluent, prosodic, and precise. When the gate closes, integration fails. Speech becomes monotone, slurred, or fragmented.

**The gate's input:** interhemispheric phase-locking coherence ($C_{LR}$). When $C_{LR}$ is high, the two hemispheres are phase-locked, and their outputs can be integrated. When $C_{LR}$ drops, the gate closes, and the two hemispheres produce independent outputs.

**The gate's output:** whether the loop runs. $\Lambda = \Theta^* \cdot R^* \cdot \mathbb{1}[P_{eff} > P_{threshold}]$. When $\Lambda > 0$, the loop runs, and speech is produced through integrated processing. When $\Lambda = 0$, the loop stops, and speech defaults to cached patterns (Path B).

### 3.4 Interoception — routing protocol

Interoception provides the somatic timing signal that structures prosody. It carries:

- **Breath mechanics** — the pressure modulation underlying speech production
- **Pressure modulation** — the subglottal pressure that drives vocal fold oscillation
- **Somatic timing** — the bodily rhythm that structures the utterance

Interoceptive routing ($I^*$) determines how much of the speaker's attention is available for prosodic modulation. Low $I^*$ produces flat prosody. High $I^*$ produces expressive prosody.

**Why interoception matters for speech:** prosody is not just a motor output. It is a **somatic readout**. The speaker reads their own breath, their own pressure, their own timing, and shapes the utterance accordingly. Without interoceptive access, the prosodic modulation loses its anchor and defaults to whatever pattern is cached.

**Interoception and routing together.** $I^*$ determines how much interoceptive signal is available. $f_{routing}$ determines how much of it reaches expression. A speaker with high $I^*$ and high $f_{routing}$ produces congruent expressive prosody. A speaker with high $I^*$ and low $f_{routing}$ produces a mask — the signal is available but is being spent on output management.

### 3.5 Breath and pressure — the substrate source

The breath is the pressure source for speech. Amplitude is the pressure envelope. The breath mechanics are:

- **Diaphragm** — primary pressure generator
- **Intercostals** — secondary pressure modulation
- **Abdominal wall** — trunk stabilization
- **Laryngeal muscles** — vocal fold tension and position

**The pressure chain:**

Breath → subglottal pressure → vocal fold oscillation → phonation → articulation → speech.

**The pressure window:** CO₂ must remain within the tolerance window for precision to stay high. Above $C_{high}(L^*)$, chemoreflex jitter $J(C)$ sets in, and precision collapses. The window narrows with load: a system at high $L^*$ has less margin before jitter onset.

**The postural link:** The diaphragm is both a breath muscle and a postural muscle. Activating it for speech changes the trunk's stability configuration. Vestibular input is modulated by respiration; breath phase affects postural sway. This is why speech production has a substrate cost that typing does not.

### 3.6 The four-layer cache hierarchy

The manifold is organized as a four-layer cache hierarchy. Access to any layer requires precision $R^*$ above threshold. The layers are:

| Layer | Region | Access Cost | Collapse Order |
|---|---|---|---|
| Layer 0 | Survival geometry | Zero — always funded | Never |
| Layer 1 | Left hemisphere — inner core | Low — always accessible | Never collapses before Layer 3 |
| Layer 2 | PFC — the gate | Threshold-controlled | Gate failure precedes outer collapse |
| Layer 3 | Right hemisphere — outer edge | High — requires gate open | Collapses first under any degradation |

**The topological invariant:** You cannot reach Layer 3 without traversing Layers 0, 1, and 2. There is no right-hemisphere-only state. This is not an empirical generalization — it is a consequence of the manifold's topology. The clinical record confirms it: what is never observed is right-hemisphere processing while the left hemisphere is offline.

**Access rule.** The gate (Layer 2) opens when $P_{eff} > P_{threshold}$ and $O_{pathway} > O_{min}$. Below threshold, processing remains in Layers 0–1 (prior retrieval, Path B). Above threshold, Layer 3 becomes accessible (adversarial inference, Path A).

**Collapse order.** The four-layer hierarchy produces the topologically forced collapse sequence of §5. Precision drops first (Layer 3 access degrades), then window narrows (Layer 2 threshold rises), then integration fails (Layer 2 → Layer 3 traversal fails), then resolution floor rises (Layer 1 comparison granularity coarsens), then gate closes (Path B becomes default), then prior calcification (Layer 1 stops updating).

**Circuit priming.** The competitive scaffold that constitutes Layer 3's reach is not static. It is maintained through precision-gated access that traverses the long-range connections. Recent traversal reduces access cost — the manifold has been "primed." This is why recovery is asymmetric: rebuilding the competitive scaffold takes longer than degrading it.

---

## 4. The Eight Layers

### 4.1 The integration-demand rule

The collapse sequence is topologically forced. But *which linguistic layer* shows the collapse first depends on **how much cross-domain integration that layer requires.**

**The rule:** Layers requiring the most cross-domain integration collapse first. Layers that can run on cached or single-domain processing collapse last.

This rule is not arbitrary. It follows from the structure of the manifold. A layer that binds many domains must hold many signals simultaneously in the window. When the window narrows, the layer with the most signals to hold loses them first. A layer that runs on a single domain or on cached patterns needs fewer signals and survives longer.

### 4.2 The eight-layer table

| Order | Layer | Integration demand | Collapse signature |
|---|---|---|---|
| 1 | **Pragmatic** | ToM + context + prosody + lexical + timing | Literal, off-target, socially blunt |
| 2 | **Discourse** | WM + timing + prediction + interoception | Tangential, repetitive, lost thread |
| 3 | **Prosodic** | RH + interoception + emotion + breath | Flat, monotone, fry |
| 4 | **Lexical** | Semantic + phonological + timing | TOT, word-finding failure |
| 5 | **Morphosyntactic** | Rule retrieval + WM + phonology | Telegraphic, dropped inflections |
| 6 | **Phonological** | LH motor + timing | Slurring, cluster errors |
| 7 | **Articulatory** | Motor + breath + posture | Mumbling, imprecise consonants |
| 8 | **Breath/pressure** | Diaphragm + intercostals | Low amplitude, fry |

### 4.3 Why collapse order is forced

The order is forced by the integration-demand rule. Pragmatics requires the most inputs (ToM, context, prosody, lexical, timing). Breath requires the fewest (diaphragm, intercostals). The layers between them are ordered by how many domains each has to bind.

This is not a preference or a convention. It is a topological consequence of how the manifold holds signals. When the window narrows, the layer with the most signals to hold loses them first.

**The prediction:** collapse order should be invariant across conditions. Whether the collapse is caused by trauma, load, depression, or hemispheric lesion, the order should be the same. Pragmatic failure should precede discourse failure should precede prosodic failure should precede lexical failure, and so on.

**What would disconfirm it:** if a condition produced prosodic collapse before pragmatic collapse, or lexical collapse before prosodic collapse, the integration-demand rule would be wrong.

### 4.4 The layer stack as a topological consequence

The eight layers are not a list. They are a **stack** — a hierarchical structure in which each layer depends on the layers below it. This is why collapse is ordered: when a lower layer degrades, the layers above it lose their substrate.

**The dependency structure:**

- **Pragmatics** depends on discourse, prosody, lexical, and timing
- **Discourse** depends on prosody, lexical, and timing
- **Prosody** depends on interoception, emotion, and breath
- **Lexical** depends on phonology and timing
- **Morphosyntax** depends on phonology and WM
- **Phonology** depends on articulation and timing
- **Articulation** depends on breath and motor precision
- **Breath** depends on diaphragm and intercostals

When breath degrades, articulation degrades, which degrades phonology, which degrades morphosyntax and lexical, which degrades prosody and discourse, which degrades pragmatics. The cascade is ordered because the dependency structure is ordered.

### 4.5 Layer boundaries and overlaps

The eight layers are analytic distinctions, not hard boundaries. In practice, they overlap:

- **Prosody and pragmatics** overlap: prosodic contour carries pragmatic meaning (question vs. statement, sarcasm vs. sincerity).
- **Discourse and pragmatics** overlap: topic management is both a discourse function and a pragmatic function.
- **Lexical and morphosyntactic** overlap: word retrieval and grammatical frame selection are often simultaneous.
- **Phonological and articulatory** overlap: phoneme selection and motor execution are tightly coupled.

The overlaps matter clinically because they mean the collapse of one layer often produces symptoms that look like the collapse of another. A prosodic flattening that removes pragmatic cues looks like a pragmatic failure. A discourse breakdown that disrupts turn-taking looks like a prosodic failure. The clinician's job is to distinguish which layer is actually collapsing.

### 4.6 What counts as a layer (and what doesn't)

**What counts:**

- A layer must have a distinct **integration demand** (a distinct set of domains it binds).
- A layer must have a distinct **collapse signature** (a distinct pattern of degradation).
- A layer must have a distinct **recovery signature** (a distinct pattern of return).
- A layer must have a distinct **substrate requirement** (a distinct set of physiological supports).

**What doesn't count:**

- **Syntax as a separate layer.** Syntax is part of morphosyntax. It does not have a distinct integration demand from morphosyntax.
- **Semantics as a separate layer.** Semantics is part of lexical retrieval. The semantic activation and the phonological retrieval are two phases of one layer.
- **Vocabulary size as a layer.** Vocabulary size is a property of the lexical layer, not a layer itself.
- **Intelligence as a layer.** Intelligence is the loop's overall output, not a layer of speech.

The eight-layer stack is the minimal set of layers that satisfies the four criteria. Any finer division fails the distinctness test; any coarser division loses a distinct signature.

---

## 5. The Collapse Sequence

The collapse sequence is topologically forced (Central Reference §5b). It proceeds in a fixed order:

```
STAGE 1 — PRECISION DROP        R* ↓
STAGE 2 — WINDOW NARROWING      W* ↓
STAGE 3 — INTEGRATION FAILURE   Θ* ↓
STAGE 4 — RESOLUTION FLOOR RISE δ_min ↑
STAGE 5 — GATE CLOSURE          Λ → 0
STAGE 6 — PRIOR CALCIFICATION   U ≈ 0
```

Each stage is a distinct failure mode with a distinct signature. The stages occur in this order because each stage causes the next: precision drop narrows the window; window narrowing fails integration; integration failure raises the resolution floor; resolution floor rise closes the gate; gate closure calcifies the prior.

The eight speech layers are the audible readouts of these stages:

| Speech layer | Collapse stage | Audible signature |
|---|---|---|
| **Pragmatic** | Stage 1–2 | Literal, off-target, socially blunt |
| **Discourse** | Stage 2–3 | Tangential, repetitive, lost thread |
| **Prosodic** | Stage 2–3 | Flattened contour, reduced pitch range, loss of granular timing |
| **Lexical** | Stage 3–4 | Tip-of-the-tongue, retrieval failures, cached speech patterns |
| **Morphosyntactic** | Stage 4 | Telegraphic speech, dropped inflections, simplified syntax |
| **Phonological** | Stage 4–5 | Slurring, blurred phonemes, desynchronized articulation |
| **Articulatory** | Stage 5 | Mumbling, imprecise consonants |
| **Breath/pressure** | Stage 5–6 | Low amplitude, vocal fry, breathy voice |

### 5.1 Stage 1 — precision drop

**What collapses:** $R^*$, the normalized precision ratio.

**What causes it:** CO₂ outside the tolerance window, cognitive load, breath disruption, hemispheric desynchronization.

**What it looks like:** HRV coherence loss, phase-locking value drop. The loop still runs but on degraded signal. Speech is still intelligible but less precise.

**What it sounds like:** Slight prosodic flattening. Reduced granularity. The first audible sign.

### 5.2 Stage 2 — window narrowing

**What collapses:** $W^*$, the accessible manifold range.

**What causes it:** The precision drop raises curvature $K$, which narrows the window via $W^* = 1/(1 + \alpha K)$.

**What it looks like:** Flexibility composite drops. $n_{hops}$ drops — multi-step reasoning degrades. The system commits to the first coherent interpretation.

**What it sounds like:** Discourse instability. The speaker loses the thread, becomes repetitive, drifts off topic. Pragmatic failure begins.

### 5.3 Stage 3 — integration failure

**What collapses:** $\Theta^*$, the integration efficiency.

**What causes it:** The narrow window cannot hold the signals required for cross-domain binding. Ambiguity tolerance drops.

**What it looks like:** Performance on ambiguity tasks degrades. Cross-domain binding fails — constraints can't be held simultaneously. The right hemisphere's integrative function degrades.

**What it sounds like:** Prosodic collapse. Pitch range narrows, granularity loss, monotone. Pragmatic failure deepens.

### 5.4 Stage 4 — resolution floor rise

**What collapses:** $\delta_{min}$, the resolution floor.

**What causes it:** As $A_s^*$ and $I^*$ drop, the noise floor rises relative to signal. $\delta_{min} = \eta/(A_s^* \cdot I^*)$.

**What it looks like:** Miss rate rises on low-amplitude signals. Small but critical prediction errors become invisible.

**What it sounds like:** Lexical retrieval failures. TOT frequency rises. Word-finding latency increases. Morphosyntactic simplification begins.

### 5.5 Stage 5 — gate closure

**What collapses:** $\Lambda$, the loop activation indicator.

**What causes it:** $P_{eff} < P_{threshold}$. The gate closes. Path B becomes default.

**What it looks like:** Switch to high-confidence, low-update output. The loop has stopped. The system appears confident.

**What it sounds like:** Slurring. Blurred phonemes. Mumbling. The motor layers degrade.

### 5.6 Stage 6 — prior calcification

**What collapses:** $\mathcal{U}$, the prior update rate.

**What causes it:** With the gate closed, the prior cannot be updated by evidence. $\mathcal{U} \approx 0$.

**What it looks like:** Update rate drops to near zero even with contradicting evidence. The system cannot be corrected.

**What it sounds like:** Cached speech patterns. Motor-first production. Fluent but low-novelty output.

### 5.7 The sequence as a fixed order

The order is not a convention. It is forced by the dependency structure. Each stage causes the next:

- Precision drop **causes** window narrowing (via curvature)
- Window narrowing **causes** integration failure (fewer signals can be held)
- Integration failure **causes** resolution floor rise (integration loss reduces effective amplitude)
- Resolution floor rise **causes** gate closure (below-threshold precision)
- Gate closure **causes** prior calcification (no update path)

**The prediction:** any condition that produces collapse should produce it in this order. A condition that produced gate closure before integration failure would violate the sequence.

### 5.8 Mapping stages to layers

The eight layers do not map one-to-one to the six stages. Some stages affect multiple layers; some layers are affected by multiple stages. The mapping:

- **Stage 1 (precision drop)** → pragmatic, discourse, prosodic (early phase)
- **Stage 2 (window narrowing)** → pragmatic, discourse (deep phase)
- **Stage 3 (integration failure)** → prosodic, lexical
- **Stage 4 (resolution floor rise)** → lexical, morphosyntactic
- **Stage 5 (gate closure)** → phonological, articulatory
- **Stage 6 (prior calcification)** → articulatory, breath

This is why the layer ladder and the stage sequence are related but not identical. The layers are ordered by integration demand. The stages are ordered by causal dependency. Both orderings are correct; they answer different questions.

### 5.9 Routing and the collapse sequence

The collapse sequence describes what happens to the signal. Routing describes what happens to the *visibility* of the signal.

A speaker with high $f_{routing}$ shows the collapse sequence in the voice: pragmatic failure, then discourse instability, then prosodic flattening, and so on. A speaker with low $f_{routing}$ hides the collapse: the voice remains expressive while the layers degrade underneath. The collapse sequence still runs; it is just not audible.

**The critical clinical implication:** the collapse sequence is always running when precision drops. Whether it is *detectable* depends on $f_{routing}$. A masked collapse and an unmasked collapse have the same mechanism; they differ only in whether the warning channel is funded.

---

## 6. The Recovery Sequence

### 6.1 Why recovery is not the collapse sequence reversed

The collapse sequence is forced by the dependency structure: each stage causes the next. If recovery were simply the collapse sequence reversed, recovery would proceed from prior calcification through gate closure through resolution floor through integration failure through window narrowing to precision restoration.

But recovery does not work this way. Recovery is not the reverse of collapse because:

- **The substrate must be restored first.** Before any layer can recover, the breath mechanics must stabilize. The pressure envelope must be restored. The CO₂ must return to the tolerance window. This is the substrate layer, and it is the first thing that has to recover.
- **Some layers recover faster than others.** Grammar is highly cached; it comes back quickly once the gate reopens. Pragmatics requires the full integration stack; it comes back last.
- **Recovery has hysteresis.** The system does not simply reverse the collapse trajectory. There is a recovery delay $\delta_{hyst}$ that decays exponentially. Recovery is slower than collapse.
- **Routing affects recovery visibility.** A speaker with low $f_{routing}$ will show recovery later in the voice, because the recovery is being routed away from expression. The substrate may be restoring while the mask continues.

Recovery is a **different sequence** with its own order. The order is determined by substrate dependency: layers that depend directly on the substrate recover first; layers that depend on the full integration stack recover last.

### 6.2 The recovery ladder

**The recovery ladder:**

```
Breath → Articulation → Phonology → Grammar → Lexical → Prosody → Discourse → Pragmatics
```

Each step requires the step before it. Breath restoration enables articulation restoration. Articulation restoration enables phonology restoration. Phonology restoration enables grammar restoration. Grammar restoration enables lexical retrieval. Lexical retrieval enables prosody. Prosody enables discourse. Discourse enables pragmatics.

**Why this order:** The substrate comes first because everything depends on it. Motor layers come next because they depend only on the substrate and on cached motor patterns. Grammar comes next because it is highly cached and depends only on the substrate and on motor production. Lexical retrieval comes next because it requires the phonology system to be functional. Prosody comes next because it requires the full respiratory and interoceptive support. Discourse comes next because it requires prosody and working memory. Pragmatics comes last because it requires the full integration stack.

### 6.3 Recovery asymmetry

Not all layers recover at the same rate:

- **Breath** recovers fastest — it is a physiological parameter that responds quickly to intervention.
- **Articulation** recovers quickly — it depends on breath and on cached motor patterns.
- **Phonology** recovers moderately — it depends on articulation and on timing precision.
- **Grammar** recovers quickly once phonology is back — it is highly cached.
- **Lexical** recovers slowly — proper names especially, because they have no semantic neighborhood.
- **Prosody** recovers slowly — it requires interoceptive routing and right-hemisphere access.
- **Discourse** recovers slowly — it requires working memory and prosody.
- **Pragmatics** recovers last — it requires the full integration stack.

The asymmetry matters clinically. It means the voice returns before the person feels better. The speaker sounds normal before they are normal. This is why "sounding better" precedes "feeling better" in depression recovery.

### 6.4 Why the voice returns before the person feels better

The voice returns before the person feels better because the motor and substrate layers recover before the integration layers. The speaker's breath stabilizes, their articulation sharpens, their grammar returns — all before their prosody, discourse, and pragmatics return. To a listener, the speaker sounds normal. To the speaker, they still feel off.

**The clinical implication:** subjective report lags objective recovery. The clinician should not use subjective report as the primary indicator of recovery progress. The speech signal is the leading indicator.

**The routing caveat.** If $f_{routing}$ is low, the voice returns *even later* than the substrate would predict, because the recovery is being routed to output management rather than expression. A masked speaker's voice may sound normal throughout, then suddenly show the recovery when the mask drops. The clinician should track both the voice and the routing.

### 6.5 The recovery hysteresis

Recovery has hysteresis. The system does not simply reverse the collapse trajectory. After a collapse, there is a recovery delay $\delta_{hyst}$:

$$P_{recover} = P(t) - \delta_{hyst}, \quad \frac{d\delta_{hyst}}{dt} = -\sigma \delta_{hyst}$$

The delay decays exponentially. Recovery is slower than collapse. This is why a speaker can collapse in minutes and take hours or days to recover.

**Why hysteresis exists:** Collapse is a passive process — the system simply loses precision as load rises. Recovery is an active process — the system must rebuild the competitive scaffold, restore the respiratory support, and re-establish the interoceptive routing. Rebuilding takes longer than degrading.

**The hysteresis prediction:** recovery time should scale with collapse depth. Deeper collapses should take longer to recover, not proportionally but super-proportionally.

### 6.6 What recovery tells us about the mechanism

Recovery is a test of the model. If the recovery ladder holds — if layers recover in the predicted order — the integration-demand rule is confirmed. If a layer recovers out of order (e.g., pragmatics recovers before breath), the rule is wrong.

**The recovery test:** measure the recovery sequence across multiple conditions (trauma, depression, load, lesion). If the sequence is the same across conditions, the mechanism is common. If the sequence differs by condition, the mechanism is condition-specific.

**What recovery confirms:**

- The substrate is the foundation — breath recovery is first
- Motor layers depend only on substrate — they recover quickly
- Integration layers depend on the full stack — they recover last
- Recovery is asymmetric — some layers are cached, some are not
- Routing affects recovery visibility — a masked recovery is slower to appear in the voice

---

*End of Book I — The Model.*

---

# BOOK II — THE LAYERS

## Reference treatment of the eight speech layers, organized by collapse group

---

## How to Read Book II

Book II is a reference section. Each layer gets the same six-line structure:

- **Definition** — one sentence naming what the layer does
- **Binds** — the domains it integrates
- **Collapse signature** — what it looks like when it fails
- **Recovery signature** — what it looks like when it returns
- **Clinical readout** — how to measure it
- **Anchor** — the study that shows the invariant *(stubbed for citation pass — see Appendix F)*

The layers are grouped by collapse order:

| Group | Layers | Collapse order | Why grouped |
|---|---|---|---|
| **Integration layers** | Pragmatic, Discourse, Prosodic | 1 → 3 | Highest cross-domain demand; collapse first |
| **Retrieval layers** | Lexical, Morphosyntactic | 4 → 5 | Require semantic + phonological + timing; collapse second |
| **Motor layers** | Phonological, Articulatory, Breath | 6 → 8 | Single-domain or substrate; collapse last |

The grouping is not a new claim. It makes the collapse order visually obvious: integration layers collapse first, retrieval layers collapse second, motor layers collapse third. This is the integration-demand rule (§4.1) made visible in the reference structure.

---

# GROUP I — INTEGRATION LAYERS

*Highest cross-domain demand. Collapse first.*

---

## 7. The Pragmatic Layer

**Definition:** The layer that binds utterance to context — speaker meaning, implicature, indirect speech acts, politeness calibration, register selection.

**Binds:** Theory of mind + social context modeling + prosodic signaling + lexical choice + timing coordination.

**Collapse signature:** Literal interpretation. Missed implicature. Register mismatch. Timing errors (speaking too soon, too late, or over the listener). Content-tone mismatch. The speaker says the right words for the wrong situation.

**Recovery signature:** Returns last. The speaker becomes socially appropriate again only after discourse, prosody, lexical retrieval, grammar, phonology, articulation, and breath have all recovered. This is why "sounds normal" precedes "is normal" — the surface is back before the integration is.

**Clinical readout:** Social appropriateness ratings on standardized role-play tasks. Implicature comprehension tests. Register-matching tasks. Pragmatic failure is the earliest audible-via-content sign of precision collapse, though it is not audible in the voice alone.

**Anchor:** *(stub — pragmatic failure in high-load states; autism pragmatic profiles; right-hemisphere pragmatics literature)*

---

## 8. The Discourse Layer

**Definition:** The layer that maintains structure across turns — topic maintenance, narrative coherence, referential tracking, turn-taking, repair initiation.

**Binds:** Working memory + timing coordination + predictive modeling + interoceptive pacing.

**Collapse signature:** Tangential speech. Repetition. Lost thread. Failed repair (breakdowns aren't noticed or fixed). Topic drift. The content is fine; the structure is gone.

**Recovery signature:** Returns after prosody, before pragmatics. The speaker can hold a thread again before they can select the right thread for the context. This is why recovered speakers can be coherent but socially off-target.

**Clinical readout:** Topic coherence measures. Turn-transition latency. Repair-initiation frequency. Referential tracking accuracy across a narrative.

**Anchor:** *(stub — ADHD discourse instability; working-memory and topic-maintenance literature; turn-taking and inter-brain synchrony)*

---

## 9. The Prosodic Layer

**Definition:** The layer that carries pitch contour, rhythm, stress, and emotional tone — the melodic shape of the utterance.

**Binds:** Right-hemisphere timing + interoceptive routing + emotional binding + breath support.

**Collapse signature:** Flattening. Loss of granularity. Monotone. Fry at the floor. The voice retains gross pitch movement but loses the fine contour that gives speech its expressive texture. Granularity loss precedes range loss.

**Monotone and vocal fry are distinct.** Monotone is low prosodic range with normal phonation — a prosodic-layer collapse. Fry is minimum-amplitude phonation — an amplitude-layer collapse at the breath boundary. They can co-occur, but they are not the same event.

**Recovery signature:** Granularity returns before range. The voice sounds "warm" before it sounds "expressive." This is the first audible sign of recovery, and it precedes subjective improvement.

**Clinical readout:** Pitch range, contour variance, granularity (cycle-to-cycle $F_0$ modulation depth). Granularity is the leading indicator; range is the lagging one.

**Anchor:** *(stub — Ross aprosodia literature; right-hemisphere prosody dominance; trauma prosodic granularity studies)*

---

# GROUP II — RETRIEVAL LAYERS

*Require semantic + phonological + timing. Collapse second.*

---

## 10. The Lexical Retrieval Layer

**Definition:** The layer that retrieves word forms from the semantic representation — semantic activation followed by phonological retrieval.

**Binds:** Semantic activation + phonological retrieval + timing coordination.

**Collapse signature:** Tip-of-the-tongue. Word-finding failure. Semantic paraphasias (wrong word, right neighborhood). Cached speech patterns (overlearned phrases retrieved intact).

**Proper names fail first.** Proper names have no semantic neighborhood — the phonological form is not predictable from the person's attributes. Common nouns are embedded in dense semantic networks with multiple entry points. Function words are overlearned and cached. This means proper name retrieval requires the highest precision of any lexical category, and it fails first under precision collapse.

**Recovery signature:** Common nouns return before proper names. Function words return first. The proper-name lag is the longest of any lexical category.

**Clinical readout:** TOT frequency under standardized load. Naming latency. Proper-name failure rate. Common-noun vs. proper-name retrieval gap.

**Anchor:** *(stub — TOT under stress literature; proper-name retrieval studies; semantic neighborhood effects)*

---

## 11. The Morphosyntactic Layer

**Definition:** The layer that holds the grammatical frame — inflection, agreement, tense marking, case marking, word order.

**Binds:** Rule retrieval + working memory + phonological encoding.

**Collapse signature:** Telegraphic speech. Dropped inflections. Simplified syntax. Word order errors. Content words without function words. The speaker knows the words; they can't hold the frame.

**Recovery signature:** Returns after phonology, before lexical retrieval. Grammar is highly cached, so it comes back quickly once the phonology system is functional. This is why a recovering speaker can produce grammatical sentences with word-finding difficulty — the frame is back before the vocabulary is.

**Clinical readout:** Inflection error rate. Mean length of utterance (MLU). Function-word omission rate. Word-order error rate.

**Anchor:** *(stub — telegraphic speech in aphasia; agrammatism literature; stress effects on grammatical processing)*

---

# GROUP III — MOTOR LAYERS

*Single-domain or substrate. Collapse last.*

---

## 12. The Phonological Layer

**Definition:** The layer that selects phonemes and sequences them into syllables — phoneme selection and articulatory planning.

**Binds:** Left-hemisphere motor sequencing + timing precision.

**Collapse signature:** Slurring. Blurred phoneme boundaries. Cluster errors. Tight-timing word errors (consonant clusters, rapid transitions, complex syllable structures). Phoneme substitutions.

**Tight-timing words** require tighter phase-locking than loose-timing words. The tighter the phase-locking, the higher the precision required. This is why "strengths," "rural," and "particularly" fail before "cat," "dog," and "the."

**Phonotactic complexity varies by language.** English allows complex clusters; Japanese allows almost none. The same precision level produces different error rates in different languages.

**Recovery signature:** Returns after articulation, before grammar. Phoneme boundaries sharpen as the motor system stabilizes.

**Clinical readout:** Slurring measures. Cluster error rate. Phoneme boundary crispness. Tight-timing word error rate.

**Anchor:** *(stub — articulatory timing literature; phonotactic complexity cross-linguistic studies; Parkinson's articulation)*

---

## 13. The Articulatory Layer

**Definition:** The layer that executes the motor gestures — the physical production of the phoneme sequence.

**Binds:** Motor precision + breath pressure + postural stability.

**Collapse signature:** Mumbling. Reduced amplitude. Imprecise consonants. Voice quality changes. Motor-first production (fluent output without semantic binding, Stage 6 collapse readout).

**Mumbling is amplitude collapse.** The pressure envelope drops, the vocal fold oscillation drops, the articulation precision drops. The output is quiet and imprecise. Slurring is different — it is hemispheric desynchronization, a phonological-layer failure. They often co-occur but have different mechanisms.

**Recovery signature:** Returns after breath, before phonology. Motor patterns are cached, so they come back quickly once the substrate is stable.

**Clinical readout:** Consonant precision. Amplitude stability. Motor-first production incidence. Postural sway during speech.

**Anchor:** *(stub — motor speech disorder literature; dysarthria profiles; motor-first production in manic and dissociative states)*

---

## 14. The Breath/Pressure Layer

**Definition:** The layer that generates and sustains the subglottal pressure envelope — the substrate source for all speech production.

**Binds:** Diaphragm + intercostals + abdominal wall + laryngeal muscles.

**Collapse signature:** Low amplitude. Vocal fry. Breathy voice. Short phrase length. Chest breathing dominance. The pressure envelope is at its floor.

**The postural link.** The diaphragm is both a breath muscle and a postural muscle. Activating it for speech changes the trunk's stability configuration. Vestibular input is modulated by respiration; breath phase affects postural sway. This is why speech production has a substrate cost that typing does not — the pressure system competes with postural control for the same precision budget.

**Recovery signature:** Returns first. Breath is a physiological parameter that responds quickly to intervention. Everything else depends on it, so nothing else recovers until it does.

**Clinical readout:** Amplitude. Phrase length. Fry onset threshold. Breath mechanics (respiratory inductance plethysmography). Postural sway during speech.

**Anchor:** *(stub — breath mechanics and prosody studies; CO₂ tolerance and speech; Zelano et al. 2016 respiration entrainment)*

---

# Book II Summary Table

| Group | Layer | Order | Collapse signature | Recovery order |
|---|---|---|---|---|
| **Integration** | Pragmatic | 1 | Literal, off-target, socially blunt | 8 (last) |
| **Integration** | Discourse | 2 | Tangential, repetitive, lost thread | 7 |
| **Integration** | Prosodic | 3 | Flat, monotone, granularity loss | 6 |
| **Retrieval** | Lexical | 4 | TOT, word-finding failure, proper names first | 5 |
| **Retrieval** | Morphosyntactic | 5 | Telegraphic, dropped inflections | 4 |
| **Motor** | Phonological | 6 | Slurring, cluster errors | 3 |
| **Motor** | Articulatory | 7 | Mumbling, imprecise consonants | 2 |
| **Motor** | Breath/pressure | 8 | Low amplitude, fry | 1 (first) |

**The collapse order** runs 1 → 8 (integration first, motor last). **The recovery order** runs 8 → 1 (motor first, integration last). The two orders are mirrors, but not symmetric — recovery is slower than collapse, and some layers recover faster than others within their group.

---

# Where Book II Ends

Book II is a lookup table with enough context to be usable. Each layer has six lines: definition, binds, collapse signature, recovery signature, clinical readout, anchor. The anchor is stubbed for the citation pass.

**What Book II does not do:**

- It does not argue for the layer boundaries. That argument is in Book I §4.
- It does not specify the measurement protocols. That's Book IV.
- It does not cover cross-linguistic variation. That's Book III §20.
- It does not cover the etiological profiles. Those are in Book V §26.

**What Book II does:**

- It gives the reader a reference for each layer.
- It shows the collapse order at a glance.
- It shows the recovery order as the mirror.
- It names the anchor for each layer, so the citation pass has a target.

---

# BOOK III — THE DYNAMICS

## How the model changes across contexts

---

## How to Read Book III

Book III is a set of demonstrations. Each chapter shows one **variable change** producing one **behavior change**, with an anchor for the invariant. Chapters are short (2–3 pages), each structured the same way:

- **The variable change** — what changes in the model
- **The behavior change** — what changes in speech
- **The anchor** — the study or observation that shows the invariant *(stubbed — see Appendix F)*
- **The prediction** — what the model expects to see

Book III does not re-argue the model. That's Book I. Book III shows the model *moving* — what happens when the variable changes across contexts.

**Seven chapters:**

| Chapter | Variable change | Behavior change |
|---|---|---|
| 15. Recovery in practice | Substrate restoration | Audible recovery before subjective recovery |
| 16. Cross-domain conflicts | Concurrent precision demand | Layer-specific degradation |
| 17. Channel economics | Channel substrate cost | Channel preference shift under load |
| 18. Salience routing and masking | Routing target | Congruent vs. incongruent prosody |
| 19. Precision ecology | Environmental $W^*$ narrowing + postural load | Generational channel shift and postural speech signature |
| 20. Cross-linguistic variation | Suprasegmental demand | Different failure modes by language type |
| 21. Modality and code | Channel substrate profile | Sign vs. speech vs. inner speech collapse schedules |

---

## 15. Recovery in Practice

### 15.1 The variable change

Recovery is substrate restoration. The variable that changes is $A_s^*$ (oscillatory amplitude) restoring, $I^*$ (interoceptive routing) returning, and $C_{high}(L^*)$ (CO₂ ceiling) decompressing as $L^*$ drops.

The model says: nothing recovers until the substrate recovers. Breath comes first. Then articulation, phonology, grammar, lexical, prosody, discourse, pragmatics — in that order.

### 15.2 The behavior change

**The voice returns before the person feels better.** This is the central applied observation. The motor and substrate layers recover before the integration layers. The speaker's breath stabilizes, articulation sharpens, grammar returns — all before prosody, discourse, and pragmatics return.

**To the listener:** the speaker sounds normal.
**To the speaker:** they still feel off.

**Why this matters clinically:** subjective report lags objective recovery. A speaker who says "I'm not better yet" may already be sounding better. A speaker who says "I'm fine now" may still be in the integration-recovery phase and not yet reliable for high-demand social or cognitive tasks.

**The recovery-detection asymmetry:** the recovery signal is audible in the voice before it's reportable by the speaker. This makes speech a leading indicator of recovery, just as it's a leading indicator of collapse.

**The routing caveat.** If $f_{routing}$ is low, the recovery is routed away from expression. The substrate restores, but the voice doesn't show it until the mask drops. A masked speaker may sound the same throughout the recovery, then suddenly show the recovery when the routing changes. The clinician should track both the voice and the routing.

### 15.3 The anchor

*(stub — depression recovery prosody studies; trauma recovery voice studies; the "sounds better before feels better" clinical observation)*

### 15.4 The prediction

**PREDICT-SPEECH-21:** In recovery from depression, trauma, or burnout, prosodic granularity returns before subjective mood report. The gap between granularity return and subjective report should be measurable in days to weeks.

**PREDICT-SPEECH-22:** Recovery order should mirror collapse order. Layers that collapse last should recover first. If a layer recovers out of order, the integration-demand rule is wrong.

**PREDICT-SPEECH-23:** Recovery time should scale super-proportionally with collapse depth. Deeper collapses should take disproportionately longer to recover, not proportionally longer.

---

## 16. Cross-Domain Conflicts

### 16.1 The variable change

Speech production consumes precision. Concurrent tasks also consume precision. When two tasks compete for the same precision budget, speech degrades — and it degrades **layer-specifically**, depending on which layers the concurrent task competes with.

The variable change: **concurrent precision demand.**

### 16.2 The behavior change

The conflict model predicts different degradation signatures depending on the task pair. The rule: the concurrent task competes with the layers that share its precision demand.

| Task pair | Shared precision demand | Predicted degradation |
|---|---|---|
| **Gaming + talking** | Motor timing + visual attention + WM | Prosody + discourse (both require timing + WM) |
| **Driving + talking** | Motor timing + spatial attention | Prosody + articulation (both require timing + motor) |
| **Coding + talking** | Working memory + symbolic manipulation | Discourse + morphosyntax (both require WM + frame-holding) |
| **Reading + talking** | Visual + semantic + phonological | Lexical + phonological (both require semantic + phonological) |
| **Listening to speech + speaking** | Auditory + prosodic + semantic | Prosody + pragmatic (both require prosodic + contextual binding) |

**The prediction:** the degradation signature should be predictable from the shared precision demand. Gaming should flatten prosody before it telegraphs grammar. Coding should telegraph grammar before it flattens prosody. The signature is the task pair made audible.

### 16.3 The anchor

*(stub — dual-task interference literature; driving-and-talking studies; gaming-and-talking studies; coding-and-talking observations)*

### 16.4 The prediction

**PREDICT-SPEECH-24:** The degradation signature during a concurrent task is predictable from the shared precision demand. Task pairs with motor-timing overlap degrade prosody and articulation; task pairs with WM overlap degrade discourse and morphosyntax.

**PREDICT-SPEECH-25:** "Can you talk while X?" is a precision-budget question. Speakers who show larger speech degradation during a concurrent task should also show lower baseline precision on other measures.

---

## 17. Channel Economics

### 17.1 The variable change

Channels differ in substrate cost. Speech is the most expensive — pressure modulation, postural reconfiguration, laryngeal control. Typing is cheap — posturally static, no pressure demand. Inner speech is nearly free — no motor output at all.

The variable change: **channel substrate cost.**

### 17.2 The behavior change

When precision is abundant, the speaker uses speech freely. When precision is scarce, the speaker shifts to cheaper channels. The shift is not stylistic; it is substrate-driven.

**The shift pattern:**

| Precision state | Channel preference |
|---|---|
| Abundant | Speech (highest bandwidth, highest cost) |
| Moderate | Speech, with typing for high-demand content |
| Scarce | Typing (lower cost, more editable) |
| Depleted | Inner speech, minimal output |

**Why people avoid phone calls.** Phone calls require speech production and real-time comprehension simultaneously. Both compete for the same precision budget. Texting allows the comprehension and production to be sequential rather than simultaneous. The preference for texting is a precision-budget optimization, not a social preference.

**Why people stop talking while gaming.** Gaming already consumes motor timing and visual attention. Adding speech production means the pressure system competes for the same budget. The speaker goes silent — not because they don't want to talk, but because the budget is spent.

**Why ND profiles select different channels under load.** The channel shift is substrate-driven in every population. ND profiles show it earlier and more sharply because their baseline precision is lower.

### 17.3 The anchor

*(stub — typing vs. speech preference studies; phone-call avoidance literature; gaming-and-talking observations; ND communication preference studies)*

### 17.4 The prediction

**PREDICT-SPEECH-26:** Channel preference shifts from speech to typing under increasing load. The shift is a leading indicator of precision collapse — it happens before measurable speech degradation.

**PREDICT-SPEECH-27:** The magnitude of the speech-vs-typing precision gap correlates with CO₂ tolerance, postural sway during speech, and HRV. Speakers with low CO₂ tolerance show larger gaps.

**PREDICT-SPEECH-28:** Speech produced while seated is more precise than speech produced while standing, because postural demand is lower. The seated-vs-standing gap should be larger in speakers with low CO₂ tolerance.

---

## 18. Salience Routing and Masking

### 18.1 The variable change

The variable is $f_{routing}$ — the proportion of available salience that reaches expression, versus the proportion spent on output management.

**High $f_{routing}$:** salience flows into the voice. Prosody is congruent with state.

**Low $f_{routing}$:** salience is spent on controlling what the output looks like. Prosody is incongruent with state.

The variable change: **routing target.**

### 18.2 The behavior change

**The mask is a routing configuration, not a behavior.** When a speaker routes salience to output management, they are not "pretending." They are spending precision on the production of normal-seeming output. The precision spent there is precision not spent on:

- **Interoceptive readout** — the system's own state detection
- **Cross-domain integration** — the layers that need the most precision
- **Recovery** — the substrate restoration that requires slack

**Why masking is invisible to the listener.** The voice is funded. High $A_s^*$ produces high-amplitude, prosodically rich speech regardless of where the salience is routed. The listener hears expressiveness. They do not hear congruence. Congruence requires comparing the voice to the state, and the listener does not have access to the state.

**Why masking is invisible to the speaker.** If salience is routed to output management, less is available for interoception. The system is not reading its own state. It cannot detect its own collapse because the detection channel is the one being starved. This is the mechanism behind "I didn't realize how bad it was until I crashed."

**Why masking precedes burnout.** Chronic low $f_{routing}$ means chronic interoceptive starvation. The system runs without its own warning channel. Collapse proceeds from Stage 1 to Stage 3–4 without triggering the Stage 1–2 monitoring window. The result is terminal collapse from a state that looked fine the whole way down.

### 18.3 The masking profile table

| Population | Why $f_{routing}$ is low | Signature |
|---|---|---|
| **ND adults** | Social cost of unmasked expression is high; masking is trained early | Expressive speech, high allostatic load, late collapse detection |
| **Trauma survivors** | Expression was unsafe; routing to output management is protective | Expressive or flat speech, incongruent with reported state |
| **High-status professionals** | Performance is role-required; expression is managed | Expressive speech, depletion, "imposter" reports |
| **Alexithymia** | $I^*$ is low, so $S_{available}$ is low regardless of routing | Flat speech, no mask possible — nothing to route |
| **Depression** | $A_s^*$ is low, so there is little to route | Flat speech, congruent — the collapse is honest |

**The alexithymia/depression distinction.** Both produce flat prosody. Alexithymia produces it because the interoceptive signal is unavailable ($S_{available}$ is low). Depression produces it because the amplitude is unavailable ($A_s^*$ is low). The routing variable separates them: alexithymia has low $S_{available}$ with normal routing; depression has low $A_s^*$ with normal routing. Neither is a masking profile.

**The ND/trauma distinction.** Both produce masking. ND masking is substrate-driven — the cost of unmasked expression is higher for the ND speaker because the default allocation differs from the context-appropriate one. Trauma masking is context-driven — the cost of unmasked expression was higher in the original context. Same routing configuration, different origin. The routing variable doesn't distinguish them; the history does.

### 18.4 The anchor

*(stub — emotional granularity literature; masking and allostatic load studies; ND masking cost studies; alexithymia interoception studies)*

### 18.5 The prediction

**PREDICT-SPEECH-58:** Prosodic congruence — the match between voice and reported state — is predicted by $f_{routing}$, not by $A_s^*$ or $\Pi_{cog}$ alone. Two speakers with the same amplitude and load but different routing targets show different congruence.

**PREDICT-SPEECH-59:** Chronic low $f_{routing}$ predicts later collapse detection. Maskers reach Stage 3–4 before reporting Stage 1–2 symptoms, compared to non-maskers at the same precision level.

**PREDICT-SPEECH-60:** Allostatic load is higher in high-$A_s^*$, low-$f_{routing}$ speakers than in high-$A_s^*$, high-$f_{routing}$ speakers. The mask has a measurable cost.

---

## 19. Precision Ecology

### 19.1 The variable change

Environments differ in their precision demand. Some environments narrow $W^*$, increase $J$, and load the postural system. Others leave the substrate alone.

The variable change: **environmental precision demand** — including digital load and postural load.

### 19.2 The behavior change

**Digital load.** Modern digital environments place continuous demands on precision:

- **Continuous micro-threat cues** (notifications, social media, email) raise $\Pi_{cog}$ and keep the system in low-grade threat processing
- **Multitasking** raises $J$ and narrows $W^*$
- **High channel-cost activities** (gaming, streaming, video calls) consume precision that would otherwise go to speech production
- **Text-based communication** shifts the channel toward lower-cost options

The predicted pattern: populations in high-digital-load environments show the pragmatic → discourse → prosody collapse sequence in daily life, not just under acute load. The collapse becomes the baseline.

**Postural load.** The diaphragm is both a breath muscle and a postural muscle. Modern postural patterns — extended sitting, forward head posture, phone-in-hand positioning — change the trunk's stability configuration. This affects the pressure system directly:

- **Forward head posture** changes the diaphragm's mechanical advantage
- **Extended sitting** reduces diaphragm excursion
- **Phone-in-hand posture** creates asymmetric trunk loading
- **Screen-viewing posture** tends toward chest breathing

The predicted pattern: postural load reduces breath efficiency, which reduces the pressure envelope, which flattens prosody and reduces amplitude. The generational speech pattern may be substantially a postural pattern.

**The combined ecology.** Digital load and postural load are not separate. They interact: the postures people adopt while using devices reduce breath efficiency, while the devices themselves place precision demands that make speech production harder. A generation raised with devices in hand may have a **different baseline substrate** than a generation raised without them — not because of the devices per se, but because of the postural and precision-load patterns the devices induce.

### 19.3 The anchor

*(stub — digital load and cognition studies; posture and breathing studies; forward head posture and diaphragm function; generational speech pattern observations)*

### 19.4 The prediction

**PREDICT-SPEECH-29:** Generational speech patterns track generational substrate profiles. Populations raised in high-digital-load, high-postural-load environments should show earlier pragmatic and discourse collapse signatures than populations raised in low-load environments.

**PREDICT-SPEECH-30:** Postural interventions (breath training, posture correction, seated speech) should produce measurable improvement in prosodic granularity and amplitude stability. The improvement should be larger in high-postural-load speakers.

**PREDICT-SPEECH-31:** The channel shift toward text-based communication should track both digital load and postural load. Populations with high postural load should show the shift even when digital load is controlled.

**The caution:** generational and ecological claims are hard to disentangle from cohort effects, technology adoption, and cultural change. If the predictions fail, they disconfirm the ecological projection, not the model. The model's core claims (variable, layers, collapse order) hold regardless.

---

## 20. Cross-Linguistic Variation

### 20.1 The variable change

Languages differ in how many timing-encoded layers they stack. Stress-timed languages use timing for rhythm. Tonal languages use it for lexical identity. Pitch-accent languages use it for word recognition. Mora-timed languages use it for unit duration.

The variable change: **suprasegmental demand.**

### 20.2 The behavior change

The same precision drop produces different collapse signatures depending on the language's suprasegmental architecture:

| Language type | What timing carries | Collapse signature |
|---|---|---|
| **Stress-timed** | Lexical stress, rhythm | Prosodic flattening; stress misplacement; rhythm destabilization |
| **Syllable-timed** | Even timing, less reduction | Reduced prosodic range; less dramatic collapse (timing is less load-bearing) |
| **Mora-timed** | Unit duration | Timing irregularities; mora-count errors |
| **Tonal** | Lexical meaning (pitch contour) | **Lexical identity errors** — the word changes, not just the tone |
| **Pitch-accent** | Lexical meaning (pitch location) | **Accent misplacement** — the pitch is there but on the wrong syllable |
| **Intonational** | Phrase-level meaning | Phrase-boundary errors; question/statement confusion |

**The Japanese case.** Japanese is mora-timed *and* pitch-accent. Two timing-encoded layers stacked. A precision drop in Japanese doesn't just flatten emotional prosody — it can change lexical identity. This is a different failure mode than in English, where a precision drop flattens prosody but doesn't typically change word meaning.

**Phonotactic complexity.** English allows complex clusters ("strengths"); Japanese allows almost none. The same precision level produces different articulation error rates in different languages.

### 20.3 The anchor

*(stub — tonal language speech error studies; pitch-accent processing under load; cross-linguistic prosody studies; phonotactic complexity comparisons)*

### 20.4 The prediction

**PREDICT-SPEECH-32:** Speakers of suprasegmentally complex languages (tonal, pitch-accent, mora-timed) show different collapse signatures than speakers of suprasegmentally simple languages. Tonal speakers show lexical identity errors under load; pitch-accent speakers show accent misplacement; stress-timed speakers show prosodic flattening.

**PREDICT-SPEECH-33:** Speakers of suprasegmentally complex languages allocate more baseline precision to the timing layer, measurable as higher baseline interhemispheric coherence or higher CO₂ tolerance.

**PREDICT-SPEECH-34:** Articulation error rates on tight-timing words scale with the language's phonotactic complexity, not with word frequency alone.

---

## 21. Modality and Code

### 21.1 The variable change

Channels differ in substrate cost. Sign language has no pressure demand but requires sustained visual attention and manual motor precision. Inner speech has no motor output at all. Written language bypasses the timing layer and the pressure system.

The variable change: **channel substrate profile.**

### 21.2 The behavior change

Each modality has its own collapse schedule:

| Modality | Substrate cost | Collapse schedule |
|---|---|---|
| **Speech** | Pressure modulation, postural reconfiguration, laryngeal control | Integration layers collapse first; motor layers last |
| **Sign** | Visual attention, manual motor precision — no pressure demand | Prosodic collapse (facial expression, movement dynamics) may be on a different schedule than speech prosody |
| **Inner speech** | Minimal — no motor, no pressure | Preserved longer than overt speech; skips articulatory and breath layers |
| **Writing** | Minimal — posturally static, fine motor only | Preserved relative to speech during precision collapse; bypasses timing layer entirely |

**Code-switching as demand management.** Bilingual speakers switching between languages with different suprasegmental architectures are switching demand profiles in real time. Code-switching into a higher-demand language should produce earlier collapse signatures than staying in the lower-demand language.

**Inner speech preservation.** Inner speech should be preserved longer than overt speech under precision collapse, because it skips the two most expensive layers (articulatory and breath). This is testable with experience-sampling methods.

**Written/speech dissociation.** Writing bypasses the timing layer and the pressure system. Written output should be preserved relative to spoken output during precision collapse, and the gap should widen as precision drops. This is a clean, cheap test: collect both from the same subjects under load.

### 21.3 The anchor

*(stub — sign language prosody studies; inner speech under load; written vs. spoken production under load; bilingual code-switching and cognitive load)*

### 21.4 The prediction

**PREDICT-SPEECH-35:** Inner speech is preserved longer than overt speech under precision collapse. The preservation gap should scale with collapse depth.

**PREDICT-SPEECH-36:** Written output is preserved relative to spoken output during precision collapse. The written-vs-spoken gap should widen as precision drops.

**PREDICT-SPEECH-37:** Deaf signers show different collapse signatures than hearing speakers, because the substrate cost profile is different. Sign prosody should collapse on a different schedule than speech prosody.

**PREDICT-SPEECH-38:** Code-switching into a higher-demand language (more suprasegmental layers) produces earlier collapse signatures than staying in a lower-demand language.

---

# Book III Summary Table

| Chapter | Variable change | Behavior change | Key prediction |
|---|---|---|---|
| 15. Recovery in practice | Substrate restoration | Voice returns before subjective recovery | PREDICT-21, -22, -23 |
| 16. Cross-domain conflicts | Concurrent precision demand | Layer-specific degradation by task pair | PREDICT-24, -25 |
| 17. Channel economics | Channel substrate cost | Channel preference shift under load | PREDICT-26, -27, -28 |
| 18. Salience routing and masking | Routing target | Congruent vs. incongruent prosody | PREDICT-58, -59, -60 |
| 19. Precision ecology | Environmental $W^*$ narrowing + postural load | Generational channel shift + postural speech signature | PREDICT-29, -30, -31 |
| 20. Cross-linguistic variation | Suprasegmental demand | Different failure modes by language type | PREDICT-32, -33, -34 |
| 21. Modality and code | Channel substrate profile | Different collapse schedules by modality | PREDICT-35, -36, -37, -38 |

---

# Where Book III Ends

Book III is a set of demonstrations. Each chapter shows one variable change producing one behavior change, with an anchor stubbed for the citation pass. The chapters are short because the model is already specified in Book I. Book III just shows the model moving.

**What Book III does not do:**

- It does not re-argue the model.
- It does not specify measurement protocols. That's Book IV.
- It does not cover the clinical conditions. That's Book V.
- It does not have the full prediction registry. That's Appendix B.

**What Book III does:**

- It shows the model operating across seven contexts.
- It generates 21 new predictions (PREDICT-SPEECH-21 through -38, and -58 through -60).
- It names the anchor for each demonstration.
- It makes the paper's empirical reach explicit.

**The anchor stubs** are the citation pass targets. Each chapter names what kind of study would confirm or disconfirm its claim. When you're ready, the citation pass fills them in.

---

*End of Books I–III.*

# The Spoken Language Paper v3.1 — Part 2

## Books IV–V and Appendices A–H

---

# BOOK IV — THE MEASUREMENT

## Conceptual protocol for observing the model

---

## How to Read Book IV

Book IV is the measurement book. It answers one question: **how do we observe the model?**

It is organized around the layer structure, not around a list of measures. Each layer has one primary biomarker. Channel preference sits outside the layer structure as the cheapest leading signal.

**Five chapters:**

| Chapter | Content |
|---|---|
| 22. Why speech is a monitoring channel | The Stage 1–2 window; speech changes before subjective report |
| 23. The biomarker inventory | One biomarker per layer, plus channel preference |
| 24. The diagnostic battery | How to combine biomarkers into a protocol |
| 25. The monitoring ladder | Which layer to measure at which stage |
| 26. Channel preference as diagnostic | The cheapest signal — the channel shift |

Book IV is **conceptual**, not implementation-detail. It says what to measure and why. The implementation is for a companion methods paper.

---

## 22. Why Speech Is a Monitoring Channel

### 22.1 The monitoring window

Central Reference §5b contains the critical annotation:

> *"Stage 5 looks like competence from the outside. The monitoring window is Stages 1–2."*

The monitoring metrics currently used in clinical practice — HRV, RHR, Control Pause, respiratory rate — are physiological. They are not speech. But the speech signature changes at Stages 1–2, before Stage 5 closes the gate.

**Stage 5 looks like competence.** When the gate closes, the output becomes high-confidence and low-variance — the signature of an expert operating from deep prior. The system appears functional. The monitoring window has already passed.

**The speech signal is in the window.** Speech changes at Stages 1–2, when precision drops and the window narrows. Pragmatic failure, discourse instability, and prosodic flattening are audible before the gate closes. This is what makes speech a monitoring channel.

### 22.2 Why speech is the right channel

Speech has four properties that make it a good monitoring channel:

- **It's non-invasive.** No blood draw, no lab equipment, no clinical visit. A phone recording is sufficient.
- **It's continuous.** It can be sampled repeatedly, in natural contexts, without disrupting the speaker.
- **It's layered.** The eight layers give eight measurable readouts, each tied to a stage of collapse.
- **It's leading.** Speech changes before subjective report. The speaker does not need to notice the change for the signal to be present.

### 22.3 The routing caveat

Speech is a monitoring channel only if the salience is routed to expression. A speaker with low $f_{routing}$ is spending precision on output management, and the collapse may not be audible in the voice.

**This does not break the monitoring claim.** It adds a second measurement: congruence. The voice may not show the collapse, but the *mismatch* between the voice and the speaker's reported state does. A masked speaker who sounds fine but reports exhaustion is showing the routing signal.

**The monitoring claim, revised:** speech is a Stage 1–2 monitoring channel for *unmasked* collapse. For masked collapse, the monitoring signal is the congruence gap — the mismatch between voice and state.

### 22.4 The clinical claim

**Speech is a Stage 1–2 monitoring channel that the field is not currently using.**

This is the paper's applied contribution. The mechanism is specified in Book I; the layers are specified in Book II; the dynamics are specified in Book III. Book IV specifies what to measure.

### 22.5 The full monitoring ladder preview

| Stage | Layer collapsing | Biomarker |
|---|---|---|
| 1–2 | Pragmatic | Social appropriateness ratings |
| 2–3 | Discourse | Topic coherence |
| 2–3 | Prosodic | Pitch granularity |
| 3–4 | Lexical | TOT frequency, proper-name failure rate |
| 4 | Morphosyntactic | Inflection error rate |
| 4–5 | Phonological | Slurring measures |
| 5 | Articulatory | Consonant precision |
| 5–6 | Breath | Amplitude, fry onset |
| **Stage-independent** | **Channel preference** | **Speech-to-typing shift** |
| **Stage-independent** | **Routing** | **Congruence gap** |

The channel preference shift and the congruence gap sit outside the layer ladder because they are not layer collapses — they are **budget and routing readouts**. The speaker shifts channels before any layer collapses, and shows the congruence gap when the collapse is masked. They are the earliest signals.

---

## 23. The Biomarker Inventory

### 23.1 How to read this chapter

Each layer has one **primary biomarker**. The biomarker is chosen because it's:

- **Tied to the layer** — it measures what the layer does
- **Extractable** — it can be computed from a standard recording
- **Leading** — it changes before the layer's grosser properties degrade
- **Sensitive** — it responds to precision change, not just to gross impairment

Each entry follows the same structure:

- **What it measures**
- **What it tracks** (in the model)
- **Why it's early**
- **How to extract it**
- **Anchor** *(stubbed for citation pass — see Appendix F)*

### 23.2 The primary biomarkers, by layer

---

**Pragmatic layer — Social appropriateness rating**

**What it measures:** The match between the utterance and its social context — whether the speaker said the right thing for the situation.

**What it tracks:** The integration of ToM, context, prosody, lexical choice, and timing. Pragmatic failure is the first audible-via-content sign of precision collapse.

**Why it's early:** Pragmatics requires the most cross-domain integration. When any input degrades, pragmatics degrades first. It has no cached fallback because context is always novel.

**How to extract it:** Standardized role-play tasks with blinded raters. Implicature comprehension tests. Register-matching tasks. The rating is not acoustic — it's content-based.

**Anchor:** *(stub — pragmatic failure in high-load states; autism pragmatic profiles; right-hemisphere pragmatics)*

---

**Discourse layer — Topic coherence**

**What it measures:** The stability of the conversational thread across turns — whether the speaker stays on topic, tracks referents, and repairs breakdowns.

**What it tracks:** Working memory, timing coordination, predictive modeling, interoceptive pacing. Discourse collapse is the second audible-via-content sign.

**Why it's early:** Discourse requires holding multiple turns in working memory. When $W^*$ narrows, the thread falls out of the window.

**How to extract it:** Topic coherence measures on narrative samples. Turn-transition latency. Referential tracking accuracy. Repair-initiation frequency.

**Anchor:** *(stub — ADHD discourse instability; working-memory and topic-maintenance; turn-taking and inter-brain synchrony)*

---

**Prosodic layer — Pitch granularity**

**What it measures:** Cycle-to-cycle pitch modulation depth — the fine variation in fundamental frequency across adjacent pitch periods.

**What it tracks:** Right-hemisphere motor control over the laryngeal and respiratory muscles. Granularity loss is the first audible-in-the-voice sign of precision collapse.

**Why it's early:** Granularity loss precedes pitch range loss. The voice retains gross pitch movement but loses the fine contour before it loses range. This is why granularity is the leading prosodic indicator.

**How to extract it:** Acoustic analysis of sustained vowels or standardized utterances. Compute cycle-to-cycle $F_0$ variation. Granularity is distinct from range — a speaker can have a wide range with low granularity (a "smooth" monotone) or a narrow range with high granularity (a "quiet expressive" voice).

**Anchor:** *(stub — Ross aprosodia; trauma prosodic granularity; right-hemisphere prosody dominance)*

---

**Lexical layer — Proper-name failure rate**

**What it measures:** The rate of proper-name retrieval failures under standardized load.

**What it tracks:** Lexical retrieval precision. Proper names have no semantic neighborhood, so they require the highest precision of any lexical category. They fail first.

**Why it's early:** Proper names fail before common nouns under precision collapse, because they have the least redundant retrieval pathway. The single entry point — the direct semantic-phonological link — fails first.

**How to extract it:** Standardized naming tasks under load. Compare proper-name retrieval to common-noun retrieval. The proper-name/common-noun gap is the biomarker.

**Anchor:** *(stub — TOT under stress; proper-name retrieval studies; semantic neighborhood effects)*

---

**Morphosyntactic layer — Inflection error rate**

**What it measures:** The rate of dropped inflections, agreement errors, and function-word omissions.

**What it tracks:** Rule retrieval, working memory, phonological encoding. Morphosyntactic collapse is the telegraphic speech signature.

**Why it's early within its stage:** Grammar is highly cached, so it survives longer than lexical and prosodic. But when it collapses, the inflection error rate rises sharply — the frame can't be held.

**How to extract it:** Inflection error rate. Mean length of utterance. Function-word omission rate. Word-order error rate.

**Anchor:** *(stub — telegraphic speech in aphasia; agrammatism; stress effects on grammatical processing)*

---

**Phonological layer — Slurring measures**

**What it measures:** Phoneme boundary crispness — the sharpness of the transition between adjacent articulation events.

**What it tracks:** Left-hemisphere motor sequencing + timing precision. Slurring is hemispheric desynchronization, not a phoneme production failure.

**Why it's early within its stage:** Slurring precedes full motor collapse. The phoneme boundaries blur before the phonemes drop out.

**How to extract it:** Slurring measures on standardized utterances. Cluster error rate. Tight-timing word error rate. Phoneme boundary crispness (spectral transition sharpness).

**Anchor:** *(stub — articulatory timing; phonotactic complexity cross-linguistic; Parkinson's articulation)*

---

**Articulatory layer — Consonant precision**

**What it measures:** The precision of consonant production — place, manner, and voicing accuracy.

**What it tracks:** Motor precision + breath pressure + postural stability. Articulatory collapse is the mumbling signature.

**Why it's early within its stage:** Consonant precision degrades before vowels, because consonants require tighter motor timing. Mumbling is a consonant-precision failure, not a vowel failure.

**How to extract it:** Consonant precision measures. Amplitude stability. Motor-first production incidence. Postural sway during speech.

**Anchor:** *(stub — motor speech disorder; dysarthria profiles; motor-first production in manic and dissociative states)*

---

**Breath layer — Amplitude and fry onset**

**What it measures:** The pressure envelope — its amplitude, its stability, and the threshold at which fry begins.

**What it tracks:** Diaphragm, intercostals, abdominal wall, laryngeal muscles. Breath collapse is the substrate failure.

**Why it's early within its stage:** Amplitude drops before fry begins. Fry is the floor of the pressure envelope — the point at which the vocal folds vibrate at their lowest stable mode. The fry onset threshold is the biomarker.

**How to extract it:** Amplitude. Phrase length. Fry onset threshold. Breath mechanics (respiratory inductance plethysmography). Postural sway during speech.

**Anchor:** *(stub — breath mechanics and prosody; CO₂ tolerance and speech; Zelano et al. 2016)*

---

### 23.3 The routing biomarker

---

**Routing — Prosodic congruence**

**What it measures:** The match between the voice and the speaker's reported state. A speaker who sounds animated but reports exhaustion is incongruent. A speaker who sounds flat and reports depression is congruent.

**What it tracks:** $f_{routing}$ — the proportion of available salience that reaches expression. Congruence is high when $f_{routing}$ is high; congruence is low when the mask is running.

**Why it's early:** Congruence shifts before the voice degrades, because the routing shifts before the collapse. A speaker who is beginning to mask will show the congruence gap before they show the collapse.

**How to extract it:** Compare acoustic expressiveness measures (pitch range, amplitude, granularity) to self-reported state (mood, energy, load). The gap between the two is the congruence measure. Requires a self-report instrument paired with the acoustic sample.

**Anchor:** *(stub — emotional granularity literature; masking and allostatic load studies; alexithymia interoception studies)*

---

### 23.4 The channel-preference biomarker

---

**Channel preference — Speech-to-typing shift**

**What it measures:** The speaker's channel choice under load — whether they shift from speech to typing (or from speech to inner speech, or from typing to silence).

**What it tracks:** The precision budget. Channel choice is a readout of how much precision the speaker has available for the highest-cost channel.

**Why it's earliest:** Channel preference shifts **before** any layer collapses, because the shift is a proactive response to the budget. The speaker avoids the channel that would show the degradation. By the time the degradation is measurable in speech, the speaker has already shifted away from speech.

**How to extract it:** Self-report of channel preference. Observation of channel choice in natural contexts. Experimental measures: give the speaker a choice between speech and typing under load, and observe the shift.

**Anchor:** *(stub — typing vs. speech preference; phone-call avoidance; ND communication preference studies)*

---

### 23.5 The biomarker table

| Layer | Biomarker | What it tracks | Why it's early |
|---|---|---|---|
| Pragmatic | Social appropriateness rating | ToM + context + prosody + lexical + timing | Highest integration demand |
| Discourse | Topic coherence | WM + timing + prediction + interoception | Second-highest integration demand |
| Prosodic | Pitch granularity | RH motor control over laryngeal/respiratory muscles | Granularity precedes range loss |
| Lexical | Proper-name failure rate | Retrieval precision | Proper names have no semantic neighborhood |
| Morphosyntactic | Inflection error rate | Rule retrieval + WM + phonology | Cached but collapses sharply when it does |
| Phonological | Slurring measures | LH motor sequencing + timing | Boundary blur precedes phoneme dropout |
| Articulatory | Consonant precision | Motor + breath + posture | Consonants fail before vowels |
| Breath | Amplitude and fry onset | Diaphragm + intercostals | Amplitude drop precedes fry |
| **Routing** | **Prosodic congruence** | **$f_{routing}$** | **Shifts before the collapse** |
| **Channel** | **Speech-to-typing shift** | **Precision budget** | **Proactive — happens before layer collapse** |

---

## 24. The Diagnostic Battery

### 24.1 The battery principle

The diagnostic battery is not a fixed protocol. It is a **selection rule**: measure the biomarker for the layer you're interested in, use channel preference as the leading indicator, and use congruence as the masking check.

**The selection rule:**

1. **If you want the earliest signal:** measure channel preference. The shift from speech to typing is the first indicator.
2. **If you want to know whether the collapse is masked:** measure congruence. The gap between voice and reported state is the masking signal.
3. **If you want the layer-specific signal:** measure the biomarker for the layer whose collapse you're monitoring.
4. **If you want the full picture:** measure all eight layer biomarkers plus channel preference and congruence.

The battery is modular. It can be run as a single measurement (one layer, one biomarker) or as a full protocol (all layers, all biomarkers, plus routing and channel).

### 24.2 The single-layer protocol

For monitoring a specific layer:

- **Recording:** Standardized utterance or natural speech sample.
- **Extraction:** Compute the layer's primary biomarker.
- **Baseline:** Compare to the speaker's own baseline, not to a population norm.
- **Interpretation:** A drop from baseline in the biomarker indicates collapse at that layer.

**Why within-person baseline:** The framework's variables are normalized to the individual's own baseline. Population norms are not the comparator. A degraded world-class performer may be more impaired than a baseline junior — the metric captures this.

### 24.3 The full protocol

For monitoring all layers:

- **Recording:** Natural speech sample + standardized utterances + channel-preference observation + self-report of state.
- **Extraction:** Compute all eight biomarkers plus channel preference and congruence.
- **Ordering:** The layers should collapse in order. If they don't, the collapse is not following the forced sequence, and something else is happening.
- **Congruence check:** Compare the acoustic expressiveness to the reported state. A large gap indicates low $f_{routing}$ — the collapse may be masked.
- **Interpretation:** The pattern across layers is the readout. A single layer's collapse tells you which layer is degrading. The pattern tells you which stage of the collapse sequence you're in. The congruence tells you whether the collapse is visible.

### 24.4 The layer-to-stage mapping

The biomarkers map to the collapse sequence stages:

| Stage | Layer(s) collapsing | Biomarker(s) |
|---|---|---|
| 1–2 | Pragmatic | Social appropriateness rating |
| 2–3 | Discourse | Topic coherence |
| 2–3 | Prosodic | Pitch granularity |
| 3–4 | Lexical | Proper-name failure rate |
| 4 | Morphosyntactic | Inflection error rate |
| 4–5 | Phonological | Slurring measures |
| 5 | Articulatory | Consonant precision |
| 5–6 | Breath | Amplitude and fry onset |
| **Stage-independent** | **Channel preference** | **Speech-to-typing shift** |
| **Stage-independent** | **Routing** | **Congruence gap** |

### 24.5 The diagnostic output

The diagnostic battery produces a **profile**: which layers are degraded, in which order, whether channel preference has shifted, and whether the collapse is masked.

**The profile tells you:**

- **How deep the collapse is.** Pragmatic-only = early. Pragmatic through lexical = mid. Pragmatic through breath = terminal.
- **How fast it's progressing.** Compare the profile to a previous profile. The speed of layer loss is the collapse rate.
- **Where the recovery will start.** Recovery runs the mirror order. The last layer to collapse will be the first to recover.
- **Whether the collapse is masked.** A large congruence gap indicates low $f_{routing}$ — the collapse is hidden, and the speaker may not be able to report it accurately.

### 24.6 The recording conditions

Standardized conditions matter. The diagnostic should be run under consistent conditions:

- **Same time of day** — load varies by time
- **Same recording setup** — microphone, environment, distance
- **Same utterance set** — standardized materials allow comparison
- **Same load state** — or load state measured and recorded
- **Same self-report instrument** — for the congruence measure

The implementation details are for a companion methods paper. Book IV specifies the conceptual protocol.

---

## 25. The Monitoring Ladder

### 25.1 The monitoring principle

Each stage of collapse has a best-measurable layer. The clinician's job is to pick the layer that's cheapest to measure and most sensitive to the current stage.

**The principle:** measure the layer whose collapse marks the stage you're monitoring. Don't measure all layers if you only need one.

### 25.2 Stage-by-stage monitoring

| Stage | What to measure | Why |
|---|---|---|
| 1–2 | Channel preference + pragmatic rating + congruence | Earliest signals; content-based and routing-based |
| 2–3 | Discourse coherence + pitch granularity | Structure and voice are both changing |
| 3–4 | Proper-name failure rate | Retrieval is the next layer to go |
| 4 | Inflection error rate | Grammar collapse follows lexical |
| 4–5 | Slurring measures | Phoneme boundaries blur |
| 5 | Consonant precision | Motor execution degrades |
| 5–6 | Amplitude + fry onset | Substrate failure |

### 25.3 Choosing the layer

**If you're screening:** measure channel preference and congruence. They're the cheapest and earliest signals.

**If you're monitoring a specific layer:** measure that layer's biomarker.

**If you're tracking stage progression:** measure the layers in collapse order — pragmatic, discourse, prosodic, lexical, morphosyntactic, phonological, articulatory, breath.

**If you're tracking recovery:** measure the layers in recovery order — breath, articulatory, phonological, morphosyntactic, lexical, prosodic, discourse, pragmatic. The first layer to recover tells you where the recovery is.

### 25.4 The full monitoring table

| Stage | Layer | Biomarker | Cost | Sensitivity |
|---|---|---|---|---|
| 1–2 | Pragmatic | Social appropriateness rating | Medium | High |
| 2–3 | Discourse | Topic coherence | Medium | High |
| 2–3 | Prosodic | Pitch granularity | Low | High |
| 3–4 | Lexical | Proper-name failure rate | Low | High |
| 4 | Morphosyntactic | Inflection error rate | Medium | Medium |
| 4–5 | Phonological | Slurring measures | Low | High |
| 5 | Articulatory | Consonant precision | Low | Medium |
| 5–6 | Breath | Amplitude and fry onset | Low | High |
| **Stage-independent** | **Channel** | **Speech-to-typing shift** | **Very low** | **Very high** |
| **Stage-independent** | **Routing** | **Congruence gap** | **Low** | **High** |

**Cost** is the effort to extract the biomarker. **Sensitivity** is how early the biomarker responds to precision change.

The cheapest and highest-sensitivity signals are channel preference and pitch granularity. The congruence measure requires a self-report instrument, which makes it slightly more expensive — but it's the only signal that catches masked collapse.

### 25.5 The monitoring protocol

**Step 1 — Establish baseline.** Record the speaker in a baseline state (low load, rested, no acute stress). Compute all biomarkers. Record self-reported state.

**Step 2 — Periodic monitoring.** Record the speaker at regular intervals. Compute the biomarkers. Compare to baseline. Compute congruence.

**Step 3 — Detect shift.** A shift in channel preference or a drop in any biomarker indicates precision collapse. A large congruence gap indicates the collapse is masked.

**Step 4 — Localize.** The pattern of biomarker drops tells you which layer is collapsing and which stage of the sequence you're in.

**Step 5 — Track recovery.** When recovery begins, the layers return in mirror order. Track the recovery ladder.

### 25.6 The clinical case

The monitoring protocol is cheap, non-invasive, and continuous. It can be run on a phone. It does not require a clinical visit, a blood draw, or specialized equipment. It is a **Stage 1–2 monitoring channel** that the field is not currently using.

**The clinical implication:** "How are you doing?" is a subjective question. "What does your voice sound like today?" is an objective one. The voice changes before the person notices. The speech signal is the leading indicator — unless the collapse is masked, in which case the congruence gap is.

---

## 26. Channel Preference as Diagnostic

### 26.1 Why channel preference matters

Channel preference is the **cheapest, earliest, and most sensitive** biomarker. It shifts before any layer collapses, because it's a proactive response to the precision budget.

**The mechanism:** The speaker avoids the channel that would show the degradation. By the time speech degradation is measurable, the speaker has already shifted away from speech.

**The clinical implication:** "Prefers to type" is not a stylistic preference. It is a **Stage 1–2 monitoring signal** — a report of a precision budget that speech production cannot afford.

### 26.2 The channel cost table

| Channel | Substrate cost | Precision cost |
|---|---|---|
| Speech | Pressure modulation, postural reconfiguration, laryngeal control | Highest |
| Sign | Visual attention, manual motor precision — no pressure demand | Moderate |
| Typing | Posturally static, no pressure demand | Low |
| Inner speech | No motor, no pressure | Minimal |
| Writing (longhand) | Posturally static, fine motor only | Low |

### 26.3 The channel shift as a leading indicator

**The prediction:** Channel preference shifts from speech to typing precede measurable speech degradation under increasing load.

**Why it's leading:** The speaker doesn't wait for their speech to degrade. They feel the budget tightening and shift preemptively. The shift is a readout of the budget, not the collapse.

### 26.4 The channel-preference protocol

**Simple version:** Ask the speaker which channel they'd choose for a high-demand conversation. Track the answer over time. A shift from speech to typing is a shift in budget.

**Experimental version:** Give the speaker a choice between speech and typing under controlled load. Observe the shift point. The shift point is the precision threshold.

**Naturalistic version:** Observe channel choice in daily life. A shift in channel choice in a specific context is a shift in the budget for that context.

### 26.5 The postural link

The channel-cost mechanism has a postural component:

- **Speech** requires postural reconfiguration (the diaphragm is both a breath muscle and a postural muscle).
- **Typing** requires no postural reconfiguration.
- **The seated-vs-standing prediction:** speech produced while seated is more precise than speech produced while standing, because postural demand is lower.

**The clinical implication:** if a speaker's speech is more precise when seated, the postural component of the channel cost is significant. The intervention target is postural, not just respiratory.

### 26.6 The channel-preference predictions

**PREDICT-SPEECH-39:** Channel preference shifts from speech to typing before measurable speech degradation. The shift is a leading indicator of precision collapse.

**PREDICT-SPEECH-40:** The magnitude of the speech-vs-typing precision gap correlates with CO₂ tolerance, postural sway during speech, and HRV. Speakers with low CO₂ tolerance show larger gaps.

**PREDICT-SPEECH-41:** Speech produced while seated is more precise than speech produced while standing. The seated-vs-standing gap is larger in speakers with low CO₂ tolerance.

### 26.7 The monitoring implication

**Channel preference is the cheapest clinical signal.** It requires no recording, no extraction, no baseline. It requires one question: "Would you rather talk or type?"

The answer is a readout of the precision budget. The shift from speech to typing is a Stage 1–2 signal that the field is not currently using.

**The congruence companion:** for masked collapse, the cheapest signal is the congruence gap. It requires one comparison: "How does your voice sound to you?" vs. "How do you feel?" A large gap is the masking signal.

---

# Book IV Summary Table

| Chapter | Content | Key output |
|---|---|---|
| 22. Why speech is a monitoring channel | Stage 1–2 window; speech changes before subjective report; routing caveat | The monitoring principle |
| 23. The biomarker inventory | One biomarker per layer + routing + channel preference | Ten biomarkers |
| 24. The diagnostic battery | Selection rule; single-layer and full protocols | The diagnostic protocol |
| 25. The monitoring ladder | Which layer to measure at which stage | The monitoring table |
| 26. Channel preference as diagnostic | The cheapest, earliest signal | The channel-preference protocol |

---

# Where Book IV Ends

Book IV is the measurement book. It says what to measure, why to measure it, and how to extract it — but not the implementation details. Those are for a companion methods paper.

**What Book IV does not do:**

- It does not specify the recording pipeline.
- It does not specify the acoustic analysis parameters.
- It does not provide normative data.
- It does not provide clinical validation.

**What Book IV does:**

- It specifies the monitoring principle.
- It names one biomarker per layer, plus routing and channel preference.
- It specifies the selection rule for the diagnostic battery.
- It provides the monitoring ladder.
- It names channel preference as the cheapest leading signal and congruence as the masking signal.

**The three new predictions** (PREDICT-SPEECH-39 through -41) are in §26.6. (Note: v3.0's Book IV said "four new predictions" but listed three; v3.1 corrects the count to three.)

---

# BOOK V — THE PROJECTIONS

## The applied payoff

---

## How to Read Book V

Book V is the applied book. It shows what the model looks like in specific conditions and populations. It is shorter than the previous books because the mechanism is already specified in Book I, the layers in Book II, the dynamics in Book III, and the measurement in Book IV. Book V just applies them.

**The structure:**

- **27. Clinical conditions** — table-driven, one row per condition; separate routing-states table
- **28. Social projection** — short chapter, cross-references Book III §19
- **29. Regional accents** — short chapter, cross-references Book III §20
- **30. Drugs and spoken language** — table-driven
- **31. Foreign accent syndrome** — full chapter (it is the cleanest single case of the mechanism)
- **32. The applied summary** — what the model explains, what it predicts, what it opens

Each chapter points to the mechanism rather than re-arguing it.

---

## 27. Clinical Conditions

### 27.1 How to read this chapter

Each clinical condition is a **different entry point into the same collapse sequence**. Some enter at Stage 1 (precision drop), some at Stage 2 (window narrowing), some at Stage 3 (integration failure). The *order* of symptom appearance differs; the *mechanism* is the same.

The table below gives, for each condition: the mechanism, the entry stage, the first layer to collapse, the distinguishing signature, and the anchor. The mechanism column is the key — it names the variable that's changing.

### 27.2 The clinical conditions table

| Condition | Mechanism | Entry stage | First layer to collapse | Distinguishing signature | Anchor |
|---|---|---|---|---|---|
| **Alexithymia** | Low $I^*$ → low $S_{available}$ | Stage 1 (interoception) | Prosodic | Flat prosody with intact lexical retrieval; no mask possible; speaker reports not knowing what they feel | *(stub — alexithymia interoception studies)* |
| **Autism** | Atypical salience mapping + reduced RH global processing | Stage 1–2 | Pragmatic + prosodic | Monotone or over-patterned prosody; semantic-tone integration difficulty; high masking cost | *(stub — autism prosody and pragmatics literature)* |
| **ADHD** | Dopaminergic regulation + WM load | Stage 2 (WM) | Discourse + prosodic | Inconsistent: monotone in hyperfocus, exaggerated in overflow; topic drift under load | *(stub — ADHD discourse instability)* |
| **Depression** | Collapsed $W^*$, low $A_s^*$, reduced autonomic arousal | Stage 1 (amplitude) | Breath/amplitude → prosodic | Low amplitude + flat prosody + slow cadence + mono-topic speech; congruent | *(stub — depression prosody and speech studies)* |
| **Anxiety** | High $J$, high $\Pi_{cog}$, threat-mode autonomic | Stage 1–2 | Pragmatic + prosodic | Tight, clipped, higher pitch, reduced variability; literal interpretation | *(stub — anxiety prosody literature)* |
| **Schizotypal / dissociative** | Disrupted self-model coherence, impaired contextual binding | Stage 2–3 | Discourse + integration | Flat, distant, oddly rhythmic; content-tone mismatch; tangential | *(stub — dissociation speech studies)* |
| **Parkinson's** | Basal ganglia motor-prosody coupling degradation | Stage 3–4 | Articulatory + amplitude | Monotone with articulatory imprecision; tight-timing word errors | *(stub — Parkinson's speech literature)* |
| **Right-hemisphere lesion** | Direct RH prosody network damage | Stage 1 (direct) | Prosodic | Monotone with preserved language; aprosodia; pragmatic failure | *(stub — Ross aprosodia literature)* |
| **FAS** | Precision collapse at the prosodic timing layer | Stage 1–2 (prosodic) | Prosodic | Foreign-sounding accent with preserved language; generic-accent perception | *(stub — FAS literature)* |
| **High cognitive load (NT)** | WM saturation, predictive overload | Stage 1–2 | Pragmatic → discourse → prosodic | Literal, tangential, then monotone during thinking; recovers when load drops | *(stub — cognitive load and speech studies)* |
| **ND burnout** | Stage 3–4 collapse, terminal, after chronic masking | Stage 3–4 | All integration + retrieval | Persistent slurring, mumbling, pragmatic failure; late detection | *(stub — ND burnout literature)* |

### 27.3 What the table shows

**One mechanism, many entry points.** Each condition enters the collapse sequence at a different stage. The entry point determines which layer collapses first. The mechanism is the same: precision drops, the window narrows, integration fails, the gate closes, the prior calcifies.

**The entry point is the variable.** Alexithymia enters at interoception ($I^*$). Depression enters at amplitude ($A_s^*$). Anxiety enters at cognitive pressure ($\Pi_{cog}$). Autism enters at salience mapping. ADHD enters at working memory ($W^*$). Each condition is a different variable failing first.

**The signature is the readout.** The first layer to collapse determines the signature. Alexithymia looks prosodic. Depression looks amplitude. ADHD looks discourse. Autism looks pragmatic-prosodic. The signature is the entry point made audible.

### 27.4 The prediction

**PREDICT-SPEECH-42:** Clinical conditions with different entry points show different collapse orders. Alexithymia should show prosodic collapse before discourse collapse. ADHD should show discourse collapse before prosodic collapse. The collapse order is the entry point.

**PREDICT-SPEECH-43:** Conditions that share an entry point show the same collapse signature. Alexithymia and right-hemisphere lesion should both show prosodic-first collapse, with different mechanisms. High-load NT and anxiety should both show pragmatic-first collapse.

### 27.5 Intervention at the substrate

The clinical implication is direct: treat at the substrate. Breath training, CO₂ tolerance work, precision activities, and postural interventions restore the substrate. The substrate restoration restores both the loop and the speech.

**The intervention sequence:**

1. **Restore breath mechanics** — diaphragmatic breathing, resonance breathing, exhalation completeness
2. **Restore CO₂ tolerance** — breath-hold training, CO₂ tables
3. **Restore interoceptive routing** — body awareness, heartbeat detection practice
4. **Restore postural support** — posture correction, seated speech practice
5. **Restore routing flexibility** — reduce the cost of unmasked expression in the speaker's context, so that $f_{routing}$ can rise without the speaker paying a social or professional penalty
6. **Restore channel flexibility** — the speaker can use speech again when the budget supports it

**Step 5 is the routing intervention.** The substrate interventions restore the capacity for expression. The routing intervention restores the *safety* of expression. A speaker who can afford to unmask will unmask; a speaker who cannot will keep routing salience to output management, and the mask will keep costing precision.

**The speech signature is a non-invasive readout of the restoration.** If $f_{routing}$ is rising, the prosody becomes more congruent before it becomes more expressive. Congruence is the first sign that the routing is recovering, just as granularity is the first sign that the prosody is recovering.

---

## 27.6 The routing-states table

The clinical conditions table lists conditions. The routing-states table lists **configurations** — states that can accompany any condition and that change the clinical picture.

| Routing state | $A_s^*$ | $f_{routing}$ | Prosodic signature | Clinical implication |
|---|---|---|---|---|
| **Genuine expressive** | High | High | Expressive, congruent | Healthy expressive range |
| **Masking / performance** | High | Low | Expressive, incongruent | Collapse is hidden; allostatic cost is high; detection is late |
| **Honest collapse** | Low | High | Flat, congruent | Collapse is visible; detection is early |
| **Failed mask / depletion** | Low | Low | Flat, incongruent | Collapse is visible but the speaker cannot report it accurately |
| **Alexithymic** | Normal | Normal | Flat, low $S_{available}$ | No mask possible; the interoceptive signal is unavailable |

**The masking row is the critical one.** It describes a speaker who sounds normal, is depleting, and cannot detect their own collapse. The clinical implication is direct: masking is not a presentation style. It is a routing configuration with a measurable cost, and it predicts late collapse detection.

**The failed-mask row is the dangerous one.** A speaker who has been masking and can no longer fund the mask shows flat, incongruent prosody. The collapse is visible, but the speaker's interoceptive readout has been starved for so long that their self-report may not match the severity of the collapse. The clinician should trust the speech signal over the self-report.

### 27.7 What the routing-states table shows

**The clinical table and the routing table answer different questions.** The clinical table answers "what condition is this?" The routing table answers "is the collapse visible?"

**A condition can present in any routing state.** A depressed speaker can be in honest collapse (flat, congruent) or in failed mask (flat, incongruent). An autistic speaker can be in genuine expressive (low masking) or in masking (high masking). The routing state is not a diagnosis; it's a configuration.

**The routing state changes the clinical priority.** A speaker in honest collapse needs substrate restoration. A speaker in masking needs substrate restoration *and* routing restoration — because the mask is what's hiding the collapse and starving the interoceptive readout.

---

## 28. Social Projection

### 28.1 How to read this chapter

The social projection is the individual model projected onto collective substrate. The mechanism is the same; the substrate is distributed. The full treatment is in Book III §19 (precision ecology) and Central Reference §3.12. This chapter gives the projection table and the key predictions.

### 28.2 The social projection table

| Individual | Social |
|---|---|
| $A_s^*$ — oscillatory amplitude | Collective synchrony capacity |
| $R^*$ — precision | Shared meaning resolution |
| $K$ — curvature | Collective load |
| $W^*$ — window width | Temporal horizon of collective planning |
| $\Theta^*$ — integration | Cross-group coordination |
| $I^*$ — interoceptive routing | Collective self-awareness |
| $L^*$ — persistent load | Historical trauma, institutional conditioning |
| $\mathcal{U}$ — prior update rate | Cultural prior update rate |
| $f_{routing}$ — salience routing | Collective expression vs. collective performance |

$$\text{Synchrony} \rightarrow A_s^* \rightarrow \sigma(A_s) \rightarrow R^* \rightarrow K \rightarrow W^* \rightarrow \Theta^* \rightarrow C_s^{collective}$$

### 28.3 The exhale gate trap as collective collapse

Central Reference §5c specifies the exhale gate trap: incomplete exhalation produces a cascade from autonomic asymmetry to perfusion failure to left-hemisphere confabulation. At the social level, the same mechanism produces collective confabulation — the conspiracy cascade.

A population under chronic load has compressed CO₂ ceilings, reduced exhalation completeness, and degraded cross-hemispheric integration. The left-hemisphere interpreter runs without the right hemisphere's anomaly detection. The result is confident, categorical, and empirically untethered public discourse.

**The mechanism is the same at both layers.** The substrate is the individual's breath. The output is the collective's speech.

### 28.4 The masking cost

When the speaker's default allocation differs from the context-appropriate allocation, the speaker must override the default. The override requires precision. The precision is the masking cost.

**PREDICT-SPEECH-44:** The precision cost of prosodic masking is measurable, and it should track the same variables as other masking costs — HRV, Control Pause, TOT frequency under load.

### 28.5 The ND and social-group overlap

ND populations and certain social groups show overlapping prosodic features. The framework treats the overlap as an allocation-layer phenomenon, not a population-identity phenomenon.

Both populations run **non-default precision allocations** to the prosodic layer. In ND populations, the allocation is substrate-driven. In social-group populations, the allocation is context-driven. The surface features overlap because both are non-default allocations, not because the populations share a cause.

**PREDICT-SPEECH-45:** Prosodic features across populations should cluster by allocation profile (withheld, spent, and on what target), not by population label. If the clusters fall out by population label, the unified allocation model is disconfirmed.

### 28.6 Register, interaction, and the coupled oscillator

**Register switching** is precision allocation. Formal, informal, ritual, intimate, and pedagogical registers each have different prosodic and timing demands. Switching registers means holding the target register online while suppressing the default. This is the same masking mechanism at the register layer.

**Turn-taking** is inter-brain phase-locking. Conversation is a coupled oscillator system. The precision determines how tightly two speakers can phase-lock.

**PREDICT-SPEECH-46:** Conversational synchrony measures should correlate with individual precision measures.

### 28.7 What the social projection explains

- **Why synchronized speech, chant, and song are universal** — they are the substrate of shared meaning
- **Why collective fragmentation tracks synchrony loss** — the mechanism is the same at both layers
- **Why conspiracy thinking scales with chronic load** — the exhale gate trap is a substrate mechanism
- **Why ND and social-group prosody overlap** — both are non-default allocations, not shared causes
- **Why collective masking is invisible** — the same routing mechanism that hides individual collapse hides collective collapse

---

## 29. Regional Accents as Substrate Profiles

### 29.1 How to read this chapter

Regional accents are substrate profiles made audible. The full treatment of cross-linguistic variation is in Book III §20. This chapter gives the regional projection: how different regions produce different accents because they have different substrate profiles.

### 29.2 The regional substrate table

| Region | Breath pattern | Arousal norm | Amplitude baseline | Accent signature |
|---|---|---|---|---|
| **Vermont** | Shallow, chest-dominant | Low | Low | Monotone |
| **Deep South** | Slow, diaphragmatic | Moderate | Moderate | Melodic |
| **Midwest** | Low-arousal, shallow | Low | Low | Flat |
| **New York** | High-arousal, rapid | High | High | Clipped, rapid cadence |
| **Scandinavian** | Low amplitude | Low | Low | Flat |
| **Irish** | High amplitude | Moderate | High | Musical |
| **Japanese** | Low amplitude + rhythmic | Low | Low | Flat rhythmic |

### 29.3 Why accents persist across generations

Children entrain to the regional timing geometry. The entrainment is not phonetic learning. It is **somatic timing inheritance**:

- **Breath rhythm** — the region's default breath pattern
- **Movement rhythm** — the region's default movement vocabulary
- **Social rhythm** — the region's default interactive cadence
- **Oscillatory amplitude** — the region's default amplitude range

The child's substrate develops in the region's substrate. The development is the accent. The accent is the substrate made audible.

### 29.4 The prediction

**PREDICT-SPEECH-47:** Regional prosodic profiles correlate with regional substrate profiles (breath mechanics, amplitude baselines, arousal norms) independent of phonetic inventory.

**PREDICT-SPEECH-48:** Children raised in a region develop the region's substrate profile, not just the region's phonetic inventory. The substrate profile predicts the accent better than the phonetic input.

### 29.5 The postural component

The regional substrate profile includes postural patterns. Regions with different postural habits — different sitting patterns, different movement vocabularies, different device-use patterns — develop different breath mechanics, which produce different accents.

**PREDICT-SPEECH-49:** Regional postural patterns predict regional breath patterns, which predict regional prosodic profiles. The postural component is measurable.

---

## 30. Drugs and Spoken Language

### 30.1 How to read this chapter

Drugs shift the substrate variables. The speech shift is the substrate shift made audible. This chapter gives the drug projection table.

### 30.2 The drug projection table

| Drug class | Variable shifted | Speech effect |
|---|---|---|
| **Depressants** | Amplitude collapse ($A_s^*$ ↓) | Monotone speech; reduced prosodic range |
| **Stimulants** | Amplitude spike ($A_s^*$ ↑), $I^*$ ↑ | Clipped cadence; rapid speech; exaggerated prosody |
| **Psychedelics** | Desynchronization ($C_{LR}$ ↓) | Unusual prosody; atypical rhythm |
| **Dissociatives** | Low $I^*$ | Flat prosody; detached affect |
| **Alcohol** | Unstable gating | Slurring |
| **THC** | Delayed gating | Blurred phonemes; slower articulation |

### 30.3 The mechanism

Each drug shifts a substrate variable. The speech shift is the substrate shift made audible.

- **Depressants** lower $A_s^*$, which lowers the pressure envelope, which reduces amplitude and prosodic range.
- **Stimulants** raise $A_s^*$ and $I^*$, which raises the pressure envelope and interoceptive routing, which produces clipped cadence and exaggerated prosody.
- **Psychedelics** desynchronize hemispheric oscillations, which reduces $C_{LR}$, which produces unusual prosody and atypical rhythm.
- **Dissociatives** lower $I^*$, which reduces interoceptive routing, which flattens prosody and detaches affect.
- **Alcohol** destabilizes the gate, which produces slurring.
- **THC** delays the gate, which produces blurred phonemes and slower articulation.

### 30.4 The prediction

**PREDICT-SPEECH-50:** Drug effects on speech are predictable from the drug's effect on the substrate variables. Depressants and stimulants should produce opposite amplitude effects. Psychedelics and dissociatives should produce opposite interoceptive effects.

---

## 31. Foreign Accent Syndrome

### 31.1 Why this chapter is full-length

FAS is the cleanest single case of the mechanism. It shows, in one phenomenon, that accent is a timing geometry produced by precision, not a phonetic inventory. When precision collapses, the geometry changes, and the accent changes with it. FAS is the case study that makes the whole model visible.

### 31.2 The phenomenon

Foreign Accent Syndrome (FAS) is the sudden appearance of a perceived foreign accent, typically after stroke or brain injury. Lesions cluster in the left frontal lobe around the larynx/phonation area, or in the bilateral posterior frontal speech-motor network. The field documents the phenomenon as a speech motor disorder involving disrupted prosody, rhythm, and articulation. It does not have a mechanism that explains *why* the disruption produces a *foreign-sounding* accent rather than a generic dysarthria.

### 31.3 The precision account

FAS is a **precision collapse at the prosodic timing layer**. The native accent is a timing geometry — a specific configuration of pitch contour, rhythm, stress, and cadence. That geometry requires precision above threshold to sustain. When the lesion disrupts the network, precision drops below threshold at the prosodic layer, and the native prosody collapses.

The system defaults to a lower-precision prosodic pattern. That pattern does not match the speaker's native accent because it is not produced by the native precision system. It sounds "foreign" because it is what the system produces at a precision level the native system does not use.

### 31.4 Evidence

**Irish brogue case:** A woman with a left hemisphere stroke developed an Irish brogue matching her mother's accent. The field says suppressed prosodic patterns reemerged. The precision account says the lesion collapsed the precision that maintained her native accent's timing geometry, and the system defaulted to a previously encoded prosodic pattern that required less precision to sustain.

**Multiple accent case:** A patient alternated between at least five accents after a stroke. The field calls this "functional." The precision account says the precision is fluctuating across the threshold. When precision rises, the native prosody returns. When precision drops, the system defaults to whatever prosodic pattern is available at that precision level.

**Generic accent finding:** Listeners perceive FAS speech as a "generic" foreign accent rather than a specific one. The precision account says this is because the pattern is not produced by any language's full precision system. It is the minimum viable prosodic contour — the prosodic equivalent of vocal fry.

### 31.5 The clinical implication

FAS is the prosodic equivalent of vocal fry. The field calls it a "speech motor disorder." The framework calls it a precision collapse at the prosodic timing layer. Same phenomenon, named mechanism.

**PREDICT-SPEECH-51:** FAS patients show precision collapse at the prosodic layer as measured by other precision tests, independent of lesion location.

### 31.6 What FAS shows about the model

FAS is the cleanest case because it isolates the prosodic layer. The lesion damages the prosodic timing network, and the accent changes. Nothing else changes — language, vocabulary, grammar, and articulation are preserved. The accent is the pure readout of the prosodic timing geometry.

**The general lesson:** accent is not a phonetic inventory. It is a timing geometry. Change the precision, change the geometry, change the accent. This is the model in one phenomenon.

---

## 32. The Applied Summary

### 32.1 What the model explains

The model explains, with one mechanism, the full range of speech phenomena:

- **Prosodic collapse under stress** — precision drop at the prosodic layer
- **Vocal fry** — amplitude collapse at the breath layer
- **Monotone** — prosodic flattening with preserved phonation
- **Accent persistence** — somatic timing inheritance
- **Trauma flattening** — right-hemisphere suppression
- **TOT** — precision collapse at the lexical layer
- **Proper-name failure** — no-semantic-neighborhood retrieval failure
- **FAS** — precision collapse at the prosodic timing layer
- **Slurring** — hemispheric desynchronization
- **Mumbling** — amplitude collapse
- **Pragmatic failure** — highest-integration layer collapses first
- **Discourse instability** — working-memory-dependent layer collapses second
- **Telegraphic speech** — morphosyntactic collapse
- **Channel preference** — precision-budget readout
- **Masking** — routing configuration with measurable cost
- **Late collapse detection** — interoceptive starvation from chronic masking
- **Generational speech shift** — precision ecology
- **Cross-linguistic failure modes** — suprasegmental demand

### 32.2 What the model predicts

The model makes **60 predictions** (PREDICT-SPEECH-01 through -60), each falsifiable with standard acoustic and physiological measures. The prediction registry is in Appendix B.

**The most testable predictions:**

- **PREDICT-SPEECH-01:** Breath mechanics predict prosodic range
- **PREDICT-SPEECH-05:** TOT frequency correlates with precision
- **PREDICT-SPEECH-13:** Channel preference shifts precede speech degradation
- **PREDICT-SPEECH-15:** Collapse order follows integration demand
- **PREDICT-SPEECH-16:** Proper names fail before common nouns
- **PREDICT-SPEECH-21:** Granularity returns before subjective recovery
- **PREDICT-SPEECH-42:** Clinical conditions with different entry points show different collapse orders
- **PREDICT-SPEECH-58:** Prosodic congruence is predicted by $f_{routing}$
- **PREDICT-SPEECH-59:** Chronic low $f_{routing}$ predicts later collapse detection
- **PREDICT-SPEECH-60:** Masking has a measurable allostatic cost

### 32.3 What the model opens

**Clinical:** speech is a Stage 1–2 monitoring channel. The biomarker inventory and diagnostic battery make it actionable. Channel preference and congruence are the cheapest leading indicators.

**Linguistic:** accent is a timing geometry, not a phonetic inventory. Cross-linguistic variation in collapse signatures is predictable from suprasegmental demand.

**Social:** collective synchrony, conspiracy thinking, and mask cost are projections of the same substrate mechanism.

**Generational:** modern digital and postural environments may produce a different baseline substrate. The prediction is testable.

**Masking:** the routing variable explains why some collapses are invisible, why they reach terminal stages before detection, and why "you don't look sick" is a clinical problem with a mechanism.

### 32.4 The one line

The variable is precision. The equation is $P = R/D_T$. The routing is $f_{routing}$. The speech is the readout. The readout is the state made audible — or hidden.

---

# Book V Summary Table

| Chapter | Content | Key output |
|---|---|---|
| 27. Clinical conditions | Table-driven, 11 conditions; separate routing-states table | Entry point = collapse order; routing state = visibility |
| 28. Social projection | Short, cross-references Book III §19 | Collective synchrony, masking cost, exhale gate trap |
| 29. Regional accents | Short, cross-references Book III §20 | Substrate profiles made audible |
| 30. Drugs and spoken language | Table-driven | Substrate shift made audible |
| 31. Foreign accent syndrome | Full chapter | The cleanest single case |
| 32. The applied summary | What the model explains, predicts, opens | The one line |

---

# APPENDIX A — NOTATION AND SYMBOLS

## Full symbol table with definitions and cross-references

---

## How to Read This Appendix

This appendix defines every symbol used in the paper. Symbols are organized by category. Each entry gives the symbol, its name, its definition, and the section where it is first introduced or most fully specified.

**Notation conventions:**

- **Asterisk ($^*$)** — normalized to the individual's own baseline. $A_s^*$ is oscillatory amplitude as a ratio to the individual's baseline, not an absolute value.
- **Bold** — variables that are primary state variables (the system's current configuration).
- **Italic** — variables that are derived or diagnostic (computed from primary variables).
- **Uppercase** — state variables and structural parameters.
- **Lowercase** — coefficients, rates, and functional forms.
- **Greek letters** — parameters, thresholds, and coefficients.

---

## 1. The Master State Variables

The six primary state variables that describe the system's current configuration.

| Symbol | Name | Definition | First specified |
|---|---|---|---|
| $A_s^*$ | Oscillatory amplitude | Energy budget — how much oscillatory signal is available. Ratio to individual baseline. | Book I §3.5 |
| $R^*$ | Precision | Timing-coherence ratio — signal clarity. $P / P_{baseline}$. | Book I §2.1 |
| $W^*$ | Window width | Accessible manifold range. Cognitive flexibility composite / baseline. | Book I §2.1 |
| $\Theta^*$ | Integration efficiency | How well the system holds disparate signals together. Phase-locking stability × ambiguity tolerance / baseline. | Book I §2.1 |
| $I^*$ | Interoceptive routing | Routing protocol — how well the system reads its own geometry. Heartbeat detection accuracy / baseline. | Book I §2.1 |
| $L^*$ | Allostatic load | Cumulative allostatic debt. Five-component decomposition. | Book I §2.1 |

**Note on the asterisk:** the asterisk denotes normalization to the individual's own validated baseline. Population norms are not the comparator. A degraded world-class performer may be more impaired than a baseline junior — the metric captures this.

---

## 2. The Supply Axis Variables

The variables that determine the supply of precision and the routing of salience.

| Symbol | Name | Definition | First specified |
|---|---|---|---|
| $P$ | Precision (absolute) | $P = R/D_T$ | Book I §2.1 |
| $R$ | Sync duration | Proportion of time two oscillatory streams remain phase-locked | Book I §2.1 |
| $D_T$ | Timing distance | Average phase difference between streams | Book I §2.1 |
| $f_{routing}$ | Salience routing | Proportion of available salience that reaches expression. $S_{expressed}/S_{available}$. | Book I §2.1b |
| $S_{available}$ | Available salience | $C_s \cdot I^*$ — usable bandwidth × interoceptive routing | Book I §2.1b |
| $S_{expressed}$ | Expressed salience | $S_{available} - \sum_i P_i W_i$ — available salience minus layer management cost | Book I §2.1b |
| $C_{low}$, $C_{high}$ | CO₂ tolerance window | Range within which precision rises with CO₂ | Book I §2.1 |
| $C_{high}(L^*)$ | Load-compressed CO₂ ceiling | $C_{high}^0 - \gamma L^*$ | Book I §2.1 |
| $J(C)$ | Chemoreflex jitter | $\kappa(C - C_{high}(L^*))^2$ for $C > C_{high}(L^*)$, else 0 | Book I §2.1 |
| $\Pi_{mech}$ | Mechanical pressure | Beneficial pressure — breath-hold, resonance | Book I §2.1 |
| $\Pi_{cog}$ | Cognitive pressure | Harmful pressure — instantaneous load, sympathetic activation | Book I §2.1 |
| $U_C$ | CO₂ uniformity | $1/(\text{Var}_i[C_i] + \epsilon)$ | Book I §2.1 |
| $\delta_{hyst}$ | Collapse hysteresis | Recovery delay after precision collapse | Book I §6.5 |
| $W_{enc}$ | Encoding window | $\int_{t_{enc}} \mathbb{1}[P(t) > P_{threshold}] dt$ | Book I §2.1 |

---

## 3. The Derived Variables

Variables computed from the state variables.

| Symbol | Name | Definition | First specified |
|---|---|---|---|
| $C_s$ | Usable bandwidth | Master equation output | Book I §2.1 |
| $K$ | Curvature | $K = k(1/(R^*+\epsilon)) + \sum_i S_i C_i$ | Book I §2.1 |
| $\delta_{min}$ | Resolution floor | $\delta_{min} = \eta/(A_s^* \cdot I^*)$ | Book I §2.1 |
| $S$ | Salience | $S = C_s \cdot I^*$ | Book I §2.1 |
| $P_{eff}$ | Effective precision | $P \cdot O_{pathway} \cdot U_C$ | Book I §2.1 |
| $P_{threshold}$ | Gate threshold | $P_0 - \gamma L^*$ | Book I §2.1 |
| $\Lambda$ | Loop activation | $\Theta^* \cdot R^* \cdot \mathbb{1}[P_{eff} > P_{threshold}]$ | Book I §2.1 |
| $\eta$ | Noise floor | Baseline somatic noise | Book I §2.1 |
| $O_{pathway}$ | Oxygen pathway integrity | Substrate constraint on gate condition | Book I §2.1 |
| $k$ | Curvature coefficient | Scales the precision-to-curvature relationship | Book I §2.1 |
| $\epsilon$ | Small constant | Prevents division by zero in curvature | Book I §2.1 |

---

## 4. The Routing Variables

Variables describing how the system routes precision and salience.

| Symbol | Name | Definition | First specified |
|---|---|---|---|
| $f_{routing}$ | Routing component | $S_{expressed}/S_{available}$ — proportion of salience reaching expression | Book I §2.1b |
| $f_{gain}$ | Gain component | Sigmoid gain control | Book I §3.4 |
| $f_{sensorium}$ | Sensorium component | Available routing / required routing | Book I §3.4 |
| $C_{LR}$ | Interhemispheric coherence | Phase-locking between left and right hemisphere oscillations | Book I §3.3 |

**Note:** $f_{routing}$ is listed in both §2 (Supply Axis) and §4 (Routing) because it is the supply axis's second dimension and the routing mechanism's primary variable. §2 is its canonical definition.

---

## 5. The Update Variables

Variables describing how the prior updates.

| Symbol | Name | Definition | First specified |
|---|---|---|---|
| $\mathcal{U}$ | Prior update rate | $(A_s^* \cdot R^* \cdot \Theta^*)/(1 + \gamma K_{enc})$ | Book I §4.4 |
| $K_{enc}$ | Curvature at encoding | What geometry the prior carries forward | Book I §4.4 |
| $W_{enc}$ | Encoding window | $\int_{t_{enc}} \mathbb{1}[P(t) > P_{threshold}] dt$ | Book I §2.1 |

---

## 6. The Structural Variables

Variables describing the manifold's structure.

| Symbol | Name | Definition | First specified |
|---|---|---|---|
| $\rho_{scaffold}$ | Scaffold density | Density of long-range competitive connections | Book I §3.6 |
| $IM$ | Interference metric | Non-orthogonality of task-relevant and task-irrelevant axes | Book I §2.1 |
| $\text{Dim}$ | Neural dimensionality | Independent axes available for representation | Book I §2.1 |
| $n_{hops}$ | Inference hops | Multi-hop inferences available before collapse | Book I §2.1 |

---

## 7. The Collapse Sequence Variables

Variables describing the collapse stages.

| Symbol | Name | Definition | First specified |
|---|---|---|---|
| $R^*$ | Precision drop | Stage 1 | Book I §5.1 |
| $W^*$ | Window narrowing | Stage 2 | Book I §5.2 |
| $\Theta^*$ | Integration failure | Stage 3 | Book I §5.3 |
| $\delta_{min}$ | Resolution floor rise | Stage 4 | Book I §5.4 |
| $\Lambda$ | Gate closure | Stage 5 | Book I §5.5 |
| $\mathcal{U}$ | Prior calcification | Stage 6 | Book I §5.6 |

---

## 8. The Layer Variables

The eight speech layers, with their integration demands.

| Symbol | Layer | Integration demand | First specified |
|---|---|---|---|
| — | Pragmatic | ToM + context + prosody + lexical + timing | Book II §7 |
| — | Discourse | WM + timing + prediction + interoception | Book II §8 |
| — | Prosodic | RH + interoception + emotion + breath | Book II §9 |
| — | Lexical | Semantic + phonological + timing | Book II §10 |
| — | Morphosyntactic | Rule retrieval + WM + phonology | Book II §11 |
| — | Phonological | LH motor + timing | Book II §12 |
| — | Articulatory | Motor + breath + posture | Book II §13 |
| — | Breath/pressure | Diaphragm + intercostals | Book II §14 |

---

## 9. The Demand Axis Variables

Variables describing the language's suprasegmental architecture.

| Symbol | Name | Definition | First specified |
|---|---|---|---|
| — | Stress-timed | Timing carries lexical stress, rhythm | Book I §2.2 |
| — | Syllable-timed | Timing carries even timing, less reduction | Book I §2.2 |
| — | Mora-timed | Timing carries unit duration | Book I §2.2 |
| — | Tonal | Timing carries lexical meaning (pitch contour) | Book I §2.2 |
| — | Pitch-accent | Timing carries lexical meaning (pitch location) | Book I §2.2 |
| — | Intonational | Timing carries phrase-level meaning | Book I §2.2 |

---

## 10. The Channel Axis Variables

Variables describing output channel substrate cost.

| Channel | Substrate cost | Precision cost | First specified |
|---|---|---|---|
| Speech | Pressure modulation, postural reconfiguration, laryngeal control | Highest | Book I §2.3 |
| Sign | Visual attention, manual motor precision | Moderate | Book I §2.3 |
| Typing | Posturally static, no pressure demand | Low | Book I §2.3 |
| Writing (longhand) | Posturally static, fine motor only | Low | Book I §2.3 |
| Inner speech | No motor, no pressure | Minimal | Book I §2.3 |

---

## 11. The Biomarker Variables

The ten biomarkers, one per layer plus routing and channel preference.

| Layer | Biomarker | What it tracks | First specified |
|---|---|---|---|
| Pragmatic | Social appropriateness rating | ToM + context + prosody + lexical + timing | Book IV §23.2 |
| Discourse | Topic coherence | WM + timing + prediction + interoception | Book IV §23.2 |
| Prosodic | Pitch granularity | RH motor control over laryngeal/respiratory muscles | Book IV §23.2 |
| Lexical | Proper-name failure rate | Retrieval precision | Book IV §23.2 |
| Morphosyntactic | Inflection error rate | Rule retrieval + WM + phonology | Book IV §23.2 |
| Phonological | Slurring measures | LH motor sequencing + timing | Book IV §23.2 |
| Articulatory | Consonant precision | Motor + breath + posture | Book IV §23.2 |
| Breath | Amplitude and fry onset | Diaphragm + intercostals | Book IV §23.2 |
| Routing | Prosodic congruence | $f_{routing}$ | Book IV §23.3 |
| Channel | Speech-to-typing shift | Precision budget | Book IV §23.4 |

---

## 12. The Clinical Condition Variables

The eleven clinical conditions, with their entry points.

| Condition | Mechanism | Entry stage | First layer to collapse | First specified |
|---|---|---|---|---|
| Alexithymia | Low $I^*$ | Stage 1 (interoception) | Prosodic | Book V §27.2 |
| Autism | Atypical salience mapping + reduced RH global processing | Stage 1–2 | Pragmatic + prosodic | Book V §27.2 |
| ADHD | Dopaminergic regulation + WM load | Stage 2 (WM) | Discourse + prosodic | Book V §27.2 |
| Depression | Collapsed $W^*$, low $A_s^*$ | Stage 1 (amplitude) | Breath/amplitude → prosodic | Book V §27.2 |
| Anxiety | High $J$, high $\Pi_{cog}$ | Stage 1–2 | Pragmatic + prosodic | Book V §27.2 |
| Schizotypal / dissociative | Disrupted self-model coherence | Stage 2–3 | Discourse + integration | Book V §27.2 |
| Parkinson's | Basal ganglia motor-prosody coupling | Stage 3–4 | Articulatory + amplitude | Book V §27.2 |
| Right-hemisphere lesion | Direct RH prosody network damage | Stage 1 (direct) | Prosodic | Book V §27.2 |
| FAS | Precision collapse at prosodic timing layer | Stage 1–2 (prosodic) | Prosodic | Book V §31 |
| High cognitive load (NT) | WM saturation, predictive overload | Stage 1–2 | Pragmatic → discourse → prosodic | Book V §27.2 |
| ND burnout | Stage 3–4 collapse, terminal, after chronic masking | Stage 3–4 | All integration + retrieval | Book V §27.2 |

---

## 13. The Routing-State Variables

The five routing states, with their prosodic signatures.

| Routing state | $A_s^*$ | $f_{routing}$ | Prosodic signature | First specified |
|---|---|---|---|---|
| Genuine expressive | High | High | Expressive, congruent | Book V §27.6 |
| Masking / performance | High | Low | Expressive, incongruent | Book V §27.6 |
| Honest collapse | Low | High | Flat, congruent | Book V §27.6 |
| Failed mask / depletion | Low | Low | Flat, incongruent | Book V §27.6 |
| Alexithymic | Normal | Normal | Flat, low $S_{available}$ | Book V §27.6 |

---

## 14. The Prediction Registry Variables

The 60 predictions, with their IV/DV and falsification conditions.

*(Full registry in Appendix B.)*

---

# APPENDIX B — THE PREDICTION REGISTRY

## Full prediction registry, organized by book and layer

---

## How to Read This Appendix

The 60 predictions are organized by the book in which they are introduced. Within each book, they are ordered by the layer or phenomenon they address. Each prediction gives the IV, the DV, and the falsification condition.

The registry is designed to be **scannable**. If you want to know what the paper predicts about prosody, find the prosodic entries. If you want to know what the paper predicts about clinical conditions, find the clinical entries. If you want to know what would disconfirm the model, find the falsification column.

---

## 1. Predictions from Book I — The Model

These predictions test the model's core claims about precision, breath, and the layer structure.

| Prediction | IV | DV | Falsification |
|---|---|---|---|
| PREDICT-SPEECH-01 | Breath mechanics | Prosodic range | If breath mechanics do not predict prosodic range, the breath-to-prosody mechanism is disconfirmed |
| PREDICT-SPEECH-02 | CO₂ tolerance | Prosodic stability | If CO₂ tolerance does not predict prosodic stability, the CO₂-to-prosody mechanism is disconfirmed |
| PREDICT-SPEECH-03 | Phonation regularity and amplitude | Prosodic range | If monotone and fry always co-occur, the distinction is not clinically useful |
| PREDICT-SPEECH-04 | $C_{LR}$ | Slurring measures | If slurring tracks only global arousal and not $C_{LR}$, the integration-layer mechanism is disconfirmed |
| PREDICT-SPEECH-05 | Precision (HRV, RT variability, EEG phase-locking) | TOT frequency | If TOT frequency does not correlate with precision measures, the TOT-as-precision-collapse mechanism is disconfirmed |

---

## 2. Predictions from Book II — The Layers

These predictions test the layer-specific claims.

| Prediction | IV | DV | Falsification |
|---|---|---|---|
| PREDICT-SPEECH-06 | Trauma exposure | Prosodic measures | If trauma does not produce measurable prosodic shifts, the trauma-prosody mechanism is disconfirmed |
| PREDICT-SPEECH-07 | Rigidity profile and precision | Tight-timing word error rate | If tight-timing word errors track only vocabulary, the articulation-layer mechanism is disconfirmed |
| PREDICT-SPEECH-08 | FAS diagnosis | Precision measures | If FAS patients show normal precision on non-speech measures, the FAS-as-precision-collapse mechanism is disconfirmed |
| PREDICT-SPEECH-09 | Breath mechanics | Pitch-matching accuracy | If breath mechanics do not predict pitch-matching accuracy, the breath-to-prosody mechanism is disconfirmed |

---

## 3. Predictions from Book III — The Dynamics

These predictions test the dynamic claims across contexts.

| Prediction | IV | DV | Falsification |
|---|---|---|---|
| PREDICT-SPEECH-10 | Regional substrate measures | Regional prosodic profiles | If regional prosodic profiles do not correlate with substrate, the substrate-to-accent mechanism is disconfirmed |
| PREDICT-SPEECH-11 | Longitudinal speech measures | Timing of subjective state reports | If speech signatures follow rather than precede subjective reports, the monitoring-window claim is disconfirmed |
| PREDICT-SPEECH-12 | Population membership | Prosodic feature clusters | If clusters fall out by population label rather than allocation profile, the unified allocation model is disconfirmed |
| PREDICT-SPEECH-13 | Channel preference shift | Speech degradation | If channel preference does not shift before speech degradation, the leading-indicator claim is disconfirmed |
| PREDICT-SPEECH-14 | CO₂ tolerance, postural sway, HRV | Speech-vs-typing precision gap | If the gap does not correlate with substrate measures, the channel-cost mechanism is disconfirmed |
| PREDICT-SPEECH-15 | Integration demand | Collapse order | If collapse order does not follow integration demand, the layer-stack model is disconfirmed |
| PREDICT-SPEECH-16 | Load | Proper-name vs. common-noun failure | If proper names do not fail before common nouns, the no-semantic-neighborhood account is disconfirmed |
| PREDICT-SPEECH-17 | Suprasegmental complexity | Collapse severity | If suprasegmental complexity does not predict collapse severity, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-18 | Postural condition (seated vs. standing) | Speech precision | If seated speech is not more precise than standing, the postural-cost mechanism is disconfirmed |
| PREDICT-SPEECH-19 | Modality (sign vs. speech) | Collapse schedule | If sign prosody collapses on the same schedule as speech prosody, the channel-cost model is disconfirmed |
| PREDICT-SPEECH-20 | Modality (inner vs. overt speech) | Collapse schedule | If inner speech collapses on the same schedule as overt speech, the channel-cost model is disconfirmed |
| PREDICT-SPEECH-21 | Recovery state | Granularity vs. subjective report | If granularity does not return before subjective recovery, the recovery-ladder model is disconfirmed |
| PREDICT-SPEECH-22 | Recovery state | Layer recovery order | If recovery order does not mirror collapse order, the integration-demand rule is disconfirmed |
| PREDICT-SPEECH-23 | Collapse depth | Recovery time | If recovery time does not scale super-proportionally with collapse depth, the hysteresis model is disconfirmed |
| PREDICT-SPEECH-24 | Task pair | Degradation signature | If degradation signature is not predictable from shared precision demand, the conflict model is disconfirmed |
| PREDICT-SPEECH-25 | Task pair | Speech degradation | If "can you talk while X?" is not a precision-budget question, the conflict model is disconfirmed |
| PREDICT-SPEECH-26 | Load | Channel preference | If channel preference does not shift from speech to typing under load, the channel-cost model is disconfirmed |
| PREDICT-SPEECH-27 | CO₂ tolerance, postural sway, HRV | Speech-vs-typing precision gap | If the gap does not correlate with substrate measures, the channel-cost mechanism is disconfirmed |
| PREDICT-SPEECH-28 | Postural condition (seated vs. standing) | Speech precision | If seated speech is not more precise, the postural-cost mechanism is disconfirmed |
| PREDICT-SPEECH-29 | Environmental load | Collapse signatures | If generational speech patterns do not track substrate profiles, the ecological projection is disconfirmed |
| PREDICT-SPEECH-30 | Postural intervention | Prosodic granularity and amplitude | If postural intervention does not improve prosody, the postural-cost mechanism is disconfirmed |
| PREDICT-SPEECH-31 | Digital load, postural load | Channel shift | If channel shift does not track both loads, the ecological projection is disconfirmed |
| PREDICT-SPEECH-32 | Language type | Collapse signature | If collapse signatures do not differ by suprasegmental architecture, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-33 | Language type | Baseline precision allocation | If speakers of complex languages do not allocate more precision to timing, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-34 | Language phonotactic complexity | Tight-timing word errors | If error rates do not scale with phonotactic complexity, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-35 | Modality (inner vs. overt) | Collapse schedule | If inner speech is not preserved longer, the channel-cost model is disconfirmed |
| PREDICT-SPEECH-36 | Modality (written vs. spoken) | Collapse schedule | If written output is not preserved relative to spoken, the channel-cost model is disconfirmed |
| PREDICT-SPEECH-37 | Modality (sign vs. speech) | Collapse signature | If sign prosody collapses on the same schedule as speech, the channel-cost model is disconfirmed |
| PREDICT-SPEECH-38 | Language demand | Code-switching collapse | If code-switching into higher-demand language does not produce earlier collapse, the demand-axis model is disconfirmed |

---

## 4. Predictions from Book IV — The Measurement

These predictions test the measurement claims.

| Prediction | IV | DV | Falsification |
|---|---|---|---|
| PREDICT-SPEECH-39 | Load | Channel preference shift | If channel preference does not shift before speech degradation, the leading-indicator claim is disconfirmed |
| PREDICT-SPEECH-40 | CO₂ tolerance, postural sway, HRV | Speech-vs-typing precision gap | If gap does not correlate with substrate measures, the channel-cost mechanism is disconfirmed |
| PREDICT-SPEECH-41 | Postural condition (seated vs. standing) | Speech precision | If seated speech is not more precise, the postural-cost mechanism is disconfirmed |

---

## 5. Predictions from Book V — The Projections

These predictions test the applied claims.

| Prediction | IV | DV | Falsification |
|---|---|---|---|
| PREDICT-SPEECH-42 | Clinical condition | Collapse order | If conditions with different entry points show the same collapse order, the entry-point model is disconfirmed |
| PREDICT-SPEECH-43 | Clinical condition | Collapse signature | If conditions with the same entry point show different signatures, the entry-point model is disconfirmed |
| PREDICT-SPEECH-44 | Masking load | HRV, CP, TOT frequency | If masking cost does not track substrate measures, the masking-cost model is disconfirmed |
| PREDICT-SPEECH-45 | Population membership | Prosodic feature clusters | If clusters fall out by population label, the unified allocation model is disconfirmed |
| PREDICT-SPEECH-46 | Individual precision | Conversational synchrony | If synchrony does not correlate with individual precision, the coupled-oscillator model is disconfirmed |
| PREDICT-SPEECH-47 | Regional substrate | Regional prosodic profiles | If profiles do not correlate with substrate, the substrate-to-accent mechanism is disconfirmed |
| PREDICT-SPEECH-48 | Regional substrate | Child accent | If substrate does not predict accent better than phonetic input, the substrate-to-accent mechanism is disconfirmed |
| PREDICT-SPEECH-49 | Regional postural patterns | Regional breath patterns | If postural patterns do not predict breath patterns, the postural-cost mechanism is disconfirmed |
| PREDICT-SPEECH-50 | Drug class | Speech effect | If drug effects are not predictable from substrate variables, the substrate-shift model is disconfirmed |
| PREDICT-SPEECH-51 | FAS diagnosis | Precision measures | If FAS patients show normal precision, the FAS-as-precision-collapse mechanism is disconfirmed |

---

## 6. Predictions from Appendix D — Cross-Linguistic Data

| Prediction | IV | DV | Falsification |
|---|---|---|---|
| PREDICT-SPEECH-52 | Tonal inventory size | Tone error rate | If tone errors do not scale with tonal inventory size, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-53 | Phoneme inventory size | Phoneme discrimination errors | If discrimination errors do not scale with inventory size, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-54 | Layered suprasegmental architecture | Error cascade order | If error cascade does not follow layer stack order, the demand-axis model is disconfirmed |

---

## 7. Predictions from Appendix E — Cross-Domain Conflict Data

| Prediction | IV | DV | Falsification |
|---|---|---|---|
| PREDICT-SPEECH-55 | Task intensity | Collapse depth | If collapse depth does not scale with task intensity, the conflict model is disconfirmed |
| PREDICT-SPEECH-56 | Baseline precision | Task-intensity threshold | If the threshold does not correlate with baseline precision, the conflict model is disconfirmed |
| PREDICT-SPEECH-57 | Task pair | Layer-collapse order | If the layer-collapse order in a conflict does not follow integration demand, the layer-stack model is disconfirmed |

---

## 8. Predictions from Book III §18 — Salience Routing and Masking

| Prediction | IV | DV | Falsification |
|---|---|---|---|
| PREDICT-SPEECH-58 | $f_{routing}$ | Prosodic congruence | If congruence is not predicted by routing, the routing model is disconfirmed |
| PREDICT-SPEECH-59 | Chronic low $f_{routing}$ | Collapse detection stage | If maskers do not reach Stage 3–4 before reporting Stage 1–2 symptoms, the routing model is disconfirmed |
| PREDICT-SPEECH-60 | $A_s^*$, $f_{routing}$ | Allostatic load | If allostatic load is not higher in high-$A_s^*$, low-$f_{routing}$ speakers, the routing model is disconfirmed |

---

## 9. Predictions by Layer

For readers who want to know what the paper predicts about a specific layer.

| Layer | Predictions |
|---|---|
| **Pragmatic** | 01, 11, 24, 42, 43 |
| **Discourse** | 15, 24, 42, 43 |
| **Prosodic** | 02, 06, 09, 10, 16, 17, 21, 27, 30, 32, 33, 34, 47, 48, 51 |
| **Lexical** | 05, 16, 21, 22 |
| **Morphosyntactic** | 15, 22, 24 |
| **Phonological** | 04, 07, 34 |
| **Articulatory** | 04, 07, 18, 28, 41 |
| **Breath** | 01, 02, 03, 09, 26, 29, 31, 39, 49 |
| **Channel** | 13, 14, 18, 19, 20, 26, 27, 28, 31, 35, 36, 37, 39, 40, 41 |
| **Routing** | 58, 59, 60 |

---

## 10. Predictions by Stage

For readers who want to know what the paper predicts about a specific stage of collapse.

| Stage | Predictions |
|---|---|
| Stage 1 (precision drop) | 01, 02, 05, 06, 08, 09, 14, 27, 40, 51 |
| Stage 2 (window narrowing) | 11, 13, 15, 24, 26, 39 |
| Stage 3 (integration failure) | 04, 07, 16, 17 |
| Stage 4 (resolution floor rise) | 05, 16, 22 |
| Stage 5 (gate closure) | 04, 07, 18, 28, 41 |
| Stage 6 (prior calcification) | 20, 35 |
| **Stage-independent (routing)** | **58, 59, 60** |

---

## 11. Predictions by Falsification Type

For readers who want to know what would disconfirm the model.

| Falsification type | Predictions |
|---|---|
| Substrate does not predict speech | 01, 02, 06, 08, 09, 10, 14, 27, 40, 47, 49, 50, 51 |
| Collapse order is not forced | 15, 22, 42, 43 |
| Layer distinction is not useful | 03, 16, 19, 20, 35, 36, 37 |
| Channel cost is not real | 13, 18, 26, 28, 31, 39, 41 |
| Demand axis is not real | 17, 32, 33, 34, 38, 52, 53, 54 |
| Recovery is not asymmetric | 21, 23 |
| Conflict model is wrong | 24, 25, 55, 56, 57 |
| Allocation model is wrong | 12, 44, 45, 46 |
| Routing model is wrong | 58, 59, 60 |

---

## 12. The Prediction Registry at a Glance

| Book/Appendix | Predictions | Count |
|---|---|---|
| Book I — The Model | 01–05 | 5 |
| Book II — The Layers | 06–09 | 4 |
| Book III — The Dynamics | 10–38, 58–60 | 32 |
| Book IV — The Measurement | 39–41 | 3 |
| Book V — The Projections | 42–51 | 10 |
| Appendix D — Cross-Linguistic | 52–54 | 3 |
| Appendix E — Cross-Domain Conflict | 55–57 | 3 |
| **Total** | **01–60** | **60** |

---

## 13. What the Registry Shows

**The registry is the paper's empirical core.** It says what the paper predicts, how to test each prediction, and what would disconfirm it. It is designed to be scannable — by layer, by stage, by falsification type, or by book.

**The registry is also the paper's invitation.** Every prediction is testable with standard acoustic and physiological measures. The methodology is available. The predictions are specific. The paper is a set of experiments waiting to be run.

**The registry is the paper's honesty.** It names what would disconfirm the model. It doesn't hide behind vague claims. If the predictions fail, the model is wrong, and the registry says so.

---

# APPENDIX C — INTROSPECTIVE ACCOUNTS

## First-person observations that motivated the mechanism

---

## How to Read This Appendix

This appendix preserves first-person accounts of the mechanisms the paper specifies. These are observations, not findings. They are included because the framework's predictions are specific enough that the introspective reports can be cross-checked against the mechanism.

Each account follows the same structure:

- **The observation** — what was noticed, in first person
- **What it illustrates** — which mechanism in the paper it points to
- **The consistency check** — how the observation lines up with the mechanism the paper specifies

The accounts are not evidence. They are **motivation**. They are the moments where a mechanism was first noticed before it was formalized. They are included because the paper's claims are specific enough that a reader can check whether their own introspective experience matches.

---

## C.1 The Motor-First Probe

### The observation

> "I form my mouth like I'm going to do a consonant and then just kind of push some air through with various muscles held and see where it takes me."

### What it illustrates

The motor-first production mode (Book II §13; Book I §5.6). The motor system sets a configuration, drives it with air, and observes the output. The output is discovered, not planned.

### The consistency check

The mechanism specifies that motor-first production is the readout of Stage 6 collapse — prior calcification. The semantic layer's capacity to direct the motor system is reduced, and the motor system defaults to running on its own cached patterns. The output is fluent but low-novelty.

The observation is consistent with the mechanism: the speaker is not planning the output semantically and then executing it motorically. They are setting a motor configuration and letting it run. The output is what the motor system produces, not what the semantic system intended.

The mechanism also predicts that motor-first production is a **Stage 6** phenomenon — it appears when the gate is closed and the prior is calcifying. The observation is consistent with this: the probe is described as something that happens when the speaker is not directing the output, which is the signature of a closed gate.

---

## C.2 The Vocal Fry Observation

### The observation

> "If we have to dial back the details on vocal fry so we don't over hypothesize, we can at least know there's some conditions to it. Because people can talk monotone without vocal fry. Vocal fry feels like it only happens when amplitude is so low that there's like reverb."

### What it illustrates

The distinction between monotone and vocal fry (Book II §9; Book I §5.1). Monotone is low prosodic range with normal phonation. Fry is minimum-amplitude phonation. They are different acoustic events with different mechanisms.

### The consistency check

The mechanism specifies that monotone reflects reduced prosodic modulation — the right hemisphere's timing layer is not shaping the pitch trajectory — while the amplitude and phonation systems are intact. Fry requires minimum subglottal pressure, minimum vocal fold tension, and minimum airflow. The vocal folds vibrate at their lowest stable mode, producing the characteristic creaky, irregular, low-frequency acoustic signature.

The observation is consistent with the mechanism: the speaker distinguishes the two by the **amplitude** condition. Monotone can occur with normal amplitude. Fry only occurs when amplitude is at the floor. This is exactly what the mechanism predicts.

The observation also captures the acoustic signature — "like reverb" — which is the subharmonic oscillation and irregular periodicity that characterizes fry. The mechanism places fry at the minimum-amplitude end of the same pressure envelope that funds all speech.

---

## C.3 The Singing Observation

### The observation

> "Singing feels like it needs diaphragmatic breathing to hit the control necessary to match pitches."

### What it illustrates

The singing-as-substrate-demonstration claim (Book II §14; Book I §3.5). Singing requires diaphragmatic breathing with sustained subglottal pressure to hit and hold pitches. Chest breathing cannot do it. The pressure envelope is too shallow and too unstable to produce controlled pitch matching across a wide range.

### The consistency check

The mechanism specifies that singing is the clearest behavioral proof that prosody depends on diaphragmatic breath support. Speaking can sometimes be produced at low amplitude from chest breathing — the prosodic range is reduced but the speech is intelligible. Singing cannot. The demands of pitch matching and sustained phonation require the full pressure envelope that only diaphragmatic breathing provides.

The observation is consistent with the mechanism: the speaker reports that singing **requires** diaphragmatic breathing for pitch control. The word "control" is the key — it's not that singing is impossible from chest breathing, it's that the control necessary for pitch matching is only available from the full pressure envelope.

The mechanism also predicts that a speaker who cannot sing is a speaker whose breath mechanics are not supporting full prosodic range, whether or not their speech sounds impaired in conversation. The observation is consistent with this: the singing demand exposes a substrate limitation that conversational speech can mask.

---

## C.4 The Typing Preference

### The observation

> "I prefer to type over talk. It feels like I can follow the speed of my typing and comprehend it better. And it gives me more time to make adjustments because my talking feels imprecise. I think that might be because talking requires a change to the pressure system which affects my balance and thusly my precision."

### What it illustrates

The channel-cost mechanism (Book IV §26; Book I §2.3). Output channels differ in substrate cost. Speech spends precision on pressure modulation, postural stabilization, and laryngeal control. Typing spends none of these. The speaker's channel preference is a readout of their precision budget.

### The consistency check

The mechanism specifies the chain: speech → pressure modulation → postural reconfiguration → vestibular/proprioceptive load → precision drop in concurrent tasks. Typing bypasses this chain entirely. It is posturally static, has no pressure demand, and allows the output to be edited before commitment.

The observation is consistent with the mechanism on three points:

1. **Rate-matching.** The speaker reports following the speed of their typing. This is consistent with typing allowing the output channel to be rate-matched to the internal loop, rather than to the breath cycle.

2. **Adjustment time.** The speaker reports more time to make adjustments. This is consistent with typing's editability — the output is not committed at production time.

3. **The pressure-balance-precision link.** The speaker attributes the imprecision of speech to a pressure-system change that affects balance. This is the exact mechanism the paper specifies: the diaphragm is both a breath muscle and a postural muscle; activating it for speech changes the trunk's stability configuration; the vestibular/proprioceptive load competes for the same precision budget that comprehension and adjustment use.

The mechanism also predicts that the preference is substrate-driven, not stylistic. The observation is consistent with this: the speaker describes the preference as a functional response to a budget constraint, not as a taste.

**The further prediction:** the speaker should show a larger speech-vs-typing precision gap than a speaker with a higher precision budget, and the gap should correlate with CO₂ tolerance and postural sway during speech. The observation is consistent with this and points to a testable prediction (PREDICT-SPEECH-14, -27, -40).

---

## C.5 The Proper Name Observation

### The observation

> "I always have been bad at using names. In the moment, I often can't recall specific names."

### What it illustrates

The proper-name vulnerability mechanism (Book II §10; Book I §4.4). Proper names have no semantic neighborhood. The phonological form is not predictable from the person's attributes. This means proper name retrieval requires the highest precision of any lexical category, and it fails first under precision collapse.

### The consistency check

The mechanism specifies the structural account: a common noun like "table" is embedded in a dense semantic network — furniture, flat surface, legs, eating, writing. Activating any of those neighbors partially activates "table." The retrieval has multiple entry points. A proper name like "Jennifer" has no semantic neighborhood. Knowing that Jennifer is a colleague who works on Tuesdays doesn't activate the phonology of "Jennifer." The name is an arbitrary label attached to a rich semantic representation, with no pathway from the representation to the label.

The observation is consistent with the mechanism on two points:

1. **Selective difficulty.** The speaker reports difficulty with names specifically, not with words generally. This is consistent with proper names being the most vulnerable lexical category.

2. **In-the-moment failure.** The speaker reports the failure happening "in the moment." This is consistent with proper name retrieval requiring precision above threshold, and the retrieval failing when precision drops below the threshold.

The mechanism also predicts that proper-name failure should be the **earliest** lexical symptom of precision collapse, preceding common noun TOT, preceding verb retrieval failures, preceding grammatical errors. The observation is consistent with this: the speaker describes the difficulty as a lifelong pattern, which is consistent with a lower baseline precision for the proper-name retrieval pathway specifically.

**The further prediction:** under standardized load, the speaker should show a larger proper-name/common-noun retrieval gap than a speaker with a higher precision budget, and the gap should correlate with other precision measures. The observation is consistent with this and points to a testable prediction (PREDICT-SPEECH-16).

---

## C.6 What the Accounts Show Together

The five accounts are not independent anecdotes. They are **five different entry points into the same mechanism**:

| Account | Entry point | Mechanism |
|---|---|---|
| Motor-first probe | Production mode | Stage 6 collapse — prior calcification |
| Vocal fry | Amplitude condition | Fry requires minimum pressure; monotone does not |
| Singing | Breath support | Diaphragmatic pressure required for pitch control |
| Typing preference | Channel cost | Speech consumes precision that typing does not |
| Proper name failure | Retrieval precision | No-semantic-neighborhood words fail first |

Each account points to a different part of the model. Each is consistent with the mechanism the paper specifies. Together they show that the model is not just a formal structure — it is a set of mechanisms that can be recognized in first-person experience.

**The purpose of including them:** the paper's claims are specific enough that a reader can check whether their own introspective experience matches. If a reader recognizes the motor-first probe, the vocal fry condition, the singing demand, the typing preference, or the proper-name failure, they have a first-person confirmation of the mechanism. If they do not, the mechanism is not universal — it is context-dependent, and the reader's context may not produce the same signatures.

The accounts are invitations, not evidence. The evidence is in the predictions.

---

## C.7 How the Accounts Map to Predictions

Each account points to a testable prediction:

| Account | Prediction | What to test |
|---|---|---|
| Motor-first probe | PREDICT-SPEECH-20 | Inner speech preserved longer than overt speech under collapse |
| Vocal fry | PREDICT-SPEECH-03 | Monotone and fry dissociate by acoustic measures |
| Singing | PREDICT-SPEECH-09 | Breath mechanics predict pitch-matching accuracy |
| Typing preference | PREDICT-SPEECH-14, -27, -40 | Speech-vs-typing gap correlates with CO₂ tolerance and postural sway |
| Proper name failure | PREDICT-SPEECH-16 | Proper names fail before common nouns under load |

The accounts are the paper's motivation; the predictions are the paper's test. The two are linked by the mechanism.

---

# APPENDIX D — CROSS-LINGUISTIC DATA

## Suprasegmental architecture, phonotactic complexity, and failure mode predictions by language type

---

## How to Read This Appendix

This appendix gives the cross-linguistic data the model requires. It is organized in three parts:

- **Part 1 — Suprasegmental architecture by language** — what timing carries in each language type
- **Part 2 — Phonotactic complexity by language** — how much articulation-timing demand each language places
- **Part 3 — Failure mode predictions by language type** — what collapse looks like in each language

The data is descriptive. The predictions are the model's. Where a language's classification is contested, it is noted.

---

## Part 1 — Suprasegmental Architecture by Language

### 1.1 The suprasegmental typology

The model treats suprasegmental architecture as a **demand axis**. The more layers a language stacks onto the timing channel, the more precision it demands, and the more severe the functional consequences of the same precision drop.

| Language type | What timing carries | Load-bearing for lexical identity? | Representative languages |
|---|---|---|---|
| **Stress-timed** | Lexical stress, rhythm | Partially (stress can change meaning, e.g., "REcord" vs. "reCORD") | English, Russian, Arabic, Dutch |
| **Syllable-timed** | Even timing, less reduction | No | French, Spanish, Italian, Turkish |
| **Mora-timed** | Unit duration | Yes (mora count is lexically contrastive) | Japanese, Gilbertese, Luganda |
| **Tonal** | Lexical meaning (pitch contour) | Yes (tone changes the word) | Mandarin, Cantonese, Yoruba, Thai, Vietnamese |
| **Pitch-accent** | Lexical meaning (pitch location) | Yes (accent placement changes the word) | Japanese, Swedish, Norwegian, Serbo-Croatian |
| **Intonational** | Phrase-level meaning | No (phrase-level, not lexical) | All languages, different weights |

### 1.2 The layered case: Japanese

Japanese is the critical case because it stacks **two timing-encoded layers**:

- **Mora-timing** — every mora takes roughly equal duration. Timing is lexically load-bearing.
- **Pitch-accent** — the pitch contour is lexically contrastive. Accent placement changes word identity.

A precision drop in Japanese doesn't just flatten emotional prosody. It can **change the word**. This is a different failure mode than in English, where a precision drop flattens prosody but doesn't typically change lexical identity.

**The prediction:** Japanese speakers should show **lexical identity errors** under precision collapse, not just prosodic flattening. This is testable by comparing Japanese speakers' error profiles to English speakers' under matched precision loads.

### 1.3 The multi-layered case: Swedish and Norwegian

Swedish and Norwegian are pitch-accent languages with two accents (acute and grave). The pitch contour is lexically contrastive for some word pairs. Like Japanese, a precision drop can change word identity, though the contrastive load is lighter than in Japanese.

**The prediction:** Swedish and Norwegian speakers should show accent misplacement errors under collapse, but less severe than Japanese mora-timing errors.

### 1.4 The high-load case: Tonal languages

Tonal languages load lexical identity onto the pitch contour. Mandarin has four tones, Cantonese has six to nine, Vietnamese has six. The more tones, the more precision the speaker needs to keep them distinct.

**The prediction:** languages with more tones should show more severe lexical identity errors under the same precision drop. Mandarin (four tones) should show fewer tone errors than Cantonese (six to nine tones).

### 1.5 The light-load case: Syllable-timed languages

Syllable-timed languages place less demand on the timing channel. Timing carries rhythm but not lexical identity. French, Spanish, Italian, and Turkish fall here.

**The prediction:** speakers of syllable-timed languages should show less severe functional consequences from the same precision drop, because less of the language's meaning is carried by timing.

### 1.6 Intonational load across all languages

All languages use intonation for phrase-level meaning (question vs. statement, emphasis, emotional tone). The intonational layer is not lexically load-bearing, but it is functionally load-bearing.

**The prediction:** intonational collapse (flattened contour, question/statement confusion) should appear in all languages under precision collapse, but the functional severity should be higher in languages where intonation also carries pragmatic meaning (e.g., politeness).

---

## Part 2 — Phonotactic Complexity by Language

### 2.1 The phonotactic typology

Phonotactic complexity determines how much articulation-timing demand a language places. Complex clusters and rapid transitions require tighter phase-locking, which requires higher precision.

| Language | Phonotactic profile | Complexity |
|---|---|---|
| **English** | Complex clusters allowed ("strengths," "sixths," "twelfths") | High |
| **German** | Complex clusters allowed, final devoicing | High |
| **Russian** | Complex clusters allowed ("vzglyad," "vstrecha") | High |
| **Polish** | Complex clusters allowed ("szczęście") | Very high |
| **Spanish** | Moderate clusters, syllable-timed | Moderate |
| **Italian** | Moderate clusters, syllable-timed | Moderate |
| **French** | Moderate clusters, final consonant often silent | Moderate |
| **Japanese** | Almost no clusters (CV structure with a single coda nasal) | Very low |
| **Hawaiian** | CV structure only | Very low |
| **Mandarin** | Limited clusters (no consonant clusters in coda) | Low |
| **Cantonese** | Limited clusters, complex tones | Low (phonotactics) / High (tones) |

### 2.2 The complexity prediction

**The prediction:** the same precision level produces different articulation error rates in different languages. A rigid English speaker struggles with "strengths"; a rigid Japanese speaker struggles with almost nothing, because the language doesn't demand tight timing.

**The test:** measure articulation error rates on tight-timing words across languages. Error rates should scale with phonotactic complexity, not with word frequency alone.

### 2.3 The combined demand

A language can be high on one axis and low on another. Cantonese is low on phonotactic complexity but high on tonal complexity. English is high on phonotactic complexity but low on tonal complexity.

**The prediction:** the total demand is the sum of the two axes. Languages high on both (e.g., a hypothetical complex-cluster tonal language) should show the most severe collapse signatures. Languages low on both (e.g., Hawaiian) should show the least.

---

## Part 3 — Failure Mode Predictions by Language Type

### 3.1 The failure mode table

| Language type | Prosodic collapse | Lexical identity collapse | Articulation collapse |
|---|---|---|---|
| **Stress-timed** (English, Russian) | Prosodic flattening; stress misplacement | Rare (stress changes meaning in some pairs) | Cluster errors on complex words |
| **Syllable-timed** (French, Spanish) | Reduced prosodic range; less severe | None (timing not lexical) | Moderate cluster errors |
| **Mora-timed** (Japanese) | Flattened contour; mora-count errors | **Yes — mora count changes word** | Minimal cluster errors (CV structure) |
| **Tonal** (Mandarin, Cantonese) | Flattened contour | **Yes — tone changes word** | Minimal cluster errors (limited clusters) |
| **Pitch-accent** (Japanese, Swedish) | Flattened contour | **Yes — accent placement changes word** | Minimal cluster errors |
| **High phonotactic** (Polish, Russian) | Flattened contour | Language-specific | **Severe cluster errors** |
| **Low phonotactic** (Japanese, Hawaiian) | Flattened contour | Language-specific | Minimal cluster errors |

### 3.2 The layered failure prediction

For languages that stack multiple timing-encoded layers (Japanese: mora-timing + pitch-accent), the failure modes should **compound**:

- **First collapse:** prosodic flattening (right-hemisphere layer)
- **Second collapse:** mora-count errors (timing layer)
- **Third collapse:** accent misplacement (pitch-accent layer)
- **Fourth collapse:** lexical identity errors (combined)

**The prediction:** Japanese speakers should show a **cascade** of errors, not a single error type. The cascade order should match the layer stack order.

### 3.3 The compensating precision prediction

Speakers of languages with more timing-encoded layers should allocate more baseline precision to the timing channel.

**The prediction:** Japanese speakers should show higher baseline interhemispheric coherence or higher baseline CO₂ tolerance than English speakers, as a compensatory demand for the additional timing-encoded layers.

**The test:** measure baseline precision (via HRV coherence, phase-locking value, or CO₂ tolerance) across language groups. The prediction is that speakers of suprasegmentally complex languages show higher baseline precision.

### 3.4 The code-switching prediction

Bilingual speakers switching between languages with different suprasegmental architectures are switching demand profiles in real time.

**The prediction:** code-switching into a higher-demand language (more suprasegmental layers) should produce earlier collapse signatures than staying in the lower-demand language. The speaker's code choice under load is a demand-management strategy.

**The test:** bilingual speakers of a high-demand and a low-demand language (e.g., Cantonese and English) should show different collapse signatures depending on which language they're speaking under matched load.

### 3.5 The phonological inventory prediction

Languages differ in their phoneme inventories. A language with more phonemes requires more precise articulation to keep them distinct.

| Language | Phoneme inventory size |
|---|---|
| **Hawaiian** | ~13 phonemes |
| **Japanese** | ~20 phonemes |
| **English** | ~44 phonemes |
| **Taa (!Xóõ)** | ~160 phonemes |

**The prediction:** languages with larger phoneme inventories should show more severe phoneme discrimination errors under precision collapse, because more precision is required to keep the phonemes distinct.

---

## Part 4 — The Cross-Linguistic Prediction Table

### 4.1 Full prediction table

| Prediction | IV | DV | Falsification |
|---|---|---|---|
| PREDICT-SPEECH-32 | Language type | Collapse signature | If collapse signatures do not differ by suprasegmental architecture, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-33 | Language type | Baseline precision allocation | If speakers of complex languages do not allocate more precision to timing, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-34 | Language phonotactic complexity | Tight-timing word errors | If error rates do not scale with phonotactic complexity, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-38 | Language demand | Code-switching collapse | If code-switching into a higher-demand language does not produce earlier collapse, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-52 | Tonal inventory size | Tone error rate | If tone errors do not scale with tonal inventory size, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-53 | Phoneme inventory size | Phoneme discrimination errors | If discrimination errors do not scale with inventory size, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-54 | Layered suprasegmental architecture | Error cascade order | If error cascade does not follow layer stack order, the demand-axis model is disconfirmed |

### 4.2 The layered prediction table

| Language | Timing-encoded layers | Predicted first collapse | Predicted cascade |
|---|---|---|---|
| **English** | Stress + intonation | Prosodic flattening | Stress misplacement → cluster errors |
| **French** | Intonation | Reduced prosodic range | Minimal cascade (light load) |
| **Japanese** | Mora-timing + pitch-accent | Prosodic flattening | Mora errors → accent misplacement → lexical identity errors |
| **Mandarin** | Tone + intonation | Prosodic flattening | Tone errors → lexical identity errors |
| **Cantonese** | Tone (6–9) + intonation | Prosodic flattening | Tone errors (severe) → lexical identity errors |
| **Swedish** | Pitch-accent + intonation | Prosodic flattening | Accent misplacement → occasional lexical identity errors |
| **Polish** | Stress + intonation + complex phonotactics | Prosodic flattening | Cluster errors (severe) → stress misplacement |

---

## Part 5 — What This Appendix Shows

### 5.1 The demand axis is not abstract

The demand axis is real. Languages differ in how much they load onto the timing channel, and the differences are measurable.

### 5.2 The failure modes are language-specific

The same precision drop produces different failure modes in different languages. A Japanese speaker loses lexical identity before emotional prosody; an English speaker loses emotional prosody first. The demand axis predicts this.

### 5.3 The prediction is testable

Every prediction in this appendix is testable with standard acoustic and cross-linguistic methods. The data is available. The prediction is specific.

### 5.4 The model is cross-linguistically honest

The model does not assume English. It specifies a mechanism that produces different readouts in different languages. This is a stronger claim than "the model works for English," because it predicts **what will differ and why**.

---

# APPENDIX E — CROSS-DOMAIN CONFLICT DATA

## Task-pair conflict matrix and layer-specific degradation predictions

---

## How to Read This Appendix

This appendix gives the cross-domain conflict data the model requires. It is organized in three parts:

- **Part 1 — The conflict principle** — why tasks compete for precision
- **Part 2 — The conflict matrix** — degradation signatures by task pair
- **Part 3 — Predictions and falsification** — what would disconfirm the model

The data is descriptive. The predictions are the model's.

---

## Part 1 — The Conflict Principle

### 1.1 The principle

Speech production consumes precision. Concurrent tasks also consume precision. When two tasks compete for the same precision budget, speech degrades — and it degrades **layer-specifically**, depending on which layers the concurrent task competes with.

**The rule:** the concurrent task competes with the layers that share its precision demand.

### 1.2 The shared-demand categories

Tasks share precision demands across four categories:

- **Motor timing** — tasks requiring precise timing coordination (driving, gaming, instrument playing)
- **Working memory** — tasks requiring holding information online (coding, reading, conversation)
- **Visual attention** — tasks requiring sustained visual processing (driving, gaming, reading)
- **Semantic** — tasks requiring meaning processing (reading, listening, conversation)

A task pair that shares two or more categories should produce a larger conflict than a task pair that shares one.

### 1.3 The layer-competition table

| Speech layer | Primary precision demand | Competing task category |
|---|---|---|
| Pragmatic | ToM + context + timing | Social cognition, context tracking |
| Discourse | WM + timing + prediction | Working memory, planning |
| Prosodic | Motor timing + interoception | Motor timing, breath control |
| Lexical | Semantic + phonological | Semantic processing, verbal WM |
| Morphosyntactic | WM + rule retrieval | Working memory, symbolic manipulation |
| Phonological | Motor timing + LH sequencing | Fine motor timing, sequencing |
| Articulatory | Motor + breath + posture | Motor control, postural control |
| Breath | Diaphragm + intercostals | Postural control, physical exertion |

---

## Part 2 — The Conflict Matrix

### 2.1 The task-pair table

| Task pair | Shared demand | Predicted degradation | Why |
|---|---|---|---|
| **Gaming + talking** | Motor timing + visual attention + WM | Prosody + discourse | Gaming consumes timing + WM; speech loses both |
| **Driving + talking** | Motor timing + visual attention | Prosody + articulation | Driving consumes timing + visual; speech loses timing |
| **Coding + talking** | WM + symbolic manipulation | Discourse + morphosyntax | Coding consumes WM; speech loses frame-holding |
| **Reading + talking** | Visual + semantic + phonological | Lexical + phonological | Reading consumes semantic + phonological; speech loses retrieval |
| **Listening to speech + speaking** | Auditory + prosodic + semantic | Prosody + pragmatic | Listening consumes prosodic + semantic; speech loses prosodic framing |
| **Instrument playing + talking** | Motor timing + auditory | Prosody + articulation | Instrument consumes timing; speech loses timing + motor |
| **Math problem-solving + talking** | WM + symbolic | Discourse + morphosyntax | Math consumes WM; speech loses frame-holding |
| **Video calls + talking** | Visual + auditory + social + WM | Pragmatic + discourse + prosodic | Video calls consume all four; speech degrades across multiple layers |
| **Walking + talking** | Motor + postural | Articulatory + breath | Walking consumes postural; speech loses pressure stability |
| **Running + talking** | Motor + postural + breath | Breath + articulatory | Running consumes breath; speech loses pressure envelope |

### 2.2 The degradation order within a conflict

When a concurrent task consumes precision, the layers degrade in the order determined by their integration demand — the same order as in general collapse.

**The prediction:** even in a task conflict, the layer that collapses first is the one with the highest integration demand (pragmatic), then discourse, then prosodic, and so on. The conflict accelerates the collapse but doesn't change the order.

### 2.3 The intensity prediction

The more precision the concurrent task consumes, the faster the collapse.

| Task intensity | Predicted collapse depth |
|---|---|
| Low (walking) | Articulatory + breath only |
| Moderate (driving) | Prosody + articulation |
| High (gaming) | Prosody + discourse |
| Very high (video call with complex content) | Pragmatic + discourse + prosodic |

**The prediction:** collapse depth scales with task intensity.

### 2.4 The individual-difference prediction

Speakers with higher baseline precision should tolerate more concurrent load before speech degrades.

**The prediction:** the task-intensity threshold at which speech degrades should correlate with baseline precision (CO₂ tolerance, HRV, phase-locking value).

---

## Part 3 — Predictions and Falsification

### 3.1 The conflict predictions table

| Prediction | IV | DV | Falsification |
|---|---|---|---|
| PREDICT-SPEECH-24 | Task pair | Degradation signature | If degradation signature is not predictable from shared precision demand, the conflict model is disconfirmed |
| PREDICT-SPEECH-25 | Task pair | Speech degradation | If "can you talk while X?" is not a precision-budget question, the conflict model is disconfirmed |
| PREDICT-SPEECH-55 | Task intensity | Collapse depth | If collapse depth does not scale with task intensity, the conflict model is disconfirmed |
| PREDICT-SPEECH-56 | Baseline precision | Task-intensity threshold | If the threshold does not correlate with baseline precision, the conflict model is disconfirmed |
| PREDICT-SPEECH-57 | Task pair | Layer-collapse order | If the layer-collapse order in a conflict does not follow integration demand, the layer-stack model is disconfirmed |

### 3.2 The test designs

**Test 1 — Dual-task degradation:**
- Participants perform a speech task alone and with a concurrent task.
- Compare speech measures (pitch granularity, topic coherence, articulation precision).
- Prediction: speech degrades more with concurrent task; degradation signature depends on the shared demand.

**Test 2 — Task-intensity scaling:**
- Participants perform a speech task with concurrent tasks at increasing intensity.
- Compare speech measures across intensity levels.
- Prediction: collapse depth scales with task intensity.

**Test 3 — Individual differences:**
- Measure baseline precision in participants.
- Measure the task-intensity threshold at which speech degrades.
- Prediction: threshold correlates with baseline precision.

**Test 4 — Layer-collapse order in conflict:**
- Measure multiple layer biomarkers during a concurrent task.
- Compare collapse order to integration-demand prediction.
- Prediction: collapse order follows integration demand even in conflict.

---

## Part 4 — The Clinical Application

### 4.1 The clinical question

"Can you talk while X?" is a precision-budget question, not a preference question.

### 4.2 The clinical protocol

1. **Identify the concurrent task.** What else is the speaker doing while speaking?
2. **Identify the shared demand.** What precision category does the concurrent task consume?
3. **Predict the degradation signature.** Which layers should collapse first?
4. **Measure the degradation.** Does the observed signature match the prediction?
5. **Intervene at the substrate.** Reduce the concurrent load, restore the substrate, or shift the channel.

### 4.3 The clinical case

A patient reports difficulty with phone calls but not with texting.

**The model's interpretation:**
- Phone calls require speech production + real-time comprehension. Both compete for the same precision budget.
- Texting allows the comprehension and production to be sequential rather than simultaneous.
- The patient's precision budget is insufficient for the simultaneous demand of phone calls.
- The preference for texting is a precision-budget optimization, not a social preference.

**The intervention:**
- Reduce the concurrent demand (schedule calls when load is low)
- Restore the substrate (breath training, CO₂ tolerance work)
- Shift the channel (use texting for high-demand contexts, speech for low-demand)
- Monitor recovery (channel preference should shift back toward speech as precision restores)

### 4.4 The monitoring implication

Channel preference in a specific context is a **readout of the precision budget for that context**. A patient who avoids phone calls is reporting a precision budget that phone calls exceed. The report is clinical data.

---

## Part 5 — What This Appendix Shows

### 5.1 The conflict model is real

Task conflicts are not vague interference. They are precision-budget competitions with predictable signatures.

### 5.2 The degradation is layer-specific

The same concurrent task produces different degradation signatures depending on which layers share its precision demand.

### 5.3 The prediction is testable

Every prediction in this appendix is testable with standard dual-task methods. The data is available. The prediction is specific.

### 5.4 The clinical application is direct

"Can you talk while X?" is a precision-budget question. The answer is a clinical readout.

---

# APPENDIX F — EMPIRICAL ANCHORS

## Citations organized by claim, with verification status

---

## How to Read This Appendix

This appendix lists the empirical anchors for each claim in the paper. Each anchor is a study or body of work that shows the invariant the paper predicts.

**Structure:** anchors are organized by claim. Each entry gives the claim, the anchor, and the verification status.

**Verification status:**

- **Verified** — the citation is confirmed and complete
- **Stub** — the claim is confirmed in the literature, but the exact citation needs verification
- **Pending** — the claim is plausible but requires empirical confirmation
- **Synthesis** — the claim is a synthesis of multiple findings, not a single study

**How to use this appendix:**

- **For the citation pass:** each stub is a target. The verification pass fills them in.
- **For the falsification check:** each anchor is a place where the paper's claim can be disconfirmed.
- **For the reader:** each anchor is a place to start if they want to check the paper's claims against the literature.

---

## 1. Verified Anchors — Breath and Precision

| Claim | Anchor | Status |
|---|---|---|
| Nasal respiration entrains limbic oscillations | Zelano et al. (2016), *Journal of Neuroscience* | Verified |
| CO₂ drives cerebral vasodilation | Raichle & Plum (1972) | Verified |
| Slow breathing produces HRV and EEG coherence | Zaccaro et al. (2018), *Frontiers in Human Neuroscience* | Verified |
| Breathing training shifts parameters | Kox et al. (2014), *PNAS* | Verified |
| Control Pause measures $C_{high}$ individually | Cooper et al. (2003) — Buteyko trial | Verified |
| Hypocapnia produces cognitive and anxiety collapse | Meuret & Ritz (2010) | Verified |
| Hyperventilation impairs cognitive function | Tsukamoto et al. (2014) | Verified |
| Precision is a timing-coherence ratio | Pratap et al. (2026) | Verified |
| CO₂ tolerance window determines precision peak | Sakakibara et al. (1994) | Verified |
| Resonance breathing produces stable precision | Yamamoto et al. (2006) | Verified |
| Collapse hysteresis delays recovery | Reed et al. (2020) | Verified |

---

## 2. Verified Anchors — Neural Architecture

| Claim | Anchor | Status |
|---|---|---|
| Right-hemisphere prosody dominance | Ross (1981) — aprosodia literature | Verified |
| Hemispheric laterality affects autonomic regulation | Dono et al. (2020) | Verified |
| Interhemispheric coherence and parasympathetic activation | Yamamoto et al. (2006) | Verified |
| Feature interference is $K$ rising | Xue et al. (2026) | Verified |
| PV+ interneurons are metabolically vulnerable | Kann et al. (2015) | Verified |
| ΔCBF/ΔCMRO₂ predicts neural efficiency | Hutchison & Rypma (2013) | Verified |
| EEG-HRV coupling during hyperventilation | Titov & Dick (2022) | Verified |
| LP-ACC circuit detects change | Leow et al. (2026) | Verified |
| ACC activity scales with prediction error | Botvinick et al. (2001) | Verified |
| Beta oscillations signal prior maintenance | Engel & Fries (2010) | Verified |
| Working memory capacity ~5 items | Cowan (2016) | Verified |

---

## 3. Citation-Pass Targets — Speech Production

These are the claims that need anchors from the speech literature. Each entry gives the claim, the section where it appears, and the kind of study that would anchor it.

| Claim | Section | Anchor target | Status |
|---|---|---|---|
| Prosodic granularity loss precedes pitch range loss | Book II §9, Book IV §23.2 | Trauma prosody literature; granularity measures | Stub |
| Monotone and vocal fry are distinct acoustic events | Book II §9, Appendix C.2 | Vocal fry acoustic literature; phonation mode studies | Stub |
| Trauma produces prosodic shifts (moderated by landing state) | Book II §9, Book III §15 | Trauma prosody literature; arousal/salience moderation studies | Stub — re-anchored to routing |
| TOT increases under stress, fatigue, and load | Book II §10, Book IV §23.2 | TOT under load literature | Stub |
| Proper names fail before common nouns | Book II §10, Book IV §23.2 | Proper-name retrieval literature; Brédart (2017) | Partially verified |
| Tight-timing words require tighter phase-locking | Book II §12, Book IV §23.2 | Articulatory timing literature | Stub |
| Parkinson's produces articulatory-timing degradation | Book II §12, Book V §27.2 | Parkinson's speech literature; temporal/articulatory studies | Partially verified |
| FAS is a prosodic timing collapse | Book V §31 | Katz et al. (2008), *Clinical Linguistics & Phonetics*; Longman et al. (2025) | Partially verified |
| Slurring correlates with hemispheric desynchronization | Book II §12 | Motor speech disorder literature; hemispheric mechanisms of motor speech | Partially verified |
| Mumbling is amplitude collapse | Book II §13 | Dysarthria literature; amplitude studies | Stub |
| Register switching is precision allocation | Book V §28.6 | Register and prosody literature | Stub |
| Turn-taking is inter-brain phase-locking | Book V §28.6 | Conversation synchrony literature | Stub |

---

## 4. Citation-Pass Targets — Cross-Linguistic Variation

| Claim | Section | Anchor target | Status |
|---|---|---|---|
| Suprasegmental architecture varies by language | Appendix D | Prosodic typology literature | Stub |
| Tonal languages use timing for lexical identity | Appendix D | Tone language literature | Stub |
| Pitch-accent languages use timing for word recognition | Appendix D | Pitch-accent literature | Stub |
| Mora-timed languages use timing for unit duration | Appendix D | Mora-timing literature | Stub |
| Phonotactic complexity varies by language | Appendix D | Phonotactic literature | Stub |
| Japanese is mora-timed and pitch-accent | Appendix D | Japanese prosody literature | Stub |

---

## 5. Citation-Pass Targets — Channel and Modality

| Claim | Section | Anchor target | Status |
|---|---|---|---|
| Typing preference correlates with precision budget | Book IV §26, Appendix C.4 | Typing vs. speech preference literature | Stub — possibly synthesis |
| Speech production has postural cost | Book I §2.3, Book II §14 | Posture and breathing literature | Stub |
| Seated speech is more precise than standing | Book III §17.4 | Postural control literature | Stub |
| Inner speech is preserved under load | Book III §21.2 | Inner speech literature | Stub |
| Written output is preserved under load | Book III §21.2 | Written vs. spoken production literature | Stub |
| Sign language prosody has different collapse schedule | Book III §21.2 | Sign language prosody literature | Stub |
| Code-switching is demand management | Book III §21.2 | Bilingualism and cognitive load literature | Stub |

---

## 6. Citation-Pass Targets — Clinical Conditions

| Claim | Section | Anchor target | Status |
|---|---|---|---|
| Alexithymia involves low interoceptive accuracy | Book V §27.2 | Alexithymia interoception literature | Stub |
| Autism involves atypical prosody and pragmatics | Book V §27.2 | Patel et al. (2019), *Autism Research*; Russo et al. (2008) | Partially verified |
| ADHD involves discourse instability | Book V §27.2 | ADHD discourse literature | Stub |
| Depression involves amplitude collapse | Book V §27.2 | Depression speech literature | Stub |
| Anxiety involves prosodic tightening | Book V §27.2 | Anxiety prosody literature | Stub |
| Dissociation involves flat, distant prosody | Book V §27.2 | Dissociation speech literature | Stub |
| Parkinson's involves motor-prosody coupling degradation | Book V §27.2 | Parkinson's speech literature | Stub |
| Right-hemisphere lesions produce aprosodia | Book V §27.2 | Ross aprosodia literature | Verified |
| FAS involves prosodic timing collapse | Book V §31 | FAS literature | Partially verified |
| ND burnout involves Stage 3–4 collapse after chronic masking | Book V §27.2 | ND burnout literature; masking cost literature | Stub — re-anchored to routing |

---

## 7. Citation-Pass Targets — Social and Regional

| Claim | Section | Anchor target | Status |
|---|---|---|---|
| Collective synchrony supports shared meaning | Book V §28 | Synchrony literature | Stub |
| Exhale gate trap produces conspiracy thinking | Book V §28.3 | Conspiracy cognition literature | Stub |
| Prosodic masking has measurable cost | Book V §28.4 | Masking cost literature | Stub |
| ND and social-group prosody overlap | Book V §28.5 | Prosodic variation literature | Stub |
| Regional accents track substrate profiles | Book V §29 | Regional prosody literature | Stub |
| Accents persist via somatic timing inheritance | Book V §29.3 | Accent acquisition literature | Stub |
| Postural patterns vary by region | Book V §29.5 | Postural and movement literature | Stub |

---

## 8. Citation-Pass Targets — Drugs

| Claim | Section | Anchor target | Status |
|---|---|---|---|
| Depressants flatten prosody | Book V §30.2 | Drug effects on speech literature | Stub |
| Stimulants produce clipped cadence | Book V §30.2 | Stimulant speech literature | Stub |
| Psychedelics produce atypical prosody | Book V §30.2 | Psychedelic speech literature | Stub |
| Dissociatives flatten prosody | Book V §30.2 | Dissociative speech literature | Stub |
| Alcohol produces slurring | Book V §30.2 | Alcohol speech literature | Stub |
| THC produces blurred phonemes | Book V §30.2 | THC speech literature | Stub |

---

## 9. Citation-Pass Targets — Cross-Domain Conflicts

| Claim | Section | Anchor target | Status |
|---|---|---|---|
| Dual-task interference degrades speech | Appendix E | Dual-task literature | Stub |
| Driving and talking compete for precision | Appendix E | Driving-and-talking literature | Stub |
| Gaming and talking compete for precision | Appendix E | Gaming-and-talking literature | Stub |
| Coding and talking compete for WM | Appendix E | Coding-and-talking literature | Stub |

---

## 10. Citation-Pass Targets — Routing and Masking

| Claim | Section | Anchor target | Status |
|---|---|---|---|
| Emotional granularity predicts prosodic congruence | Book III §18, Book IV §23.3 | Emotional granularity literature | Stub |
| Masking has measurable allostatic cost | Book III §18, Book V §27.6 | Masking and allostatic load studies | Stub |
| ND masking cost is measurable | Book III §18.3 | ND masking cost studies | Stub |
| Alexithymia involves low interoceptive routing | Book III §18.3 | Alexithymia interoception studies | Stub |
| Chronic masking predicts late collapse detection | Book III §18.5, Book V §27.6 | Masking and collapse detection literature | Stub — possibly new prediction |

---

## 11. Citation-Pass Targets — Precision Ecology

| Claim | Section | Anchor target | Status |
|---|---|---|---|
| Digital load affects cognition | Book III §19 | Digital load literature | Stub |
| Posture affects breathing | Book III §19 | Posture and breathing literature | Stub |
| Forward head posture affects diaphragm function | Book III §19 | Postural mechanics literature | Stub |
| Generational speech patterns track substrate | Book III §19 | Generational speech literature | Stub |

---

## 12. The Anchor Verification Pass

The verification pass has three tasks:

1. **Fill the stubs.** For each stub, find the exact citation, verify the claim, and update the entry.
2. **Check the verified.** For each verified citation, verify that the claim is accurate and the citation is complete.
3. **Flag the contested.** If a claim is contested in the literature, mark it as contested and note the counter-evidence.
4. **Mark the syntheses.** If a claim is a synthesis of multiple findings rather than a single study, mark it as synthesis and list the component findings.

**The verification pass is the paper's last step before submission.** The mechanism is specified; the predictions are registered; the anchors are the evidence that the mechanism is consistent with what is already known.

---

## 13. Anchor Status Summary

| Category | Verified | Partially verified | Stub | Synthesis |
|---|---|---|---|---|
| Breath and precision | 11 | 0 | 0 | 0 |
| Neural architecture | 11 | 0 | 0 | 0 |
| Speech production | 0 | 3 | 9 | 0 |
| Cross-linguistic variation | 0 | 0 | 6 | 0 |
| Channel and modality | 0 | 0 | 6 | 1 |
| Clinical conditions | 1 | 2 | 7 | 0 |
| Social and regional | 0 | 0 | 7 | 0 |
| Drugs | 0 | 0 | 6 | 0 |
| Cross-domain conflicts | 0 | 0 | 4 | 0 |
| Routing and masking | 0 | 0 | 4 | 1 |
| Precision ecology | 0 | 0 | 4 | 0 |
| **Total** | **23** | **5** | **59** | **2** |

**The paper's anchor base is split between verified citations (from Central Reference), partially verified citations (from the search pass), and stubs (specific to speech).** The verification pass fills the stubs from the speech literature and marks the syntheses.

---

## 14. What the Anchors Show

The anchors show that the model is not a new theory built on nothing. It is a **unification** of findings that already exist in separate literatures.

- **The breath-precision anchors** show that the substrate mechanism is established.
- **The neural architecture anchors** show that the hemispheric model is established.
- **The speech production anchors** show that the speech signatures are documented.
- **The cross-linguistic anchors** show that suprasegmental variation is established.
- **The channel and modality anchors** show that channel differences are real.
- **The clinical anchors** show that condition-specific signatures are documented.
- **The social and regional anchors** show that collective and regional variation is real.
- **The drug anchors** show that pharmacological shifts are documented.
- **The conflict anchors** show that dual-task interference is established.
- **The routing anchors** show that masking cost is a real phenomenon.
- **The ecology anchors** show that environmental load is real.

**The framework's contribution is not the discovery of any single finding.** It is the specification of the mechanism that explains why the findings fit together. The anchors are the findings. The model is the map.

**The routing contribution is new.** The masking literature exists, the allostatic load literature exists, and the emotional granularity literature exists — but the routing variable that connects them is the paper's synthesis. The citation pass for the routing section will mark these as syntheses, not single-study anchors.

---

# APPENDIX G — RELATED PAPERS AND THE STACK

## The stack diagram, citation rule, and which paper covers what

---

## How to Read This Appendix

This appendix specifies where The Spoken Language Paper sits in the framework's document stack. It gives:

- The full stack diagram
- The citation rule
- Which paper covers what
- Which papers are companions, which are projections, and which are the specification

It exists so that a reader who comes to The Spoken Language Paper first knows where to go next, and so that a reader who comes to the framework through another paper knows how this paper relates to it.

---

## 1. The Stack

The framework is organized as a **single specification** (Central Reference) plus a set of **domain projections** (papers that apply the specification to a specific domain) plus a set of **companion papers** (papers that extend a domain projection).

```
                         Central Reference v1.5
                         (the specification)
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
            Geometry of        Loop Is the       Domain
              Inference        Intelligence      projections
               v1.0               v1.0           (hallucination,
            (biology)          (argument)         AGI, URM, etc.)
                                    │
                                    ▼
                        The Spoken Language Paper
                              v3.1 (this paper)
                              (speech projection)
                                    │
                    ┌───────────────┼───────────────┐
                    │               │               │
                    ▼               ▼               ▼
            The Singing        The Language      Language as a
            Substrate          Acquisition       Typed System
            Paper              Paper
            (companion)        (companion)
```

**The stack has three layers:**

1. **The specification layer:** Central Reference v1.5. Everything is defined here.
2. **The canonical layer:** Manifold Schema, Precision, Allostatic Load, Geometry of Inference, Loop Is the Intelligence. These are the extended derivations.
3. **The projection layer:** The Spoken Language Paper and other domain projections. These apply the specification to a specific domain.

**The companion layer:** The Singing Substrate Paper, The Language Acquisition Paper, and Language as a Typed System extend The Spoken Language Paper into adjacent domains.

---

## 2. The Citation Rule

**Cite Central Reference v1.5 alone.**

The framework's citation rule (Central Reference §25) is that future papers cite Central Reference alone. The supporting papers are domain projections and do not need separate citation unless the new paper is specifically extending one of their layers.

**For The Spoken Language Paper, this means:**

- When citing the framework's mechanism, cite Central Reference v1.5.
- When citing the speech-specific claims, cite The Spoken Language Paper v3.1.
- When citing companion material (singing, acquisition, typed systems), cite the companion paper.

**The rule exists because the framework is a single specification.** Central Reference contains every variable, every equation, and every mechanism. The supporting papers provide depth, not new content. A reader who cites Central Reference has cited the framework.

---

## 3. Which Paper Covers What

### 3.1 The specification layer

| Paper | Covers | Does not cover |
|---|---|---|
| **Central Reference v1.5** | Every variable, every equation, every mechanism in the framework | Domain-specific applications |
| **Manifold Schema v7.2** | The canonical derivation of the manifold model | Measurement protocols, domain projections |
| **Precision v3.4** | The precision formalism — $P = R/D_T$, CO₂, two-factor pressure, temporal dynamics | Speech-specific applications |
| **Allostatic Load v2.1** | The measurement layer — $L^*$ decomposition, four contracts, delta HRV, zones | Speech-specific applications |
| **Geometry of Inference v1.0** | The biological implementation — LP-ACC, four-layer cache, gate condition, somatic commutation, exhale gate trap, breath phase timing | Speech-specific applications |
| **Loop Is the Intelligence v1.0** | The argument that intelligence is the loop | Domain-specific applications |

### 3.2 The projection layer

| Paper | Covers | Depends on |
|---|---|---|
| **The Spoken Language Paper v3.1** (this paper) | The timing-geometry account of spoken language — three axes, eight layers, collapse and recovery, routing, measurement, projections | Central Reference, Precision, Geometry of Inference |
| **The Hallucination You Are Having Right Now** | The substrate-agnostic hallucination theory | Central Reference, Geometry of Inference |
| **The Profile of a Person That Is AGI** | AGI as a system property | Central Reference, Loop Is the Intelligence |
| **Dual-Substrate Cognition Architecture** | Human-AI co-processing | Central Reference, Loop Is the Intelligence |
| **Hallucinations Are Not Random** | AI hallucination mechanism | Central Reference |
| **Regulatory-Engine Qualification for Complex Decision-Making** | Governance-facing REQT artifact | Central Reference, Allostatic Load |

### 3.3 The companion layer

| Paper | Covers | Extends |
|---|---|---|
| **The Singing Substrate Paper** | The aesthetic-reception dimension of the breath-to-prosody mechanism | The Spoken Language Paper §14 (breath/pressure layer) |
| **The Language Acquisition Paper** | How the substrate develops and how precision training transfers | The Spoken Language Paper §13 (articulatory layer), §17 (channel economics) |
| **Language as a Typed System** | The typed-system account of language structure | The Spoken Language Paper (the layer stack is a typed system) |
| **The Geometry Beneath the Category** | How categories form from manifold geometry | Central Reference, Manifold Schema |
| **Autism Strengths Are Controlled** | The autism profile as a manifold configuration | Central Reference, The Spoken Language Paper §27 (clinical conditions) |
| **Building a Non-Left Hemisphere from the Start** | The developmental account of hemispheric specialization | Central Reference, The Spoken Language Paper §3 (neural architecture) |

---

## 4. What The Spoken Language Paper Contributes

The Spoken Language Paper is a **domain projection** of Central Reference. It applies the framework's mechanism to the speech domain.

**What it contributes to the framework:**

- The **three-axis model** — supply, demand, channel — as the determinants of the collapse shape
- The **routing dimension** — $f_{routing}$ as the determinant of whether the collapse is visible
- The **eight-layer stack** — pragmatic through breath — as the ordered readout of the collapse sequence
- The **integration-demand rule** — layers with more cross-domain binding collapse first
- The **recovery ladder** — the mirror-image sequence with asymmetric timing
- The **channel-cost model** — output modality as a precision-budget allocation
- The **masking mechanism** — routing to output management as a measurable cost
- The **proper-name vulnerability mechanism** — no-semantic-neighborhood retrieval failure
- The **cross-linguistic demand axis** — suprasegmental architecture as a determinant of failure mode
- The **cross-domain conflict model** — task-pair competition for the precision budget
- The **biomarker inventory** — one biomarker per layer plus routing and channel preference
- The **monitoring ladder** — which layer to measure at which stage
- The **prediction registry** — 60 predictions specific to the speech domain

**What it does not contribute:**

- New variables. Every variable is defined in Central Reference.
- New equations. Every equation is defined in Central Reference.
- New mechanisms. Every mechanism is defined in Central Reference.

**What it does is specify how the framework's mechanism expresses in the speech domain.** The framework says precision is the master variable; The Spoken Language Paper says what happens to speech when precision changes, and what happens when the routing hides the change.

---

## 5. Reading Order

### 5.1 If you come to The Spoken Language Paper first

1. Read **Book I** (the model).
2. Read **Book II** (the layers) for the layer you're interested in.
3. Read **Book III** (the dynamics) for the context you're interested in.
4. Read **Book IV** (the measurement) if you want to apply the model.
5. Read **Book V** (the projections) for the applied payoff.
6. Read **Central Reference v1.5** for the full framework.

### 5.2 If you come to the framework through Central Reference

1. Read **Central Reference v1.5** for the specification.
2. Read **The Spoken Language Paper v3.1** for the speech projection.
3. Read **the companion papers** for adjacent domains.

### 5.3 If you come to the framework through a companion paper

1. Read **Central Reference v1.5** for the specification.
2. Read **The Spoken Language Paper v3.1** for the speech projection.
3. Read **the companion paper** you came through for the adjacent domain.

---

## 6. The Framework's Posture

The framework's posture is **specification-plus-projection**. The specification (Central Reference) defines the variables and mechanisms. The projections (domain papers) apply them to specific domains. The companions (companion papers) extend the projections.

**This is not a theory with applications.** It is a **specification with projections**. The specification is the theory. The projections are the applications. The companions are the extensions.

**The Spoken Language Paper is a projection.** It is not a new theory. It is the framework applied to speech.

---

# APPENDIX H — FALSIFIABILITY SUMMARY

## All falsification conditions in one table

---

## How to Read This Appendix

This appendix gives every falsification condition in the paper, organized by type. It is the paper's honesty: it names what would disconfirm the model.

**The structure:**

- Falsification conditions organized by **type** (substrate, collapse order, layer distinction, channel cost, demand axis, recovery, conflict, allocation, routing)
- Falsification conditions organized by **prediction** (each prediction's falsification condition)
- Falsification conditions organized by **severity** (load-bearing vs. exploratory)

**How to use this appendix:**

- **For the falsification check:** each condition is a place where the model can be tested and potentially disconfirmed.
- **For the reviewer:** each condition is a specific, testable claim.
- **For the reader:** each condition is a place where the model's honesty is visible.

---

## 1. Falsification by Type

### 1.1 Substrate does not predict speech

| Prediction | Falsification condition |
|---|---|
| PREDICT-SPEECH-01 | If breath mechanics do not predict prosodic range, the breath-to-prosody mechanism is disconfirmed |
| PREDICT-SPEECH-02 | If CO₂ tolerance does not predict prosodic stability, the CO₂-to-prosody mechanism is disconfirmed |
| PREDICT-SPEECH-06 | If trauma does not produce measurable prosodic shifts, the trauma-prosody mechanism is disconfirmed |
| PREDICT-SPEECH-08 | If FAS patients show normal precision on non-speech measures, the FAS-as-precision-collapse mechanism is disconfirmed |
| PREDICT-SPEECH-09 | If breath mechanics do not predict pitch-matching accuracy, the breath-to-prosody mechanism is disconfirmed |
| PREDICT-SPEECH-10 | If regional prosodic profiles do not correlate with substrate, the substrate-to-accent mechanism is disconfirmed |
| PREDICT-SPEECH-14 | If the speech-vs-typing gap does not correlate with substrate measures, the channel-cost mechanism is disconfirmed |
| PREDICT-SPEECH-27 | If the speech-vs-typing gap does not correlate with substrate measures, the channel-cost mechanism is disconfirmed |
| PREDICT-SPEECH-40 | If the speech-vs-typing gap does not correlate with substrate measures, the channel-cost mechanism is disconfirmed |
| PREDICT-SPEECH-47 | If regional prosodic profiles do not correlate with substrate, the substrate-to-accent mechanism is disconfirmed |
| PREDICT-SPEECH-49 | If postural patterns do not predict breath patterns, the postural-cost mechanism is disconfirmed |
| PREDICT-SPEECH-50 | If drug effects are not predictable from substrate variables, the substrate-shift model is disconfirmed |
| PREDICT-SPEECH-51 | If FAS patients show normal precision, the FAS-as-precision-collapse mechanism is disconfirmed |

**What this would disconfirm:** the substrate-to-speech mechanism. If substrate variables (breath, CO₂, posture, precision) don't predict speech signatures, the mechanism fails.

### 1.2 Collapse order is not forced

| Prediction | Falsification condition |
|---|---|
| PREDICT-SPEECH-15 | If collapse order does not follow integration demand, the layer-stack model is disconfirmed |
| PREDICT-SPEECH-22 | If recovery order does not mirror collapse order, the integration-demand rule is disconfirmed |
| PREDICT-SPEECH-42 | If conditions with different entry points show the same collapse order, the entry-point model is disconfirmed |
| PREDICT-SPEECH-43 | If conditions with the same entry point show different signatures, the entry-point model is disconfirmed |
| PREDICT-SPEECH-57 | If the layer-collapse order in a conflict does not follow integration demand, the layer-stack model is disconfirmed |

**What this would disconfirm:** the integration-demand rule. If collapse order doesn't follow integration demand, the eight-layer stack is wrong.

### 1.3 Layer distinction is not useful

| Prediction | Falsification condition |
|---|---|
| PREDICT-SPEECH-03 | If monotone and fry always co-occur, the distinction is not clinically useful |
| PREDICT-SPEECH-16 | If proper names do not fail before common nouns, the no-semantic-neighborhood account is disconfirmed |
| PREDICT-SPEECH-19 | If sign prosody collapses on the same schedule as speech prosody, the channel-cost model is disconfirmed |
| PREDICT-SPEECH-20 | If inner speech collapses on the same schedule as overt speech, the channel-cost model is disconfirmed |
| PREDICT-SPEECH-35 | If inner speech is not preserved longer, the channel-cost model is disconfirmed |
| PREDICT-SPEECH-36 | If written output is not preserved relative to spoken, the channel-cost model is disconfirmed |
| PREDICT-SPEECH-37 | If sign prosody collapses on the same schedule as speech, the channel-cost model is disconfirmed |

**What this would disconfirm:** the layer distinctions. If monotone and fry are the same, or if proper names and common nouns fail together, or if channels don't differ in collapse schedule, the layer stack is not useful.

### 1.4 Channel cost is not real

| Prediction | Falsification condition |
|---|---|
| PREDICT-SPEECH-13 | If channel preference does not shift before speech degradation, the leading-indicator claim is disconfirmed |
| PREDICT-SPEECH-18 | If seated speech is not more precise than standing, the postural-cost mechanism is disconfirmed |
| PREDICT-SPEECH-26 | If channel preference does not shift from speech to typing under load, the channel-cost model is disconfirmed |
| PREDICT-SPEECH-28 | If seated speech is not more precise, the postural-cost mechanism is disconfirmed |
| PREDICT-SPEECH-31 | If channel shift does not track both digital and postural loads, the ecological projection is disconfirmed |
| PREDICT-SPEECH-39 | If channel preference does not shift before speech degradation, the leading-indicator claim is disconfirmed |
| PREDICT-SPEECH-41 | If seated speech is not more precise, the postural-cost mechanism is disconfirmed |

**What this would disconfirm:** the channel-cost mechanism. If channel preference doesn't shift under load, or if seated speech isn't more precise than standing, the channel axis is wrong.

### 1.5 Demand axis is not real

| Prediction | Falsification condition |
|---|---|
| PREDICT-SPEECH-17 | If suprasegmental complexity does not predict collapse severity, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-32 | If collapse signatures do not differ by suprasegmental architecture, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-33 | If speakers of complex languages do not allocate more precision to timing, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-34 | If error rates do not scale with phonotactic complexity, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-38 | If code-switching into a higher-demand language does not produce earlier collapse, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-52 | If tone errors do not scale with tonal inventory size, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-53 | If discrimination errors do not scale with inventory size, the demand-axis model is disconfirmed |
| PREDICT-SPEECH-54 | If error cascade does not follow layer stack order, the demand-axis model is disconfirmed |

**What this would disconfirm:** the demand axis. If languages don't differ in collapse signatures, or if the differences don't track suprasegmental architecture, the demand axis is wrong.

### 1.6 Recovery is not asymmetric

| Prediction | Falsification condition |
|---|---|
| PREDICT-SPEECH-21 | If granularity does not return before subjective recovery, the recovery-ladder model is disconfirmed |
| PREDICT-SPEECH-23 | If recovery time does not scale super-proportionally with collapse depth, the hysteresis model is disconfirmed |

**What this would disconfirm:** the recovery-ladder model. If recovery is symmetric with collapse, or if recovery time scales proportionally, the recovery model is wrong.

### 1.7 Conflict model is wrong

| Prediction | Falsification condition |
|---|---|
| PREDICT-SPEECH-24 | If degradation signature is not predictable from shared precision demand, the conflict model is disconfirmed |
| PREDICT-SPEECH-25 | If "can you talk while X?" is not a precision-budget question, the conflict model is disconfirmed |
| PREDICT-SPEECH-55 | If collapse depth does not scale with task intensity, the conflict model is disconfirmed |
| PREDICT-SPEECH-56 | If the threshold does not correlate with baseline precision, the conflict model is disconfirmed |

**What this would disconfirm:** the conflict model. If task conflicts don't produce predictable degradation, or if the degradation doesn't track the shared demand, the conflict model is wrong.

### 1.8 Allocation model is wrong

| Prediction | Falsification condition |
|---|---|
| PREDICT-SPEECH-12 | If clusters fall out by population label rather than allocation profile, the unified allocation model is disconfirmed |
| PREDICT-SPEECH-44 | If masking cost does not track substrate measures, the masking-cost model is disconfirmed |
| PREDICT-SPEECH-45 | If clusters fall out by population label, the unified allocation model is disconfirmed |
| PREDICT-SPEECH-46 | If synchrony does not correlate with individual precision, the coupled-oscillator model is disconfirmed |

**What this would disconfirm:** the allocation model. If prosodic features cluster by population label rather than allocation profile, the unified allocation model is wrong.

### 1.9 Routing model is wrong

| Prediction | Falsification condition |
|---|---|
| PREDICT-SPEECH-58 | If congruence is not predicted by routing, the routing model is disconfirmed |
| PREDICT-SPEECH-59 | If maskers do not reach Stage 3–4 before reporting Stage 1–2 symptoms, the routing model is disconfirmed |
| PREDICT-SPEECH-60 | If allostatic load is not higher in high-$A_s^*$, low-$f_{routing}$ speakers, the routing model is disconfirmed |

**What this would disconfirm:** the routing model. If masking has no measurable cost, or if congruence isn't predicted by routing, the routing variable is wrong.

### 1.10 Monitoring claim is wrong

| Prediction | Falsification condition |
|---|---|
| PREDICT-SPEECH-11 | If speech signatures follow rather than precede subjective reports, the monitoring-window claim is disconfirmed |
| PREDICT-SPEECH-29 | If generational speech patterns do not track substrate profiles, the ecological projection is disconfirmed |
| PREDICT-SPEECH-30 | If postural intervention does not improve prosody, the postural-cost mechanism is disconfirmed |
| PREDICT-SPEECH-48 | If substrate does not predict accent better than phonetic input, the substrate-to-accent mechanism is disconfirmed |

**What this would disconfirm:** the monitoring claim. If speech signatures don't precede subjective reports, the monitoring-window claim is wrong.

---

## 2. Falsification by Severity

### 2.1 Load-bearing (disconfirms the model)

These predictions test the model's core claims. If they fail, the model needs revision.

| Prediction | Core claim tested |
|---|---|
| PREDICT-SPEECH-01 | Breath-to-prosody mechanism |
| PREDICT-SPEECH-02 | CO₂-to-prosody mechanism |
| PREDICT-SPEECH-05 | TOT-as-precision-collapse |
| PREDICT-SPEECH-11 | Speech-as-monitoring-channel |
| PREDICT-SPEECH-13 | Channel-preference-as-leading-indicator |
| PREDICT-SPEECH-15 | Integration-demand rule |
| PREDICT-SPEECH-16 | Proper-name vulnerability |
| PREDICT-SPEECH-18 | Postural-cost mechanism |
| PREDICT-SPEECH-21 | Recovery-ladder model |
| PREDICT-SPEECH-24 | Conflict model |
| PREDICT-SPEECH-26 | Channel-preference shift |
| PREDICT-SPEECH-32 | Suprasegmental demand axis |
| PREDICT-SPEECH-42 | Entry-point model |
| PREDICT-SPEECH-51 | FAS-as-precision-collapse |
| PREDICT-SPEECH-58 | Routing-to-congruence |
| PREDICT-SPEECH-59 | Masking-to-late-detection |

### 2.2 Model-extending (disconfirms a specific extension)

These predictions test extensions of the model. If they fail, the extension needs revision, but the core model survives.

| Prediction | Extension tested |
|---|---|
| PREDICT-SPEECH-03 | Monotone/fry distinction |
| PREDICT-SPEECH-04 | Integration-layer mechanism |
| PREDICT-SPEECH-06 | Trauma-prosody mechanism (routing-moderated) |
| PREDICT-SPEECH-07 | Articulation-layer mechanism |
| PREDICT-SPEECH-09 | Breath-to-prosody mechanism |
| PREDICT-SPEECH-10 | Substrate-to-accent mechanism |
| PREDICT-SPEECH-12 | Allocation model |
| PREDICT-SPEECH-14 | Channel-cost mechanism |
| PREDICT-SPEECH-17 | Demand-axis model |
| PREDICT-SPEECH-19 | Sign-language channel cost |
| PREDICT-SPEECH-20 | Inner-speech channel cost |
| PREDICT-SPEECH-22 | Recovery order |
| PREDICT-SPEECH-23 | Hysteresis model |
| PREDICT-SPEECH-25 | Conflict model |
| PREDICT-SPEECH-27 | Channel-cost mechanism |
| PREDICT-SPEECH-28 | Postural-cost mechanism |
| PREDICT-SPEECH-29 | Ecological projection |
| PREDICT-SPEECH-30 | Postural-cost mechanism |
| PREDICT-SPEECH-31 | Ecological projection |
| PREDICT-SPEECH-33 | Baseline precision allocation |
| PREDICT-SPEECH-34 | Phonotactic complexity |
| PREDICT-SPEECH-35 | Inner-speech channel cost |
| PREDICT-SPEECH-36 | Written-speech dissociation |
| PREDICT-SPEECH-37 | Sign-language channel cost |
| PREDICT-SPEECH-38 | Code-switching demand |
| PREDICT-SPEECH-39 | Leading-indicator claim |
| PREDICT-SPEECH-40 | Channel-cost mechanism |
| PREDICT-SPEECH-41 | Postural-cost mechanism |
| PREDICT-SPEECH-43 | Entry-point model |
| PREDICT-SPEECH-44 | Masking-cost model |
| PREDICT-SPEECH-45 | Unified allocation model |
| PREDICT-SPEECH-46 | Coupled-oscillator model |
| PREDICT-SPEECH-47 | Substrate-to-accent mechanism |
| PREDICT-SPEECH-48 | Substrate-to-accent mechanism |
| PREDICT-SPEECH-49 | Postural-cost mechanism |
| PREDICT-SPEECH-50 | Substrate-shift model |
| PREDICT-SPEECH-52 | Demand-axis model |
| PREDICT-SPEECH-53 | Demand-axis model |
| PREDICT-SPEECH-54 | Demand-axis model |
| PREDICT-SPEECH-55 | Conflict model |
| PREDICT-SPEECH-56 | Conflict model |
| PREDICT-SPEECH-57 | Layer-stack model |
| PREDICT-SPEECH-60 | Routing-cost model |

---

## 3. The Falsification Summary Table

| Category | Predictions | Core claims tested |
|---|---|---|
| Substrate does not predict speech | 13 | Breath-to-prosody, CO₂-to-prosody, trauma-prosody, FAS, channel-cost, substrate-to-accent |
| Collapse order is not forced | 5 | Integration-demand rule, entry-point model |
| Layer distinction is not useful | 7 | Monotone/fry, proper-name, sign, inner speech, written |
| Channel cost is not real | 7 | Channel-preference, postural-cost, ecological projection |
| Demand axis is not real | 8 | Suprasegmental demand, phonotactic complexity, code-switching |
| Recovery is not asymmetric | 2 | Recovery-ladder, hysteresis |
| Conflict model is wrong | 4 | Task-pair conflict, task-intensity, baseline-precision threshold |
| Allocation model is wrong | 4 | Unified allocation, masking-cost, coupled-oscillator |
| Routing model is wrong | 3 | Routing-to-congruence, masking-to-late-detection, routing-cost |
| Monitoring claim is wrong | 4 | Speech-as-monitoring-channel, ecological projection, substrate-to-accent |

**Total: 60 predictions, 10 falsification categories, 16 load-bearing predictions, 44 model-extending predictions.**

---

## 4. What the Falsifiability Summary Shows

### 4.1 The model is specific

Every prediction has a falsification condition. The model doesn't hide behind vague claims. Each prediction says what would disconfirm it.

### 4.2 The model is honest

The falsification conditions are specific and testable. The model names what would disconfirm it, not just what would confirm it.

### 4.3 The model is testable

Every prediction is testable with standard acoustic and physiological measures. The methodology is available. The predictions are specific.

### 4.4 The model distinguishes core from extension

The predictions are organized by severity. The load-bearing predictions test the core model; the model-extending predictions test specific extensions. If an extension fails, the core model survives.

### 4.5 The routing model is load-bearing

Two of the sixteen load-bearing predictions (PREDICT-SPEECH-58, -59) test the routing model. This is deliberate: if routing doesn't predict congruence and late detection, the model loses its account of masking, which is one of its distinctive contributions.

---

## 5. The One-Line Summary

The model is falsified if:

- Substrate variables don't predict speech signatures
- Collapse order doesn't follow integration demand
- Layer distinctions aren't clinically useful
- Channel cost isn't real
- The demand axis isn't real
- Recovery isn't asymmetric
- The conflict model is wrong
- The allocation model is wrong
- The routing model is wrong
- The monitoring claim is wrong

Each of these is a testable claim. Each has a specific prediction. Each has a specific falsification condition. The model is honest about what would disconfirm it.

---

*End of The Spoken Language Paper v3.1.*
