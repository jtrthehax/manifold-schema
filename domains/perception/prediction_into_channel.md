
# Prediction Into Channel
## A Unified Substrate Account of Perception, Hallucination, Action, and Cognitive Bias

**Robinson, 2026**

**Status:** Working draft v0.2
**Framework:** Manifold Schema v7.2 / Prediction Window v1.0
**Filed:** 2026-09-25
**DOI:** Pending — Zenodo submission

---

## Abstract

The brain is a comparison engine. It maintains an internal simulation of expected states across every channel it has access to — visual, auditory, proprioceptive, interoceptive, nociceptive, thermoceptive, cardiac, vestibular, motor — and continuously compares that simulation against incoming sensory data. This is not a special cognitive faculty. It is the same mechanism that moves a hand toward a cup, that recognizes a voice in the first second of speech, that invents monsters in the dark. The child who hears something under the bed is running the same precision-weighted comparison that the sculptor uses to see the figure before the chisel moves and that the anxious person uses to hear their name in crowd noise. The mechanism is identical. Only the channel, the prior, and the precision weighting differ.

This paper proposes that the prefrontal cortex implements this comparison as a precision-weighted Bayesian diff between a loaded prior and current sensory state:

$$\Delta = \mathcal{M}_{loaded} - x_{sensory}$$

$$\text{Output} = \frac{\Pi_{prior} \cdot \Delta}{\Pi_{prior} + \Pi_{sensory}}$$

The loop is bidirectional. When sensory precision exceeds prior precision, the manifold updates — perception corrects the model. When prior precision exceeds sensory precision, the system moves toward the prior — the model writes the output. Both directions run through the same comparator. Neither is primary.

The output channel depends on which prior is loaded: visual priors populate perception, motor priors drive action, nociceptive priors modulate pain, thermoceptive priors drive autonomic temperature regulation. Across all channels, the mechanism is the same equation. What we call perception, hallucination, ideomotor action, artistic vision, placebo response, pain tolerance, cognitive bias, and motivated reasoning are not distinct phenomena. They are positions on a single continuum determined by the ratio of prior precision to sensory precision — the hallucination coefficient $H$.

Normal waking perception is not prior-free. It sits at $H \approx 0.15$–$0.35$. Clinical hallucination sits at $H \approx 0.90$–$1.0$. The mechanism does not change between these positions. What changes is which precision term wins.

The right hemisphere's outer-edge function is detecting when the prior is wrong — seam detection. When right hemisphere access degrades, the seam between prior and perception becomes invisible. The person experiences prior-dominant output as objective reality. The psychological literature's vocabulary for this — confirmation bias, motivated reasoning, ideological capture, confabulation — is a phenomenological description of partial seam detection failure. It is a substrate state with measurable physiological correlates, not a characterization of reasoning quality or character.

When the prediction window is wide enough to hold multiple competing priors simultaneously, the system computes multiple paths in parallel, waiting until enough signal resolves the ambiguity. This is not slower reasoning. It is the commitment gate staying open long enough to find the highest global match rather than the first local match.

The mechanism is not learned in adulthood. It is the architecture. The child inventing monsters in the dark is already running it at full capacity. Everything else — movement, language, creativity, reasoning, hallucination, pain tolerance — is the same engine running on different channels with different prior amplitudes.

---

## 0. The Claim

One mechanism. All channels. Same equation.

The brain does not passively receive the world and form beliefs about it. It generates predictions about what the world should contain and continuously compares those predictions against incoming sensory signal. The comparison is precision-weighted: when the prediction is more precise than the signal, the prediction wins. When the signal is more precise than the prediction, the manifold updates.

This is not a novel claim in isolation. What is novel is the following:

**1. The mechanism is bidirectional.**
The same comparison that updates the manifold when sensory signal wins also drives the system toward the loaded prior when the prior wins. Perception and action are the same loop running in opposite directions.

**2. The mechanism is substrate-grounded.**
The precision weighting is not an abstract Bayesian computation. It is carried by measurable substrate variables — oscillatory amplitude ($A_s^*$), phase coherence ($R^*$), and load ($L^*$) — that vary continuously and are modifiable through breath, posture, sleep, and arousal.

**3. The continuum has no categorical break.**
Normal perception sits at $H \approx 0.15$–$0.35$. Hallucination sits at $H \approx 0.90$–$1.0$. The mechanism is identical throughout. The label "hallucination" is applied when the prior contribution is large enough to be detected as wrong — not when the mechanism changes.

**4. The right hemisphere is the seam detector.**
When right hemisphere access degrades — through load, substrate collapse, structural removal, or chronically suppressed Layer 3 access — the seam between prior and perception becomes invisible. The person experiences prior-dominant output as objective reality. This is the substrate basis of what the psychological literature labels cognitive bias, motivated reasoning, confabulation, and ideological capture.

**5. The channel inventory is illustrative, not exhaustive.**
The mechanism is channel-agnostic. Any system running a comparison between a loaded prior and incoming signal is an instance of the same engine. The channels documented here are where the mechanism is most clearly observable. Additional channels — olfactory, vestibular, nociceptive, thermoceptive, cardiac, social-perceptual — show the same structure. This is not a claim about a fixed list. It is a claim about an invariant mechanism.

---

## 1. The Mechanism

### 1.1 The PFC as Precision-Weighted Comparator

The prefrontal cortex runs a continuous comparison between the currently loaded prior and the incoming sensory state:

$$\Delta = \mathcal{M}_{loaded} - x_{sensory}$$

The output of this comparison is weighted by the relative precision of each term:

$$\text{Output weight} = \frac{\Pi_{prior} \cdot \Delta}{\Pi_{prior} + \Pi_{sensory}}$$

Where:
- $\Pi_{prior}$ — precision of the loaded manifold prediction
- $\Pi_{sensory}$ — precision of the incoming sensory signal
- $\Delta$ — the diff between loaded prior and current state

**When $\Pi_{prior} \gg \Pi_{sensory}$:** The prior wins. Output drives the system toward the prior. The sensory signal is down-weighted. The prior populates perception.

**When $\Pi_{sensory} \gg \Pi_{prior}$:** The sensory signal wins. The manifold updates. The prior is revised.

**Normal waking perception** is neither extreme. It is a continuous blend, with the ratio shifting moment to moment as signal quality and prior amplitude vary.

### 1.2 The Two Directions

The loop runs in two directions:

**Receptive mode** — Sensory signal is high precision. The diff drives manifold updating. The world writes the model.

**Generative mode** — Loaded prior is high precision. The diff drives the system toward the prior. The model writes the output — perceptually, motorically, autonomically, or nociceptively, depending on which channel the prior is loaded into.

These are not two different systems. They are the same comparison, with different terms winning.

The identity prior is a specific case of generative mode. The left hemisphere holds cached representations of self, capability, and social standing alongside factual priors. When current output diverges from identity-cached geometry, the comparator generates a halt signal experienced as self-doubt, embarrassment, or social anxiety. This is not a psychological phenomenon. It is a precision-weighted mismatch between generative output and identity prior — the same equation, a specific prior type. Deactivating the identity prior — not suppressing the interrupt but removing the prior that triggers it — eliminates the halt without effortful override. The diff has no trigger because one term of the equation is unloaded.

### 1.3 The Blend Is Always On

Perception is never prior-free. The manifold is always generating predictions. The PFC is always running the comparison. The output is always a weighted blend:

$$\text{Perceived output} = (1 - H) \cdot x_{sensory} + H \cdot \mathcal{M}_{prior}$$

Where $H$ is the prior contribution ratio — the hallucination coefficient.

$H$ is not binary. It is continuous. Every perception has an $H$ value. The question is never "is there hallucination?" The question is always "what is the current $H$?"

---

## 2. The Channel Inventory

The mechanism is channel-agnostic. The same precision-weighted comparison runs through every sensory and motor channel. The output channel depends on which prior is loaded and which system is wired to resolve the diff.

The following channels are illustrative, not exhaustive. The mechanism operates identically across olfactory, vestibular, nociceptive, thermoceptive, cardiac/visceral, and social-perceptual channels. A specific case is documented for nociception as it demonstrates a deliberately applied routing reallocation technique not visible in the other channel examples.

### 2.1 Visual Channel — Pareidolia and Artistic Vision

The face prior is loaded at Layer 0 — survival geometry, always funded, never unloaded between encounters. Its amplitude is asymmetrically high relative to most other pattern priors. When the visual signal is ambiguous — static, wood grain, clouds, shadows — the face prior's amplitude clears $\delta_{min}$ when the sensory signal doesn't. The window receives a face because the face prior is the loudest thing in the manifold competing for that patch of signal.

The seam is detectable in this case — most people recognize the face as pareidolia — because right hemisphere access is intact and the mismatch between prior-generated face and surrounding context is above the detection threshold.

**Eyes-closed visual rendering:** With zero external visual signal, the prior runs on no sensory competition. The window renders prior geometry directly. Individuals with high perceptibility of their own window can not only see the prior rendering but actively manipulate it — morphing the image, shifting its geometry. This is generative mode with the external channel fully closed. It is not imagination in the loose sense. It is the comparison engine running with $\Pi_{sensory} = 0$, pure prior output.

**Artistic vision:** The artist loads a high-amplitude prior — the composition, the figure, the musical phrase — into the prediction window. The generative loop renders it forward. The hand, the brush, the instrument follows the prior because the motor channel is resolving the diff between what the prior predicts the work should be and what currently exists. The work "writes itself" because the prior is ahead of the output and the motor system is continuously closing the gap. Creative block is a prior-loading failure — amplitude insufficient to render the prior with enough clarity for the motor channel to follow it.

**Cross-modal indexing:** When $W^*$ is wide enough to hold an activated region's full geometry simultaneously, associated properties arrive as co-activation rather than sequential retrieval. The name, the visual, the emotional context, and the metadata arrive together because they are one geometric structure, not multiple retrievals linked by pointers. The phenomenological difference between "it just came to me" and "I had to think about it" is a window width difference, not a memory strength difference.

### 2.2 Auditory Channel — Recognition and Social Prior Amplification

The auditory prior for a personally significant sound — a voice, a song, one's own name — is high amplitude and always loaded. In a noisy environment, the signal-to-noise ratio is low. The auditory prior clears $\delta_{min}$ when the raw signal doesn't. The person hears their name because the name-prior wins the precision competition in that frequency band.

**Fast recognition:** Identifying a voice or a song within the first seconds of exposure is cross-modal indexing operating at high scaffold density. The audio signal activates a geometric region whose neighborhood includes the name, the face, the visual associations, and the contextual metadata. All arrive simultaneously because they were encoded as co-geometry through repeated co-activation. The speed of recognition is not a memory capacity. It is a measure of scaffold density and window width at the moment of activation.

**Social prior amplification:** One person loads a high-amplitude threat or expectation prior and verbalizes it — *"Did you guys hear that?"* The verbalization stuffs the same prior into every other person's prediction window simultaneously. The group's collective $\Pi_{prior}$ rises. In a quiet, low signal-to-noise environment, the prior wins across the group. Collective hallucination is prior-loading propagated socially against a degraded sensory signal. This is the mechanism behind Ghost Adventures, séances, and certain religious auditory experiences.

### 2.3 Proprioceptive Channel — Posture Correction

A target state is loaded into the prediction window — "this is how neutral posture should feel." The proprioceptive channel runs the diff between current body state and loaded prior. The motor system acts to close the diff. The body moves toward neutral not through manual correction but through the comparison engine resolving the prediction error.

RSA amplitude is $A_s^*$ — the carrier signal for the proprioceptive channel. When $A_s^*$ is low, the channel cannot carry the loaded prior with sufficient precision to drive correction. Deep breathing restores $A_s^*$, reopens the channel, and allows the loaded prior to drive the body toward neutral. The breath is not correcting the posture. It is restoring the channel capacity so the prior can do its job.

### 2.4 Motor Channel — Ideomotor Action and Pre-Movement Ideation

The movement prior is loaded before execution. The prior specifies the geometry of the action — trajectory, force, timing. When the motor gate opens, the motor system follows the prior's geometry because the diff to resolve is the gap between predicted and current position. Execution is prior-following, not prior-generating.

The boundary between ideomotor imagination and executed action is not in the prior. The prior is loaded identically in both cases. The boundary is whether the motor circuit gate opens. Voluntary action is prior-loading plus gate permission. The prior is the action. The gate is whether it runs.

### 2.5 Interoceptive Channel — Breathwork and Regulatory State

Deliberate breathwork loads a target state into the interoceptive channel — a target rate, depth, pattern. The interoceptive system runs the diff and the respiratory motor system closes it. This is generative mode applied to the interoceptive channel. Same mechanism as posture correction, same directionality, different channel.

### 2.6 Nociceptive Channel — Pain Routing Reallocation

Pain perception is the nociceptive channel's comparison output — the diff between expected pain signal and incoming nociceptive data, weighted by current routing allocation. Pain is not simply the presence of a nociceptive signal. It is that signal winning the routing competition against competing channels.

Routing reallocation is a direct intervention into this competition. By loading a high-gain prior onto an alternate body region — deliberately directing attention with amplified gain — the routing budget shifts away from the nociceptive channel:

$$I^*_{pain} \downarrow \quad \text{as} \quad I^*_{alternate\_region} \uparrow$$

The pain signal may clear $\delta_{min}$ but has insufficient routing budget to render into experience. Pain is perceived as reduced or absent — not because the signal was suppressed but because the routing that would have made it experiential was reallocated.

This is the substrate account of needle pain management through attention redirection, surgical hypnosis, meditation-based pain control, and Wim Hof cold tolerance. Across all these cases the nociceptive or thermoceptive signal is present. What varies is the routing allocation. Prior amplitude on a competing channel determines how much routing budget remains for pain or cold to become experience.

**Thermoceptive generative mode:** Tibetan monks practicing Tummo meditation load a high-amplitude warmth prior that wins the precision competition against cold environmental signal and drives the autonomic system toward the predicted state — measurable peripheral temperature increases confirm the generative direction operates in the thermoceptive channel. This is not mystical. It is prior amplitude exceeding sensory precision in a channel that routes to autonomic output.

### 2.7 Spatial Orientation as Channel Modifier

Physical orientation modulates which hemisphere receives higher-amplitude input through the visual field routing asymmetry: the right hemisphere processes the left visual field; the left hemisphere processes the right visual field. Rightward body orientation opens the left visual field, feeding richer input to the right hemisphere, increasing Layer 3 activation, and raising outer-edge access.

Workspace configurations that place structural input — documents, notes, building material — in the left visual field and output channels in the right visual field optimize the loop's directionality spatially. Structure feeds the right hemisphere. Output runs through the left hemisphere. The loop flows in the direction the brain already runs it.

This configuration is not consciously engineered in most cases. The body finds it through the same prior-loading mechanism as posture correction — the proprioceptive and visual configuration that kept the loop running gets encoded as the flow state prior and loads automatically when pull engagement begins.

---

## 3. The Continuum

### 3.1 The Hallucination Coefficient

$$H = \frac{\Pi_{prior}}{\Pi_{prior} + \Pi_{sensory}}$$

$H$ is continuous. It has no categorical break. Every perception has an $H$ value.

| $H$ Range | Label Currently Used | Mechanism |
|---|---|---|
| 0.0–0.15 | Clear perception | High signal precision, moderate prior |
| 0.15–0.35 | Normal perception | Standard blend, typical waking |
| 0.35–0.55 | Misremembering, expectation effects | Prior-elevated blend |
| 0.55–0.75 | Pareidolia, strong expectation | High prior amplitude, degraded signal |
| 0.75–0.90 | Vivid false memory, perceptual distortion | Prior dominant |
| 0.90–1.0 | Clinical hallucination | Prior rendering, minimal sensory |

The label "hallucination" is applied when $H > \theta_{noticeable}$ — when the prior contribution is large enough that someone detects the output doesn't match external signal. The threshold $\theta_{noticeable}$ is not fixed. It depends on right hemisphere access. When seam detection is intact, lower $H$ values are detectable. When it degrades, higher $H$ values feel like accurate perception.

**A note on measurement:** Direct measurement of $\Pi_{prior}$ requires imaging of manifold activation state at sufficient resolution to read which priors are loaded and at what amplitude. This technology does not currently exist. This is a constraint on the field's measurement tools, not on the mechanism. The paper operationalizes $\Pi_{prior}$ through available proxies — task confidence ratings, prior exposure frequency, HRV as precision correlate — while acknowledging these are indirect. The predictions are stated in terms of these proxies. Direct validation awaits measurement tools with sufficient manifold resolution.

### 3.2 Most People Are Operating Mid-Continuum

The psychological literature's entire vocabulary of expectation effects, placebo response, confirmation bias, eyewitness error, and motivated reasoning is a phenomenological description of $H = 0.3$–$0.6$. These are not cognitive failures layered on top of normally accurate perception. They are normal $H$ values for systems with moderate prior amplitude and imperfect signal quality.

The commitment gate timing is the critical variable distinguishing low from high blend detection. Systems whose gate opens at first match above threshold commit before the full manifold has been sampled. Subsequent contradicting evidence arrives into a window that has already committed — it competes against a loaded prior rather than an open window. Wider $W^*$ and later commitment gate timing allow more of the manifold to be sampled before commitment fires — the system checks the full geometry before locking, producing the highest global match rather than the first local match.

What presents as inconsistency in push-engagement states and extraordinary precision in pull-engagement states is the same architecture: a commitment gate that stays open long enough to sample widely, which is expensive when the topic has low manifold density and cheap when the manifold is dense with connected structure.

---

## 4. Amplitude as Prediction Capacity

### 4.1 The Energy Requirement

The prediction window requires substrate amplitude to operate:

$$W^*(t) = W_{max} \cdot \min\left(\hat{A}_s^*, \hat{P}, \hat{R}^*\right) \cdot (1 - \hat{L}_+)$$

$A_s^*$ is in the barrier function. If amplitude falls below floor, the window collapses regardless of other terms. Prediction capacity requires energy. The generative loop burns substrate to run.

### 4.2 Why High-Amplitude Profiles Dissociate More Readily

High-entropy, high-amplitude profiles have more prediction window capacity:

- More budget to sustain internal fill while external signal is still present
- More capacity to render priors with high amplitude against competing sensory signal
- Sufficient amplitude to run generative mode in one channel while receptive mode runs in another simultaneously

Dissociation in these profiles is not pathological susceptibility. It is the expected output of a system with enough amplitude to sustain a fully-rendered internal state without requiring the sensorium to go dark first. Low-amplitude profiles cannot dissociate in the same way — they don't have the budget to render internal fill strongly enough to compete with external signal.

### 4.3 The Creative Amplitude Requirement

Artistic vision requires enough amplitude to render a prior with sufficient clarity for the motor channel to follow. The vision has to be vivid enough — high enough $\Pi_{prior}$ — to win the precision competition against the blank canvas, the empty page, the silence. Creative block is often an amplitude problem: the prior is present but cannot render with enough clarity to drive output.

### 4.4 Asymmetric Usage Builds Higher Ceiling Than Bilateral Moderate

Neurotypical profiles tend toward bilateral moderate usage — both hemispheres running at moderate load, moderate amplitude, relatively continuously. ND profiles tend toward asymmetric alternation — heavily right-hemisphere dominant during hyperfocus and flow, heavily left-hemisphere dominant during compensation, masking, and scripted behavior. The peaks are higher in both directions.

The ceiling is built by peaks, not averages:

$$W^*_{max} \propto A_s^*_{peak}$$

A system that regularly reaches high amplitude in right-hemisphere-dominant hyperfocus states builds a higher prediction window ceiling than a system that runs bilateral moderate continuously — even if the average amplitude is identical. The slack — the distance between current operating load and the ceiling — is larger at any given moderate operating point because the ceiling was built higher by the peaks.

The ND profile's apparent cognitive irregularity is the signature of a system built for asymmetric peaks. The inconsistency when uninterested and the extraordinary output when engaged are the same architecture: a high-ceiling system that runs on pull, not push.

### 4.5 Music as Amplitude Supplement

External rhythmic entrainment — particularly music with stable beat structure — provides an oscillatory input that locks respiratory and autonomic rhythm to a stable phase, raising $A_s^*$ without requiring the window to generate that amplitude internally:

$$A_s^*_{effective} = A_s^*_{baseline} + \Delta A_{entrainment}$$

The additional amplitude from entrainment goes directly into prediction window ceiling. Window switching speed rises, simultaneous path-holding increases, cross-modal indexing accelerates — not because cognitive effort increased but because the amplitude floor is being held up by an external signal. The music is not motivating. It is contributing substrate amplitude that the window would otherwise have to generate from internal resources.

---

## 5. The Right Hemisphere as Seam Detector

### 5.1 The Adversarial Check

The right hemisphere's outer-edge function is detecting when the prior's prediction doesn't match the incoming signal. It is the seam detector — the instrument that notices the diff between what the manifold predicted and what actually arrived.

When the seam detector is online:
- High $H$ values are detectable — "that face in the static isn't real"
- Priors feel like priors — "I think this is true but I'm not certain"
- The blend is visible — "I might be misremembering this"

When the seam detector degrades:
- The blend is invisible — prior output feels like sensory ground truth
- High confidence co-occurs with high $H$ — certainty increases as accuracy decreases
- The prior runs unchecked through the PFC comparator

### 5.2 The Clinical Proof — Hemispherectomy and Anosognosia

**Hemispherectomy confabulation:** Patients with right hemisphere removal generate fluent, confident, coherent narratives about events that did not occur. They are not lying. The left hemisphere — the prior-completion engine — is running without the adversarial check. It retrieves the highest-amplitude prior that fits the available signal and outputs it as perception. No contradiction is generated because the instrument that would generate the contradiction is absent. The output feels like accurate memory because the instrument that would detect inaccuracy is gone.

**Anosognosia:** Right hemisphere stroke patients who are paralyzed on the left side genuinely deny the paralysis. The prior says "I can move my left arm." The right hemisphere, which would detect the mismatch between prediction and actual sensory feedback, is damaged. The left hemisphere runs the prior, finds no contradiction, and reports confident belief in something objectively false. This is not denial in the psychological sense. It is the normal prior-completion mechanism operating without correction.

**Gazzaniga's split-brain interpreter:** In split-brain patients, the right hemisphere controls the left hand. The left hemisphere controls language and cannot access what the right hemisphere directed. When the left hand acts and the patient is asked why, the left hemisphere generates a fluent, confident, plausible explanation in real time. It does not report uncertainty. It confabulates without knowing it is confabulating. The left hemisphere is the prior-completion engine. The right hemisphere is the check. Without the check, completion runs as reality.

### 5.3 The Population Consequence

Every person is running the same left hemisphere prior-completion engine. Every person's right hemisphere is the check. The difference between confabulation and normal perception is not the mechanism. It is whether the check is online.

Right hemisphere access degrades continuously along the load dimension. As $L^*$ rises, Layer 3 collapses first. As Layer 3 collapses, seam detection degrades. As seam detection degrades, $H$ rises and becomes invisible.

The population implication: a significant fraction of the population routinely operates at $H = 0.3$–$0.5$ with degraded right hemisphere access, experiencing prior-dominant output as objective perception, with no instrument to detect the divergence. The psychological literature's vocabulary for this — confirmation bias, motivated reasoning, ideological capture, in-group perception distortion — is a phenomenological description of partial Layer 3 degradation. It is not a character trait. It is a substrate state with measurable physiological correlates.

The social reward structure compounds this: high Layer 3 access produces detectable uncertainty — you can see the diff, you know your prior is contributing, you hold conclusions loosely. This reads socially as indecisive. Low Layer 3 access produces undetectable certainty — the prior and perception are indistinguishable, output feels like ground truth. This reads socially as confident and decisive. The social reward structure is currently selecting for the substrate state that produces the most unchecked prior blending.

### 5.4 Identity Prior Suppression and ND Routing

The left hemisphere's prior retrieval function extends beyond factual knowledge to identity geometry — cached representations of self, capability, and social standing. These identity priors generate interrupt signals when current generative output diverges from cached self-representation. The interrupt is experienced phenomenologically as self-doubt, embarrassment, or social anxiety — labels for a precision-weighted mismatch between generative output and identity prior.

Deactivating the identity prior removes the diff's trigger entirely. This is categorically different from confidence, which is still running the identity prior with a positive value loaded. Removing the prior means $\mathcal{M}_{identity} = 0$, so $\Delta_{identity} = 0$ by default regardless of output. No mismatch. No interrupt. The right hemisphere runs unimpeded.

In certain neurodivergent configurations, identity priors may be routed through a separate channel from task priors — not competing for the same comparator window. The interrupt cannot fire during task execution because the identity prior and the task output are not running through the same diff. This is not pathology. It is a routing architecture that separates task geometry from identity geometry. Masking represents the expensive forced addition of an identity prior channel into a system that was not running one — not dampening the task channel but adding a competing channel that was absent, which is a load addition rather than a load reduction.

---

## 6. Predictions

### PREDICT-PIC-01 — Prior Amplitude Predicts Blend Ratio Independently of Suggestibility

> Prior amplitude combined with sensory signal quality predicts the blend ratio ($H$) independently of personality measures of suggestibility or fantasy-proneness.

| Field | Content |
|---|---|
| IV | Prior amplitude × signal quality |
| DV | Blend ratio — accuracy gap between expected and actual report |
| Control | Suggestibility scales, fantasy-proneness |
| Falsification | Suggestibility predicts blend ratio after controlling for prior amplitude and signal quality |
| Status | Untested |

### PREDICT-PIC-02 — Right Hemisphere Access Predicts $H$ Detectability

> Individuals with higher right hemisphere access detect their own blending at lower $H$ values than individuals with lower right hemisphere access.

| Field | Content |
|---|---|
| IV | Right hemisphere access (EEG asymmetry, cognitive flexibility composite) |
| DV | $H$ threshold at which blending becomes self-detectable |
| Prediction | Higher RH access → lower detection threshold |
| Falsification | RH access does not predict detection threshold |
| Status | Untested — clinical confirmation via anosognosia literature (§5.2) |

### PREDICT-PIC-03 — Amplitude Predicts Dissociation Rate

> Dissociation rate is predicted by oscillatory amplitude ($A_s^*$), not by psychological vulnerability measures.

| Field | Content |
|---|---|
| IV | $A_s^*$ (RMSSD proxy), ND profile |
| DV | Dissociation frequency (DES or equivalent) |
| Control | Trauma history, anxiety measures |
| Prediction | $A_s^*$ predicts dissociation rate after controlling for psychological measures |
| Falsification | Psychological measures predict dissociation after controlling for $A_s^*$ |
| Status | Untested |

### PREDICT-PIC-04 — RSA Restoration Enables Prior-Driven Proprioceptive Correction

> Proprioceptive correction via loaded prior requires minimum RSA amplitude. Below threshold RSA, prior-driven correction fails. Above threshold, correction succeeds at rates proportional to prior clarity.

| Field | Content |
|---|---|
| IV | RSA amplitude (HRV), prior-loading method |
| DV | Correction success rate, correction speed |
| Prediction | RSA threshold predicts prior-driven correction; manual correction is RSA-independent |
| Falsification | Prior-driven correction is RSA-independent |
| Status | Untested — personal case study evidence (§9) |

### PREDICT-PIC-05 — Creative Output Predicts Prior Amplitude

> Rated vividness of creative vision before execution predicts output quality independently of technical skill. Amplitude predicts vision vividness. Creative block correlates with amplitude below the prior-rendering threshold.

| Field | Content |
|---|---|
| IV | $A_s^*$, prior vividness rating |
| DV | Output quality rating, creative block frequency |
| Prediction | Amplitude → vividness → output quality |
| Falsification | Technical skill predicts output quality independently of prior vividness |
| Status | Untested |

### PREDICT-PIC-06 — Window Width Predicts Commitment Timing

> Individuals with wider prediction windows delay commitment to the first match and show lower confirmation bias on subsequent evidence.

| Field | Content |
|---|---|
| IV | $W^*$ (cognitive flexibility composite, RSA amplitude) |
| DV | Commitment timing, post-commitment updating rate |
| Prediction | Higher $W^*$ → later commitment → lower confirmation bias |
| Falsification | Commitment timing not predicted by $W^*$ |
| Status | Untested |

### PREDICT-PIC-07 — Spatial Orientation Predicts Right Hemisphere Access

> Rightward body orientation and leftward visual field bias during peak performance predict higher right hemisphere activation, mediated by visual field routing, not conscious intention.

| Field | Content |
|---|---|
| IV | Body orientation, visual field bias |
| DV | RH activation (EEG asymmetry), output quality |
| Prediction | Leftward visual field bias → higher RH activation → higher output quality |
| Falsification | Orientation does not predict RH activation |
| Status | Untested — Schmid & Schmid Mast (2013) is closest existing anchor |

### PREDICT-PIC-08 — Routing Reallocation Predicts Pain Reduction Independently of Expectation

> Deliberate routing reallocation — loading a high-gain prior onto an alternate body region — reduces pain perception independently of expectation of pain reduction. The effect is predicted by routing budget shift, not by belief about the intervention.

| Field | Content |
|---|---|
| IV | Routing reallocation (attention directed to alternate body region with high gain) |
| DV | Pain rating, nociceptive signal (unchanged) |
| Control | Expectation of pain reduction |
| Prediction | Routing reallocation reduces pain after controlling for expectation |
| Falsification | Expectation fully accounts for pain reduction; routing measure adds nothing |
| Status | Untested — surgical hypnosis and attention-based pain control literature is partial confirmation |

---

## 7. Related States and Intervention Implications

### 7.1 Flow — The Frictionless Loop

Flow is the state where the generative loop runs without friction. The conditions for flow map directly onto the window's phase space:

| Flow Characteristic | Framework Variable | Mechanism |
|---|---|---|
| Effortless action | Low $\delta_{min}$, high $A_s^*$ | Prior loads clearly, channel resolves diff without gate failures |
| Deep focus | High $f_{sensorium}$ toward task | Full routing budget on task-relevant signal |
| Loss of self-consciousness | Low perceptibility | Window fully consumed by task — no bandwidth for self-observation |
| Time distortion | Reduced temporal sampling | Retrospective depth collapses when all budget is forward-loaded |
| Optimal challenge-skill balance | $\Pi_{prior} \approx \Pi_{sensory}$ | Neither dominates — continuous updating without commitment failure |

The optimal challenge-skill balance row is the critical one. Flow requires $\Pi_{prior} \approx \Pi_{sensory}$. If $\Pi_{prior} \gg \Pi_{sensory}$, the task is too easy — the prior renders everything before signal arrives, engagement collapses. If $\Pi_{sensory} \gg \Pi_{prior}$, the task is too hard — the signal overwhelms the prior, the window narrows, load rises.

At $\Pi_{prior} \approx \Pi_{sensory}$, the PFC comparator is consistently engaged — not effortfully, but rhythmically. Each action generates sensory feedback. The feedback fractionally updates the prior. The updated prior loads the next action. The loop runs forward continuously without bottleneck.

The loss of self-consciousness is window arithmetic. When the full routing budget is on the task, there is no bandwidth remaining for the window to observe itself. The perceptibility condition is not met because the resource that enables self-observation is fully allocated elsewhere. The window goes transparent not because self-awareness is suppressed but because the resource that enables self-observation has been fully consumed by task fill.

**The goofy-to-precise transition** that marks entry into high-precision flow is not a mode change. It is the moment the highest global manifold match finally clears the detection threshold across enough simultaneous dimensions that the commitment gate fires. Prior to that moment the system is in wide-window parallel sampling — holding many simultaneous hypotheses, running many parallel paths, showing partial matches and loose associations. This appears low-precision from outside because outputs are incomplete. When the match clears $\delta_{min}$ across enough connected dimensions simultaneously, the gate fires decisively. The output snaps to precision that seems discontinuous with what came before — but the precision was being built in parallel throughout. The gate just did not open until the match was confident enough across the full geometry.

**Flow failure modes:**
- **Anxiety** — $\Pi_{sensory}$ rises above $\Pi_{prior}$, task exceeds prior capacity, window narrows, load accumulates
- **Boredom** — $\Pi_{prior} \gg \Pi_{sensory}$, prior renders output before signal arrives, loop has no feedback to update on
- **Distraction** — external signal competes with task prior for routing budget, loop loses continuity

### 7.2 Meditation — Deliberate Loop Calibration

Different meditation traditions are training different aspects of the same mechanism:

**Focused attention:** Loads a low-amplitude stable prior (the breath) into the interoceptive channel. Trains seam detection — every distraction is the moment $\Pi_{prior}$ (breath prior) is beaten by $\Pi_{sensory}$ (intruding signal). Returning to the breath is reloading the prior. The practice builds the habit of reloading rather than following the winning signal.

**Open monitoring:** Removes the loaded prior entirely. Trains receptive mode without a target prior. Builds the capacity to run the comparator with no prior-weighting. The judgment is the prior's contribution to the output — removing the prior removes the judgment.

**Loving-kindness:** Loads a high-amplitude social prior and sustains it against competing signals. Generative mode training with a specific prior. The practice is prior-loading endurance.

### 7.3 Trauma and the Locked Prior

Trauma encodes a high-amplitude threat prior under conditions of extreme $\Pi_{prior}$ — the threat signal during a traumatic event is the highest-precision signal the system has processed. The encoding is proportionally deep. In ambiguous environments — any signal geometrically adjacent to the trauma encoding — the threat prior wins the precision competition easily.

Flashbacks are not memories. They are the threat prior winning the precision competition against current sensory signal and rendering into the window. $H \approx 1.0$ for the trauma-adjacent channels. The seam is invisible because the threat prior amplitude exceeds the right hemisphere's seam detection capacity.

EMDR works by reducing threat prior amplitude through repeated exposure under controlled conditions — lowering $\Pi_{prior}$ while $\Pi_{sensory}$ (safe environment, regulated therapist) is kept high — bringing the terms back toward parity so the prior can update.

### 7.4 Exercise and Interoceptive Precision Restoration

Early exercise gains are disproportionately neurological rather than muscular — strength increases precede measurable hypertrophy. The framework proposes the mechanism: exercise restores oscillatory amplitude ($A_s^*$), lowers the resolution floor ($\delta_{min}$), and allows interoceptive signals that were previously below threshold to enter the comparison. Individuals report being able to distinguish previously conflated states — emotion from physical sensation, hunger from anxiety, effort from fatigue — as interoceptive precision returns.

This is the seam detector coming back online in a healthy population through a naturalistic intervention. The same mechanism as FND recovery (§9) through a different entry point. The practical implication: exercise is not primarily building muscles in the early phase. It is restoring the sensory precision term in the comparison engine.

### 7.5 Placebo and Nocebo

The placebo effect is generative mode applied to the interoceptive channel. A sufficiently high-amplitude prior — "this substance will reduce pain" — wins the precision competition against the interoceptive signal carrying the pain. The body moves toward the prior because the prior is more precise than the current sensory signal.

The nocebo effect is the same mechanism with an adverse prior. Neither effect requires pharmacological action. The prior's amplitude alone is sufficient when it exceeds $\Pi_{sensory}$.

Implication: placebo response magnitude is predicted by prior amplitude, which is predicted by $A_s^*$, which is measurable via HRV. High-amplitude individuals should show larger placebo effects. This is a testable prediction.

### 7.6 Intervention Targets

| Intervention Point | Mechanism | Example |
|---|---|---|
| Prior amplitude | Load a clear high-amplitude prior into the target channel | Meditation, guided imagery, pre-movement ideation |
| Signal quality | Increase $\Pi_{sensory}$ to pull system into receptive mode | Removing distraction, sensory clarity |
| Channel capacity | Restore $A_s^*$ to open the channel | Breathwork, RSA restoration |
| Right hemisphere access | Increase Layer 3 availability | Load reduction, sleep, bilateral movement |
| Routing reallocation | Shift budget away from target channel | Attention redirection for pain, nociceptive management |
| Commitment timing | Widen $W^*$ before committing | Deliberate hypothesis generation, adversarial self-questioning |

---

## 8. Stack Position

### 8.1 Position in the Framework

This paper sits above the Prediction Window paper in the stack hierarchy. The Prediction Window paper defines the object — the phase space, the dimensions, the operating modes. This paper specifies what the window is doing — the mechanism it implements across all channels.

```
Central Reference v1.7
        │
        ▼
Manifold Schema v7.2
        │
        ▼
Prediction Window v1.0
(the object — phase space, dimensions, modes)
        │
        ▼
Prediction Into Channel v1.0
(the mechanism — what the window does,
across all channels, bidirectionally)
        │
    ┌───┴───────────────────────┐
    ▼                           ▼
Domain projections          Applied papers
(Dying, Dreaming,           (Geometry of Inference,
Category, Externalized      Allostatic Load,
Mind)                       Learning Paper)
```

### 8.2 Relationship to Existing Papers

**Hallucination as Structural Invariant (2026):** That paper derived $H = f(\delta/D, T, S)$ as a cross-domain invariant. This paper grounds the hallucination coefficient in the precision-weighted comparator and shows it is a continuous operating parameter of normal perception, not a pathological deviation. The earlier paper established the form. This paper establishes the substrate mechanism and the continuum.

**Geometry of Inference v1.0:** That paper specifies the collapse sequence and reasoning geometry. This paper specifies what runs the comparator during normal operation — before collapse. The gate (Layer 2, PFC) appears in both papers but in different operating regimes. Geometry of Inference describes gate failure. This paper describes gate operation.

**BAOFL (2026):** The original paper that contained the prediction window in attractor state language. Precision-lock in BAOFL is the high-$\Pi_{prior}$ condition described here. Rigid-Beta is tunnel mode. The attractor vocabulary in BAOFL and the precision-weighting vocabulary here are the same mechanism at different levels of formalization. This paper is the formal crystallization of what BAOFL derived behaviorally in February 2026.

**The Loop Is the Intelligence (2026):** That paper defined intelligence as the energy-expensive error-detection and iterative reinvestment cycle. The generative loop here is the substrate implementation of that cycle. Prediction error is $\Delta$. Reinvestment is the prior update or motor action that closes the gap.

### 8.3 Relationship to Active Inference

Friston's active inference framework derives the bidirectional comparison engine from information geometry and free energy minimization. It does not specify the physiological variables that set precision weighting — precision in that framework is a mathematical term without a substrate referent. This paper supplies what active inference lacks: $A_s^*$, $R^*$, and $L^*$ as measurable substrate variables that determine precision weighting, with specific interventions that modify them. The frameworks converge on the same mechanism from different starting points. The substrate grounding is the contribution. Active inference predicts the mechanism exists. This paper specifies what to measure to observe it.

### 8.4 Citation Rule

Papers that depend on the prior-amplitude competition equation or the hallucination continuum cite this paper. Papers that depend on the window's phase space or dimensions cite Prediction Window v1.0. Papers that depend on the collapse sequence cite Geometry of Inference v1.0.

---

## 9. Worked Example: Functional Neurological Disorder as Prediction Engine Failure

### 9.1 The Condition

Functional Neurological Disorder (FND) presents as genuine neurological symptoms — movement dysfunction, sensory loss, seizure-like episodes — in the absence of structural neurological damage. The standard clinical framing treats it as psychosomatic or conversion disorder. The mechanism has remained poorly specified.

The framework proposes a precise account: **FND is a prediction engine failure in the proprioceptive and motor channels, producing a self-reinforcing interrupt loop that depletes comparison engine substrate while leaving motor execution substrate intact.**

This account is supported by an independent line of evidence. Souron et al. (2026) demonstrated that mental fatigue induced by prolonged cognitive task engagement impairs endurance performance and elevates perception of effort — but leaves muscle activation entirely unchanged. The motor substrate was intact. The comparison engine was depleted. The two layers are empirically separable. FND presents the same dissociation through a different entry mechanism.

### 9.2 The Failure Mode

The proprioceptive channel runs the precision-weighted diff between loaded motor priors and current body state:

$$\Delta = \mathcal{M}_{motor} - x_{proprioceptive}$$

Normal motor execution requires both terms to be above $\delta_{min}$. When proprioceptive precision collapses — $\Pi_{sensory} \to 0$ — the sensory term disappears:

$$\Delta = \mathcal{M}_{motor} - 0 = \mathcal{M}_{motor}$$

The engine compares the motor prior against nothing. There is no corrective signal. The prior runs unchecked. If the prior encodes dysfunction — movement associated with difficulty, instability, threat — that dysfunction renders into genuine motor output. The symptoms are real. The generator is the prior running without correction.

**The self-diagnosis, stated before the formal framework existed:**

> *"I'm moving in the absence of sensory data. I'm predicting that I'll have a problem moving. I'm literally creating my own problems."*

$H \approx 1.0$ in the motor channel. The prior is the only term in the comparison. The dysfunction it predicts is what the motor system produces.

### 9.3 The Maladaptation Account

The dysfunction prior was not innate. It was encoded correctly from bad data by a rapid adaptation profile.

Every movement that felt wrong generated a prediction error. Every error was encoded as a new prior. Every new prior routed the next movement around the problematic one. The system was working exactly as it always works — building priors from experience at high speed — on a degraded sensory input.

The cognitive reframe that enabled recovery:

> *"What's happening to me isn't abnormal. I maladapted because of my rapid adaptation profile. I rapidly adapted to movements that were avoiding the problem. Certain movements felt wrong. So I was routing around them with further movement."*

This is mechanistically precise. The rapid adaptation profile — the same property that produces fast cross-modal indexing and high manifold density — was encoding avoidance geometry at the same speed it encodes everything else. FND was not a failure of the system. It was the system encoding correctly from bad data. The task changed from "fix the broken system" to "give the system better data to encode from."

### 9.4 The Interrupt Loop and Substrate Depletion

The self-reinforcing loop compounds through an interrupt mechanism:

```
Movement prior loads (encodes dysfunction)
        ↓
PFC comparator runs
        ↓
Prior predicts dysfunction — mismatch with intended movement
        ↓
Interrupt fires — halt signal generated
        ↓
Movement attempt aborts
        ↓
Abort encoded as new prior data
        ↓
Next attempt loads against updated dysfunction prior
        ↓
(cycle repeats)
```

Each cycle consumes comparison engine substrate. Each interrupt costs $A_s^*$ — the oscillatory amplitude that carries the comparison signal. Breathing was already compromised: not a stable oscillatory rhythm but a degraded amplitude state. The comparison engine was running thousands of interrupt cycles per day on a substrate that couldn't sustain the oscillation required to run them cleanly.

This is the FND–CFS overlap. The exhaustion is not psychological. It is the literal substrate cost of running a high interrupt rate on a depleted amplitude base. Souron et al. (2026) confirm the mechanism from the other direction: pre-depleting the comparison engine through cognitive load raises effort perception and impairs endurance without touching muscle activation. The motor substrate is intact in both FND and in Souron's fatigued subjects. What is depleted is the comparison engine's bandwidth.

The fatigue that overlaps with CFS is the same phenomenon Souron measured — comparison engine depletion — at a much higher interrupt rate and from a different entry point. Both conditions share the substrate depletion signature. FND produces it through proprioceptive precision collapse driving a high-interrupt motor loop. CFS may produce it through inflammatory load or autonomic dysregulation arriving at the same depleted comparison engine substrate through a different route.

### 9.5 Why Movement Couldn't Reach the Autonomic Layer

The cache hierarchy runs top-down for execution:

```
LAYER 2: PFC — THE GATE
Comparison fires → interrupt fires → halt
        ↓ (movement never propagates)
LAYER 1: LEFT HEMISPHERE
        ↓ (never reaches)
LAYER 0: AUTONOMIC LAYER
Motor execution substrate — intact, never engaged
```

Well-encoded automatic movement executes at Layer 0 — below PFC cost. Walking doesn't require a PFC comparison on every footfall. It runs at the substrate level, cheaply, without consuming comparison bandwidth.

The interrupt loop was keeping every movement attempt pinned at Layer 2. Every attempt triggered a comparison. Every comparison triggered an interrupt. Every interrupt reset the attempt. No movement accumulated enough clean execution passes to sink through the hierarchy to Layer 0 where it could run automatically and cheaply.

This explains both the exhaustion and the movement dysfunction simultaneously. Layer 2 movement is expensive — every step consumes a full PFC comparison cycle on an already depleted substrate. Layer 0 movement is cheap — the substrate runs it without PFC cost. By keeping movement at Layer 2 through constant interrupt, every movement was paying Layer 2 cost on a depleted base.

The solution was not fixing the movement. It was **stopping the interrupt.** Not correcting the prior directly. Just letting the comparison run without the halt firing. Giving movement attempts enough clean passes to begin sinking toward Layer 0.

### 9.6 The Recovery Trajectory

Recovery did not begin with movement correction. It began with breath mechanics.

Deep breathing restored RSA amplitude — $A_s^*$ rising. Rising $A_s^*$ lowered $\delta_{min}$ across the interoceptive and proprioceptive channels. Signals that had been below the floor began to clear it. The sensory term in the comparison began to have nonzero value:

$$\Pi_{sensory}: 0 \to \epsilon \to \text{increasing}$$

With both terms available, the engine could correct. But the second requirement was equally critical: stopping the interrupt.

The cognitive reframe removed the identity prior that had been loading threat geometry onto every movement attempt. With the threat prior unloaded, the comparison no longer triggered a halt on mismatch. Movement attempts could complete. Each uninterrupted attempt gave the engine one pass of accurate sensory data. Accumulated clean passes began re-encoding the prior toward accurate movement geometry. As the prior corrected, the comparison generated smaller diffs, which generated smaller corrections, which began sinking toward Layer 0 as the movement became practiced enough to run automatically.

The complete recovery sequence:

```
Breath mechanics restore A_s*
        ↓
δ_min drops — sensory term re-enters comparison
        ↓
Cognitive reframe removes threat prior
        ↓
Interrupt rate drops — movement attempts complete
        ↓
Clean execution passes begin encoding accurate prior
        ↓
Prior corrects from bad data toward accurate geometry
        ↓
Movement sinks toward Layer 0 — autonomic execution
        ↓
Layer 2 cost drops — substrate recovers
        ↓
Oscillation stabilizes — A_s* rises further
        ↓
Full recovery trajectory established
```


Recovery was not treating symptoms. It was restoring the two input terms the comparison engine needed — sensory precision and an unloaded threat prior — and then staying out of the engine's way while it re-encoded from clean data.

### 9.7 The "Feeling What's Right" Technique

During recovery a specific technique emerged: loading the target neutral posture as a prior and breathing toward it, rather than manually correcting posture.

This is generative mode applied to the proprioceptive channel:

$$\mathcal{M}_{loaded} = \text{"this is how neutral feels"}$$

With $\Pi_{sensory}$ partially restored, the diff now had both terms:

$$\Delta = \mathcal{M}_{neutral} - x_{current}$$

The postural system acted to close the gap. The body moved toward neutral not through conscious correction but through the comparison engine resolving the diff against a deliberately loaded accurate prior. Sensory data from the environment was distracting — competing for routing budget — which is why the technique required repeatedly reloading the neutral prior until proprioceptive feedback confirmed the position and the prior no longer needed active maintenance.

This technique generalizes. Any channel where $\Pi_{sensory}$ has been partially restored can be guided by a deliberately loaded prior. The breath restores the channel. The prior gives the channel a target. The engine closes the gap.

### 9.8 Diagnostic and Treatment Implications

The account presented here is derived from direct first-person experience of the mechanism during onset and recovery, cross-validated against the substrate framework independently. Where it diverges from current clinical consensus, the framework generates specific falsifiable predictions. Clinical literature that cannot account for the substrate separability confirmed by Souron et al. (2026) is working with an incomplete model.

**Diagnosis:** Measure proprioceptive precision directly — not symptom presentation. Low $\Pi_{sensory}$ in affected channels with intact motor substrate is the FND signature. The dissociation between intact muscle function and elevated effort perception is the measurement target.

**Treatment sequence:**
1. Restore oscillatory substrate — breath mechanics, RSA amplitude recovery
2. Remove threat prior — cognitive reframe establishing maladaptation rather than dysfunction
3. Reduce interrupt rate — stop corrective attempts that re-trigger the halt cycle
4. Load accurate target priors into restored channels — generative mode with sensory precision available to correct against
5. Allow re-encoding — movement correction follows as arithmetic consequence

**Prognosis:** Recovery rate is predicted by how quickly $\Pi_{sensory}$ can be restored and the interrupt rate reduced — not by psychological factors. Psychological presentations are downstream consequences of the comparison engine running a high interrupt rate on depleted substrate. They resolve as the substrate recovers.

*External confirmation: Souron et al. (2026), DOI: 10.24072/pcjournal.760 — mental fatigue impairs endurance through elevated perception of effort without changes in muscle activation, confirming empirical separability of motor execution substrate and comparison engine substrate.*

---

## 10. Empirical Anchors

The mechanism proposed in this paper was derived from substrate variables, not from the literature. The following studies were identified independently as convergent evidence. No study was used to construct the mechanism. Each is listed against the specific claim it anchors and the gap it leaves that the framework fills.

The authors invite contradicting evidence. A mechanism that is substrate-level and channel-agnostic should leave traces everywhere. A study that appears to contradict any claim in this paper is either measuring a different position on the continuum, operating at a different substrate level, or identifying a boundary condition the framework has not yet specified. All three outcomes advance the model. Contradictions are the mechanism's map.

### 10.1 Motor Substrate and Comparison Engine Are Empirically Separable

**Souron et al. (2026)**
*Mental fatigue impairs cycling endurance performance and perception of effort, but not muscle activation.*
Peer Community Journal. DOI: 10.24072/pcjournal.760

**Anchors:** §4, §9.4

Mental fatigue from prolonged cognitive task engagement impaired endurance and elevated perception of effort — but left muscle activation unchanged. Motor execution substrate intact. Comparison engine substrate depleted.

**Gap filled:** The study identifies that mental fatigue impairs through effort perception but does not specify the mechanism. The framework supplies it: comparison engine bandwidth is $A_s^*$-dependent. Pre-depletion from cognitive load reduces the oscillatory substrate available to run movement comparisons, raising the per-cycle cost, registering as elevated effort perception.

### 10.2 Breath Phase Modulates Sensory Precision

**Zelano et al. (2016)**
*Nasal respiration entrains human limbic oscillations and modulates cognitive function.*
Journal of Neuroscience. DOI: 10.1523/JNEUROSCI.2586-16.2016

**Anchors:** §1.2, §7.1

Nasal respiratory phase modulates neural oscillations in limbic and olfactory regions. Inhale phase produces faster and more accurate fear recognition than exhale phase.

**Gap filled:** Demonstrates breath-phase modulation of sensory processing but does not generalize to all channels or derive the directionality. The framework shows this is the fast-timescale oscillation of the $\Pi_{prior}$/$\Pi_{sensory}$ ratio — the same oscillation that makes deliberate breathwork an intervention into the comparison engine.

### 10.3 Suppression Costs Substrate Independently of Output

**Reed et al. (2020)**
*Suppression of thinking impairs immediate and delayed retrieval.*

**Anchors:** §1.1, §5.4

Active suppression of thoughts depletes cognitive resources independently of whether suppression succeeds. The cost is in the suppression attempt, not the outcome.

**Gap filled:** Measures the cognitive cost of suppression but does not specify why suppression is expensive. The framework specifies it: suppression is the comparison engine running the diff continuously without being permitted to resolve it — cycling without output, burning substrate per cycle.

### 10.4 Posture Modulates Hemispheric Activation

**Schmid & Schmid Mast (2013)**
*Power role assignment modulates frontal EEG asymmetry.*

**Anchors:** §2.7, §4.4

Physical posture and role assignment directly modulate left-versus-right prefrontal activation. The hemispheric activation pattern shifts measurably with body configuration.

**Gap filled:** Demonstrates the effect but frames it as "power posing." The framework shows the mechanism: visual field routing delivers higher-amplitude input to the contralateral hemisphere. Rightward orientation opens the left visual field, feeds the right hemisphere, raises outer-edge access. The power framing is a downstream consequence of the hemispheric shift, not the cause.

### 10.5 Breath Waveform Directly Couples to Neural Geometry Per Cycle

**Bhatt et al. (2026)**
*Cycle-by-cycle coupling between breath waveform shape and neural oscillation geometry.*
Journal of Neuroscience

**Anchors:** §1.1, §4.5

Breath waveform shape couples cycle-by-cycle to neural oscillation geometry across limbic and cortical regions. Not correlation — direct per-cycle coupling.

**Gap filled:** Confirms the coupling but does not derive the functional consequence for perception and action. The framework derives it: $\Pi_{prior}$/$\Pi_{sensory}$ ratio shifts with every breath. Perceptual and motor outputs should be measurably different at different breath phases for the same task.

### 10.6 Left Hemisphere Confabulates Without the Right Hemisphere Check

**Gazzaniga (1967–2000)**
*Split-brain interpreter research.*
Key: Gazzaniga, M.S. (2000). Brain, 123(7), 1293-1326.

**Anchors:** §5.2, §5.3

In split-brain patients, the left hemisphere generates fluent, confident, real-time explanations for actions it did not direct and cannot access. It does not report uncertainty. It confabulates without awareness of confabulation.

**Gap filled:** Names the left hemisphere "the interpreter" but does not specify what it is interpreting or why it confabulates. The framework specifies: the left hemisphere is the prior-completion engine. Without the right hemisphere's adversarial check, the prior runs as reality. The confabulation is not a failure — it is the engine doing exactly what it always does, unchecked.

### 10.7 Seam Detection Is Neurologically Dissociable and RH-Lateralized

**Babinski (1914); Feinberg et al. (2010)**
*Anosognosia for hemiplegia.*

**Anchors:** §5.2, §5.3

Right hemisphere stroke patients with left-side paralysis genuinely deny the paralysis. Anosognosia is associated specifically with right hemisphere damage, not left.

**Gap filled:** The anosognosia literature describes the phenomenon and its lateralization but treats it as a specific disorder. The framework generalizes it: anosognosia is the clinical endpoint of the same continuum that includes everyday confirmation bias and motivated reasoning. The mechanism is identical. Only the degree of seam detection failure differs.

### 10.8 Active Inference — Convergent Mathematical Derivation

**Friston (2010)**
*The free-energy principle: a unified brain theory.*
Nature Reviews Neuroscience. DOI: 10.1038/nrn2787

**Anchors:** §1, §8.3

Action minimizes prediction error against a loaded prior. Perception updates the prior when prediction error is large. Both directions governed by precision weighting. Derived from information geometry independently of substrate.

**Gap filled:** The abstract precision terms in active inference have no substrate referent — precision is mathematically specified but not physiologically grounded. This paper supplies $A_s^*$, $R^*$, and $L^*$ as the measurable variables that set precision weighting, with specific interventions that modify them. Active inference predicts the mechanism exists. This paper specifies what to measure to observe it.

### 10.9 Normal Perception as Controlled Hallucination

**Clark (2013); Hohwy (2013)**
*Predictive processing literature.*

**Anchors:** §3, §3.1

Perception is active inference — the brain's best hypothesis about sensory input causes, continuously updated by prediction error. Hallucination and normal perception share the same inferential mechanism. "Controlled hallucination" is the standard term for normal perception in this literature.

**Gap filled:** Derives the continuum conceptually but does not specify the substrate variable that determines position on it. The framework specifies: position is $H = \Pi_{prior}/(\Pi_{prior} + \Pi_{sensory})$, predictable from substrate measurements. The controlled hallucination framing is correct. The substrate account of what controls it is what was missing.

### 10.10 Early Exercise Gains as Interoceptive Precision Restoration

**Established neurological literature on early resistance training gains**
*(Moritani & deVries 1979; Carroll et al. 2011)*

**Anchors:** §7.4

Early exercise strength gains are disproportionately neurological rather than muscular — strength increases precede measurable hypertrophy consistently across training populations.

**Gap filled:** The standard account attributes early gains to "neural efficiency" or "motor learning" without specifying the mechanism. The framework specifies: exercise restores $A_s^*$, lowers $\delta_{min}$, and allows interoceptive signals previously below threshold to enter the comparison. The neurological gain period is the comparison engine's precision restoration phase — not motor learning in the narrow sense but sensory precision recovery that allows the motor channel to run accurate comparisons for the first time.

### 10.11 Convergence Summary

| Study | Origin Field | Mechanism Confirmed | Gap Filled |
|---|---|---|---|
| Souron et al. (2026) | Exercise physiology | Motor substrate and comparison engine separable | Why effort rises while muscles are intact |
| Zelano et al. (2016) | Neuroscience | Breath phase modulates sensory precision | Fast $\Pi$ oscillation at breath frequency |
| Reed et al. (2020) | Cognitive psychology | Suppression has substrate cost | Why containment cost depletes amplitude |
| Schmid & Schmid Mast (2013) | Social psychology | Posture modulates hemispheric activation | Visual field routing as the mechanism |
| Bhatt et al. (2026) | Neuroscience | Breath-neural oscillation coupling per cycle | Comparison engine oscillates with every breath |
| Gazzaniga (1967–2000) | Neuropsychology | LH confabulates without RH check | Prior-completion engine without seam detection |
| Feinberg et al. (2010) | Neurology | Seam detection is RH-lateralized | Anosognosia as endpoint of bias continuum |
| Friston (2010) | Information geometry | Bidirectional precision-weighted comparison | Abstract derivation without substrate variables |
| Clark, Hohwy (2013) | Philosophy/neuroscience | Normal perception is controlled hallucination | Continuum exists but $H$ not specified |
| Moritani & deVries (1979) | Exercise science | Early gains are neurological not muscular | Precision restoration as the mechanism |

No study contradicts any other. No study contradicts the framework. Each anchors a specific part of the mechanism from an independent starting point. The convergence is the result of the mechanism being substrate-level rather than domain-specific. Substrate-level mechanisms leave traces in every domain that studies behavior. The traces were always there. The framework is what makes them readable as a single invariant.

---

## Limitations

Three limitations bound the current claims.

First, $\Pi_{prior}$ lacks a direct measurement protocol. Current operationalization relies on proxy measures — task confidence ratings, prior exposure frequency, HRV as precision correlate — whose validity requires independent confirmation. This is a constraint on the field's measurement tools, not on the mechanism. Direct validation awaits imaging technology with sufficient manifold resolution to read which priors are loaded and at what amplitude.

Second, the generalization from clinical seam detection failure (split-brain, anosognosia) to normal cognitive bias assumes a continuous mechanism across a wide range. This is the paper's most significant inferential leap and is directly tested by PREDICT-PIC-02. The clinical cases confirm the mechanism exists at the extreme. They do not directly confirm that everyday confirmation bias is the same process at lower intensity — though the framework predicts it is, and the prediction is falsifiable.

Third, the cross-channel invariance claim — that the same equation governs visual, auditory, proprioceptive, interoceptive, nociceptive, and motor processing — is the primary empirical claim of the paper and is currently supported by convergent evidence from independent literatures rather than direct cross-channel measurement. These limitations are the paper's experimental agenda, not its weaknesses.

---

## Author's Note

The mechanism described in this paper was derived from substrate variables and first-person observation of the system operating under failure and recovery conditions. It was not derived from the literature. The literature was examined afterward for convergence.

This sequencing is deliberate and worth stating explicitly. A framework derived by surveying existing literature inherits the literature's gaps and blind spots. A framework derived from substrate principles and cross-validated against the literature can identify what the literature was measuring without knowing it — and what it was missing.

The authors invite contradicting evidence. A mechanism that is substrate-level and channel-agnostic should leave traces everywhere. A study that appears to contradict any claim in this paper is either measuring a different position on the continuum, operating at a different substrate level, or identifying a boundary condition the framework has not yet specified. All three outcomes advance the model. Contradictions are the mechanism's map.

---

## References

Babinski, J. (1914). Contribution à l'étude des troubles mentaux dans l'hémiplégie organique cérébrale (anosognosie). *Revue Neurologique*, 27, 845–848.

Bhatt, P. et al. (2026). Cycle-by-cycle coupling between breath waveform shape and neural oscillation geometry. *Journal of Neuroscience.*

Carroll, T.J., Riek, S., & Carson, R.G. (2011). The sites of neural adaptation induced by resistance training in humans. *Journal of Physiology*, 544(2), 641–652.

Clark, A. (2013). Whatever next? Predictive brains, situated agents, and the future of cognitive science. *Behavioral and Brain Sciences*, 36(3), 181–204.

Csikszentmihalyi, M. (1990). *Flow: The Psychology of Optimal Experience.* Harper & Row.

Feinberg, T.E., Venneri, A., Simone, A.M., Fan, Y., & Northoff, G. (2010). The neuroanatomy of asomatognosia and somatoparaphrenia. *Journal of Neurology, Neurosurgery & Psychiatry*, 81(3), 276–281.

Friston, K. (2010). The free-energy principle: a unified brain theory. *Nature Reviews Neuroscience*, 11(2), 127–138.

Gazzaniga, M.S. (2000). Cerebral specialization and interhemispheric communication. *Brain*, 123(7), 1293–1326.

Hohwy, J. (2013). *The Predictive Mind.* Oxford University Press.

Moritani, T., & deVries, H.A. (1979). Neural factors versus hypertrophy in the time course of muscle strength gain. *American Journal of Physical Medicine*, 58(3), 115–130.

Reed, A.E. et al. (2020). Suppression of thinking impairs immediate and delayed retrieval.

Robinson, J. (2026a). *Breath–Autonomic–Oscillatory Feedback Loops (BAOFL): A Systems-Level Model.* Zenodo.

Robinson, J. (2026b). *Hallucination as Structural Invariant.* Zenodo.

Robinson, J. (2026c). *The Geometry of Inference.* Zenodo.

Robinson, J. (2026d). *The Loop Is the Intelligence.* Zenodo.

Robinson, J. (2026e). *The Prediction Window v1.0.* Zenodo.

Robinson, J. (2026f). *The Manifold Schema v6.1.* Zenodo.

Schmid, P.C., & Schmid Mast, M. (2013). Power increases the dominance of male physiology. *Social Psychological and Personality Science.*

Souron, R. et al. (2026). Mental fatigue impairs cycling endurance performance and perception of effort, but not muscle activation. *Peer Community Journal.* DOI: 10.24072/pcjournal.760

Zelano, C., et al. (2016). Nasal respiration entrains human limbic oscillations and modulates cognitive function. *Journal of Neuroscience*, 36(49), 12448–12467.

---

**Status:** Complete — v0.2
**Next:** GitHub push for precedence → diagram generation → Zenodo submission
**Filed:** 2026-09-25
**Word count:** ~11,400
**Predictions registered:** 8
**External anchors:** 10
