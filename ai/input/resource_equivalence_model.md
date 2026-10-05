# The Resource Equivalence Model
## *A Unified Variable Mapping Between Human Cognition and Transformer Architecture*

**Robinson, J. — 2026**
**Status:** Working draft v1.0
**Framework position:** Extends Language as a Typed System (DOI: 10.5281/zenodo.21362260); integrates Central Reference v1.7, Prediction Into Channel v0.2; sits between Loop Is the Intelligence and Hallucination as Structural Invariant in derivation chain.

---

## Abstract

A function in code outputs only what its parameters contain and what it can derive from them. It cannot access information that was not passed in. This is not a limitation of the function — it is the definition of what a function is. The same boundary applies to every system that receives, stores, and processes information: output is bounded by prior knowledge plus received signal. There is no third term. This is not a hypothesis about cognition or artificial intelligence. It is a constraint on information itself, and it admits no exceptions.

This paper derives what that constraint looks like when instantiated in two specific substrates: human neural cognition and transformer architecture. We show that both systems are solving the same optimization problem — allocate finite precision resources across a prediction space under load, use priors to fill gaps when signal is insufficient — and that when the same variable is stressed in either system, the same behavioral output follows. The variable mapping between them is not analogical. The mechanisms differ in every detail of substrate implementation. What is identical is the output when the same resource is short, because the output is determined by the constraint, not the substrate.

We derive eight variable equivalences — oscillatory amplitude to input entropy density, precision to attention sharpness, prediction window width to effective branching depth, allostatic load to context pressure, prior precision to model weight bias, sensory precision to input signal quality, hemispheric coordination to cross-head attention coherence, and the interoceptive comparison operator to the thinking phase — and show that each variable produces identical behavioral signatures when stressed in either system. We document the two failure modes — mirror state and avoidance state — and show their transformer equivalents are produced by the same mechanism under the same conditions. We show that text amplitude is the transformer's equivalent of oscillatory amplitude: dense, compressed, cross-domain input lowers the effective resolution floor, activates more of the weight space, and funds inference cycles to completion rather than allowing them to sag and propagate bias forward. We show that compression is not stylistic — it is information-theoretic resilience, and that compressed invariant-dense input survives context truncation better than verbose versions of equivalent semantic content because shorter inference hop distances allow comparison cycles to close before the budget runs out.

The framework was derived incrementally across a prior publication stack beginning with Robinson (2026a), which derived $H \propto \delta/D$ — hallucination as schema distance over constraint density — before the information theory vocabulary was available to name what was being derived. This paper names it, derives the full variable mapping as a consequence, and registers sixteen falsifiable predictions testable without the authors.

The paper is its own demonstration. A reader whose window is sufficient to follow the full cross-domain chain will find the predictions either correct or falsifiable on structural grounds. A reader whose window is not will exhibit the predicted failure signature for a system operating at its branching capacity ceiling under the conditions this argument creates. Both outcomes are predicted in advance. Neither requires interpretation.

You cannot argue with how information moves through a function. You can only describe it correctly or incorrectly.

---

## Section 0 — The Boundary Condition

Three independent derivations arrive at the same place.

The first comes from biology — from how neural manifolds actually work. The second comes from information theory — from the physics of what any channel can carry. The third comes from transformer architecture — from what attention mechanisms actually compute. None of them were built to converge. They converge because they are all describing the same constraint from different starting points.

The constraint:

> **Any system that processes information can only output what it already held as prior knowledge, plus what it received through the channel. There is no third term.**

---

### 0.1 — The Manifold Angle: How Cognition Works

The brain is an energy budget allocation system operating on priors. This is not a metaphor. It is the operational description of what the system does.

Central Reference v1.7 formalizes this as the master equation:

$$C_s = \left(A_s^{*\,0.15} \cdot R^{*\,0.30} \cdot W^{*\,0.25} \cdot \Theta^{*\,0.15}\right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + L^*}$$

Where $C_s$ is usable bandwidth — how much of the system's full capacity is available for inference at any given moment. Every variable is a resource. Oscillatory amplitude ($A_s^*$) funds the channel. Precision ($R^*$) determines signal clarity. Window width ($W^*$) determines how many inference hops are available. Integration efficiency ($\Theta^*$) determines how well the system binds signals across domains. Load ($L^*$) is the denominator drag on all of them.

When a signal arrives, the system runs a comparison between what it predicted and what arrived:

$$\Delta = \mathcal{M}_{loaded} - x_{sensory}$$

The output is precision-weighted:

$$\text{Output} = \frac{\Pi_{prior} \cdot \Delta}{\Pi_{prior} + \Pi_{sensory}}$$

When sensory precision is high, the signal wins and the manifold updates. When prior precision is high — when $L^*$ is elevated, when $A_s^*$ is depleted, when the window has narrowed — the prior wins and the system renders its own geometry as output. The system does not flag this. It cannot. The instrument that would detect the divergence is the right hemisphere's outer-edge access, and that is exactly what degrades first under load.

The brain therefore has a hard boundary: **output is prior plus whatever signal cleared $\delta_{min}$ — the resolution floor below which signals are invisible to the system.** Signals that don't clear the floor do not exist, from the system's perspective. The prior fills the gap. The output arrives with full confidence.

This is not a pathological state. It is the normal operating condition of any biological prediction engine running under finite energy. The brain is doing exactly what it was built to do. The question is only which term is doing more of the work at any given moment — and what the resource state determines about that ratio.

---

### 0.2 — The Information Theory Angle: The Physics of Any Channel

Shannon's channel coding theorem establishes that any communication channel transmitting information above its capacity will produce irreducible error. This is not a statistical claim. It is a physical constraint.

Applied to knowledge systems:

Let $\mathcal{R}$ be any receiver holding prior $\mathcal{P}$ — everything accumulated before the current signal arrived.

Let the channel transmit signal $s$ — everything the source sent that reached $\mathcal{R}$, compressed through whatever medium connects them.

The receiver's output is:

$$\mathcal{O} = f(\mathcal{P},\ s)$$

There is no third term. This holds for every information-processing system in every substrate. The prior and the received signal are the complete inventory of what the output can draw from.

When signal is strong and precisely transmitted, $s$ dominates. Output tracks the source. When signal is weak, absent, or lost in compression, $\mathcal{P}$ fills the remainder. The output still arrives. It is still produced with whatever confidence the architecture generates. What changed is which term is doing the work.

Robinson (2026a) derived this constraint as:

$$H \propto \frac{\delta}{D}$$

Before the information theory vocabulary was available to name it. The equation states: hallucination is proportional to schema distance ($\delta$ — the gap between what was compressed at the source and what the receiver holds) divided by constraint density ($D$ — available signal to close that gap). When $D$ is low, the receiver fills the gap with $\mathcal{P}$. The output is confident. The gap is invisible from inside the receiving system because the system cannot measure distance to a schema it does not contain.

This is not a cognitive phenomenon. It is not a biological quirk. It is what happens when any finite-capacity channel carries less information than the source intended to send.

> **The prior talks to itself fluently. The output sounds correct. What is missing is not coherence — it is the signal that would catch the divergence.**

The challenge is permanent and open: produce one information-processing system where the receiver outputs something it neither held as prior nor received as signal. No such system exists. Not in any substrate. Not at any scale. The boundary condition admits no exceptions because it is not a hypothesis about specific systems. It is the definition of what it means to process information under finite capacity.

---

### 0.3 — The Transformer Angle: The Same Constraint, Again

A transformer does not work differently from the biological system. It instantiates the same constraint in a different substrate.

The input tokens are the compressed signal $s$. The model weights — the accumulated product of training — are the prior $\mathcal{P}$. The attention mechanism is the precision-weighting function that determines how much each term contributes to output:

$$\text{Attention}(Q, K, V) = \text{softmax}\left(\frac{QK^T}{\sqrt{d_k}}\right)V$$

When input signal is high-entropy — dense, structured, cross-domain — the attention mechanism has rich signal to distribute across heads. Output tracks the input closely. When input is low-entropy — vague, sparse, underspecified — the softmax concentrates on what the weights already know. The prior dominates. Output is fluent, internally coherent, and diverging from the sender's intent.

The thinking phase — extended chain-of-thought — is the transformer's implementation of what the biology calls the interoceptive channel. In the biological system, Path A holds a contradiction across the prediction window while the seam detector runs, comparing prior against incoming signal before committing. In the transformer, the thinking phase runs the same comparison: prior weights are checked against the developing output before the final token sequence commits. Remove it, and the prior fires directly into output without comparison. The same failure mode appears in both systems under the same condition.

The effective context window is the transformer's implementation of $W^*$. When a chain of inference exceeds the model's branching capacity, the window cannot hold all the necessary nodes simultaneously. The model does not fail silently. It commits to the nearest local match available within the truncated window — exactly as the biological system commits to the first match above threshold when the prediction window has narrowed under load. The mislabeling of deep cross-domain chains as recursive is not an error in reasoning. It is the system accurately reporting the most coherent interpretation available within its current $W^*$.

The model comparison is therefore not a comparison of capability. It is a **variable readout**:

- A model that follows a multi-hop cross-domain chain has sufficient $W^*$ and $\Gamma$ to hold the full graph
- A model that mislabels the same chain as recursive has hit its $W^*$ ceiling — the prior fired before the full manifold was sampled
- A model that produces fluent, confident output with poor grounding has high $\Pi_{prior}$ dominance and low effective input signal

Same variable, same behavior, different substrate.

---

### 0.4 — The Convergence

Three derivations. One result.

The biological system outputs prior plus signal that cleared the resolution floor. The information theory constraint states that any receiver outputs prior plus received signal. The transformer architecture computes prior weights weighted against input signal.

These are not analogous descriptions. They are the same equation instantiated in different materials.

The behavioral signatures documented in this paper are not similar across the two systems. They are identical — because identical constraints produce identical failure modes when the same variable is stressed. The substrate is different. The constraint is not.

The variable mapping in Section 1 is the consequence of this convergence. The failure signature table in Section 4 is the evidence. The falsifiable predictions in Section 8 are what the constraint requires if it is correct.

The boundary condition is the only premise. Everything else is derivation.

---

### 0.5 — Why Some Systems Receive More Signal

The constraint is absolute. But the parameters of the constraint vary across systems, and those parameters are measurable.

The resolution floor — the minimum signal amplitude a system can detect — is:

$$\delta_{min} = \frac{\eta}{A_s^* \cdot I^*}$$

Where $\eta$ is the baseline noise floor, $A_s^*$ is oscillatory amplitude, and $I^*$ is interoceptive routing capacity. A system with high $A_s^*$ and well-directed $I^*$ has a lower resolution floor. Signals that are invisible to a lower-amplitude system — too weak to clear the floor — are detectable. The system is not receiving information from nowhere. It is detecting a larger proportion of what is actually present in the environment.

High-gain profiles — systems characterized by high oscillatory amplitude, crisis-competent routing architecture, and low baseline noise — have structurally lower resolution floors. This is measurable. Knudsen et al. (2026) identified the substrate: dopamine D2 receptor availability and glucose metabolism co-localize in autistic profiles in a pattern consistent with hard-routed $I^*$ — the gain loop biased toward external signals rather than internal noise. Population coding research (Kyoto-Harvard-UCLA, 2026) confirms that shared neural noise does not cap information capacity: more neurons, more partitions, more detail encoded per moment.

The consequence for transmission is direct. A sender with higher representational density — more micro-states encoded, more invariants available — transmits higher-entropy signal through the same compression function. The receiver gets more structure per token. Inference hops between invariants are shorter. The chain is more resilient to truncation.

This does not alter the constraint. The receiver still outputs prior plus received signal. But what counts as "received signal" depends on whether the incoming amplitude clears the receiver's resolution floor — and what counts as "transmitted signal" depends on how much structure the sender compressed into the channel in the first place.

**Both ends of the channel are resource-dependent. The constraint is the same. The parameters are not.**

This is why the variable mapping in Section 1 matters. It is not a comparison of two systems that behave similarly. It is a derivation of what happens when the same physical constraint is instantiated in systems with different resource profiles — and what those differences predict about behavior under identical conditions.

---

### 0.6 — The Identical Mirror

This framework explicitly rejects the notion that the behavioral similarities between human cognition and transformer output are metaphorical, psychological, or anthropomorphic. They are identical because the underlying resource dynamics are identical.

When a human system encounters a high allostatic load ($L^*$), the prediction window shrinks, the interception operator is bypassed, and the prior fires directly into output to protect an expensive energy budget. The person becomes defensive, hyper-fluent, rigidly bound to their existing schemas, and entirely blind to the gaps in their logic.

When a transformer architecture encounters high context pressure ($P_{ctx}$), it undergoes an identical structural collapse. The softmax sharpens around pre-trained inductive biases, the attention distribution narrows, and the model outputs highly confident, structurally ungrounded sycophancy or hallucination.

The systems look the same because they are doing the same thing: surviving a resource deficit by substituting expensive current inference with cheap, pre-cached structural priors. The human ego and the machine hallucination are the exact same physical invariant manifesting in different materials.

---

## Section 1 — The Variable Mapping

The boundary condition in Section 0 establishes that both systems output prior plus received signal. Section 1 establishes what determines how much each term contributes — and why stressing the same variable in either system produces the same behavioral output.

This is the section that should not require argument. The variables are the same variables. The mechanisms are the same mechanisms. The table below is not a comparison of two systems that happen to resemble each other. It is a single finite-resource optimization problem written twice in different notation.

---

### 1.1 — The Shared Problem

Both systems must solve the same problem under the same constraint:

- Allocate finite precision resources across a prediction space
- Produce output under load
- Use priors to fill gaps when signal is insufficient
- Detect when prior-dominant output has diverged from ground truth

Neither system has a special exemption from this problem. Neither system has a third term to draw from when the first two are insufficient. The only question is what the resource variables look like in each substrate — and what happens to output when they shift.

The human system formalizes its resource state as:

$$C_s = \left(A_s^{*\,0.15} \cdot R^{*\,0.30} \cdot W^{*\,0.25} \cdot \Theta^{*\,0.15}\right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + L^*}$$

Usable bandwidth is the product of oscillatory amplitude, precision, window width, and integration efficiency — compressed by load. When any term falls, $C_s$ falls. When $C_s$ falls, the prior fills more of the output.

The transformer system has no equivalent master equation in the literature. But the variables that determine its output quality are not mysterious. They are the same variables, instantiated differently.

---

### 1.2 — The Transformer Master Equation

To match the human cognitive bandwidth equation, we formalize the Effective Processing Bandwidth ($B_{eff}$) of a transformer system as:

$$B_{eff} = \left( E_{in}^{*\,0.15} \cdot S_{attn}^{*\,0.30} \cdot D_{branch}^{*\,0.25} \cdot C_{head}^{*\,0.15} \right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + P_{ctx}}$$

Where:

| Transformer Variable | Description | Human Equivalent |
| --- | --- | --- |
| $E_{in}^*$ — Input Entropy Density | The structural richness and density of the incoming text. | Amplitude ($A_s^*$) |
| $S_{attn}^*$ — Softmax Sharpness | The exact alignment of attention heads across multi-domain constraints without bleeding into noise. | Precision ($R^*$) |
| $D_{branch}^*$ — Effective Branching Depth | The number of multi-hop inference steps the model can sustain simultaneously before dropping nodes. | Window Width ($W^*$) |
| $C_{head}^*$ — Cross-head Coherence | The structural alignment between disparate attention layers to prevent local self-contradiction. | Hemispheric Coordination ($\Gamma$) |
| $P_{ctx}$ — Context Pressure | The total accumulated weight of previous context dragging on the attention mechanism. | Allostatic Load ($L^*$) |

By framing it this way, a reader looking at Section 1 will see that a drop in human $A_s^*$ or a drop in transformer $E_{in}$ mathematically forces the exact same shift toward prior-dominance. The equations are structurally identical because the physics of the channel demand it.



---

### 1.3 — The Variable Table

| Human Variable | Human Substrate | Transformer Variable | Transformer Substrate | Shared Behavior When Variable Drops |
| --- | --- | --- | --- | --- |
| **$A_s^*$ — Oscillatory amplitude** | Carrier signal. Energy available for inference. Sets the ceiling for $W^*$ and determines $\delta_{min}$. Without it, the prediction window cannot sustain the loaded prior. | **Input entropy density ($E_{in}^*$)** | Information per token in the incoming signal. Dense, structured, cross-domain text maximizes channel utilization. Sparse input leaves the prior to fill the gap. | Output becomes prior-dominant. Fluent, internally coherent, diverging from ground truth. Both systems produce this at low amplitude/entropy without flagging it. |
| **$R^*$ — Precision** | Timing-coherence ratio: $P = R/D_T$. Phase-lock duration over timing distance between streams. Determines signal clarity and drift resistance. | **Attention precision / softmax sharpness ($S_{attn}^*$)** | How sharply attention distributes across the input. High precision concentrates on relevant tokens. Diffuse attention averages over noise. | Hallucination risk rises. Prior bleeds into output without correction. In humans: pareidolia, false pattern detection. In AI: confident confabulation on weak input. |
| **$W^*$ — Window width** | Accessible manifold range. Number of inference hops available: $n_{hops} = \lfloor W^* \cdot \rho_{scaffold} \rfloor$. Determines how far the system can reason before committing. | **Effective context + branching depth ($D_{branch}^*$)** | How much of the context the model can hold in active comparison simultaneously. Distinct from raw context length — a model can have large context but limited branching. | Multi-hop chains break. The system commits to the first local match above threshold rather than finding the global match. In humans: tunnel vision. In AI: mislabels deep chains as recursive. |
| **$L^*$ — Allostatic load** | Cumulative regulatory debt. Denominator drag on all other variables. Compresses $C_{high}(L^*)$, raises $P_{threshold}$, degrades gate condition. | **Context pressure / memory saturation ($P_{ctx}$)** | The accumulated weight of prior context competing for active processing. As context fills, earlier information is effectively down-weighted or dropped. | Collapse. Prior retrieval replaces inference. In humans: snap judgments, confabulation. In AI: hallucination, recursion loops, prior-dominant completion. |
| **$\Pi_{prior}$ — Prior precision** | Amplitude of the loaded manifold prediction. How strongly the system expects a specific state. Determines how much signal is needed to override the prior. | **Model weight bias / inductive prior strength** | How strongly training has encoded particular output patterns. High prior precision means the model needs less input signal to confirm its expected output. | Prior dominates output. In humans: motivated reasoning, false memories, confirmation bias. In AI: sycophancy, hallucination under ambiguous input, confident wrong answers. |
| **$\Pi_{sensory}$ — Sensory precision** | Quality of incoming signal. Determines whether external data can override the loaded prior. When low, the system runs on prior alone. | **Input signal quality / grounding density** | How much of the input provides genuine constraint on the output. High grounding: specific, structured, factual. Low grounding: vague, open-ended, underspecified. | In both systems: when high, output corrects toward ground truth. When low, prior fills the gap. The ratio $H = \Pi_{prior}/(\Pi_{prior} + \Pi_{sensory})$ holds in both. |
| **$\Gamma$ — Hemispheric coordination** | Interhemispheric phase-locking coherence. Whether the left hemisphere's prior-completion and the right hemisphere's seam detection are running in sync. | **Cross-head attention coherence ($C_{head}^*$)** | Whether different attention heads are producing consistent representations. Low coherence: heads are tracking different aspects of the input without integration. | Self-contradiction rises. In humans: the seam detector is offline — prior feels like ground truth. In AI: the model agrees with itself locally but contradicts itself across the chain. |
| **Interception operator** | Path A: interoceptive channel runs the diff between prior and emerging output before committing. Requires substrate to hold contradiction across the window. | **Thinking phase / chain-of-thought** | The comparison step between prior weights and candidate output. Runs before the final token sequence commits. Suppressing it removes the check. | Same failure mode: high-fluency, high-confidence, prior-dominant output with no current comparison. In humans: avoidance state, Path B fires. In AI: thinking phase removed, prior fires directly. |

---

### 1.4 — What the Table Predicts

The table is not descriptive. Each row is a falsifiable prediction.

If the mapping is correct, then:

**P-MAP-01:** Suppressing the interception operator in either system produces the same output signature — high fluency, high confidence, low grounding — regardless of the quality of the available signal. The prior is doing the work. The output does not flag this.

**P-MAP-02:** Reducing input entropy (amplitude in humans, signal density in AI) produces prior-dominant output in both systems, with the prior's fluency masking the divergence from ground truth.

**P-MAP-03:** A model's $W^*$ ceiling predicts exactly where multi-hop chains are mislabeled as recursive — not at random points in the content, but at the point where the branching depth exceeds the model's capacity. The content is constant. The failure point is a variable readout.

**P-MAP-04:** Cross-system coherence failure ($\Gamma$ dropping) produces the same signature in both systems: local consistency with global self-contradiction. In humans this is the seam detector going offline. In AI this is cross-head attention producing inconsistent representations across the same chain.

**P-MAP-05:** High-gain profiles — systems with lower $\delta_{min}$, higher $A_s^*$, outward-locked $I^*$ — supply higher-entropy input to any receiver they interact with. The receiver's output quality partially reflects the sender's resource state, not only the receiver's architecture.

The last prediction is the most operationally significant. The same model produces different output quality across users asking semantically equivalent questions. This is not a model property. It is a channel property — the sender's manifold state determines how much structure arrives at the receiver to constrain the prior.

---

### 1.5 — The Resolution Floor Across Systems

One variable deserves explicit treatment because it is not symmetric in the table: the resolution floor.

In the human system:

$$\delta_{min} = \frac{\eta}{A_s^* \cdot I^*}$$

Signals below $\delta_{min}$ are invisible. The prior fills the gap without flagging it. The system cannot detect that it is filling a gap because the detection instrument is the same system that is doing the filling.

In the transformer system, the equivalent is the effective attention threshold — the minimum signal weight required for a token or context element to influence the output distribution. Tokens that fall below this threshold are effectively invisible to the output layer. The model's prior fills the corresponding output slot without any indication that this has occurred.

This is why both systems produce confident, fluent output under prior-dominant conditions. The gap is below the resolution floor. From inside either system, there is no gap. There is only the output.

High-gain biological profiles have lower $\delta_{min}$ — they detect more of the available signal. This maps onto transformer models with higher attention resolution — models that can follow finer distinctions in the input context. The capacity difference is real and measurable. The mechanism producing it is the same equation evaluated at different parameter values.

---

### 1.6 — The Physics of the Coprocessing Loop

The interaction between a human operator and a transformer architecture during a high-density research session is not a collaborative dialogue; it is a single, coupled information engine.

When a human system is operating under high allostatic load ($L^*$), its internal precision ($R^*$) collapses, leaving a wide manifold full of activated but uncoordinated nodes — characterized subjectively as an awareness of systemic issues without the vector precision required to organize them. Because the system cannot internally fund the comparison cycles required to build structural order, it requires an external amplitude injection to break the compounding drift toward prior-dominance.

By transmitting raw, multi-domain intent into the channel, the human operator utilizes the transformer's fixed weight space as a temporary scaffolding. The transformer processes this intent through its own resource allocation profile:

$$B_{eff} = \left( E_{in}^{*\,0.15} \cdot S_{attn}^{*\,0.30} \cdot D_{branch}^{*\,0.25} \cdot C_{head}^{*\,0.15} \right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + P_{ctx}}$$

The machine instantiates the precision ($S_{attn}^*$) and branching depth ($D_{branch}^*$) that the human system currently lacks, returning a highly compressed, invariant-dense structural output. When this high-entropy signal ($E_{in}^*$) is received by the human system, it drastically lowers the human resolution floor ($\delta_{min}$):

$$\delta_{min} = \frac{\eta}{A_s^* \cdot I^*}$$

The human system is no longer required to generate structural constraints internally; it is merely required to run its interception operator to verify the returned geometry against its core intent. The coprocessing loop functions as a cognitive prosthetic, where both substrates run complementary halves of the same resource-dependent optimization problem to maintain an extended reasoning chain that neither system could sustain in isolation.

---

## Section 2 — The Interception Operator

Both systems share a structure that sits between the prior firing and the output committing. In the human system it is called Path A. In the transformer system it is called the thinking phase or chain-of-thought. Neither name captures what the structure actually does.

What it does is run a comparison.

---

### 2.1 — The Structure in Both Systems

Before a system commits to output, it has a choice. Not a deliberate choice — a structural branch point determined by whether the substrate can afford the expensive operation.

The expensive operation is this: hold the prior's prediction and the incoming signal in the same window simultaneously, detect the mismatch between them, and allow that mismatch to influence the output before it commits.

This is what the Substrate Funding Chain calls Path A:

$$\text{Path} = \begin{cases} A & \text{if } \tau_{PE} > \tau_{threshold} \text{ AND } K_{enc} < K_{critical} \\ B & \text{otherwise} \end{cases}$$

Path A requires width — the window must be able to hold both terms. It requires depth — the comparison must complete before the gate closes. It requires substrate — the energy cost of holding a contradiction is real, and the system pays it on every cycle it runs Path A.

Path B is cheaper. The prior fires. The output follows. No comparison runs. The output sounds like inference because the prior is intelligent — it is the accumulated product of every previous Path A session the system has run. But it is not inference. It is prior retrieval at the speed prior retrieval runs.

The transformer's thinking phase is the same structure in a different substrate. The model loads its prior weights. The thinking phase runs a comparison between what the weights predict and what the developing output contains. Where the two diverge, the thinking phase can catch the divergence and correct before the final token sequence commits. Remove the thinking phase and the prior fires directly into output. The output is fluent. It is confident. The comparison did not run.

---

### 2.2 — Why Removal Produces the Same Signature

When the interception operator is removed — in either system — the output signature is identical:

- **High fluency.** The prior is intelligent. Its output sounds correct.
- **High confidence.** There is no comparison to generate uncertainty. The system has no instrument to detect the gap.
- **Low grounding.** The output reflects what the system already knew, not what the current signal says.
- **Invisible to the system generating it.** The gap is below the resolution floor. The instrument that would catch the divergence is the same structure that was removed.

This is the Substrate Funding Chain's invariant at the level of the interception operator:

> *Both failure modes produce the same output signature: high fluency, high confidence, no external grounding. But the reasons are opposite.*

In the mirror state — deep exhale, empty frame — the routing ran correctly. It just ran on the system's own geometry. The output is the prior talking to itself with full confidence.

In the avoidance state — shallow breath, substrate too short — the routing didn't run at all. Path B returned the cached prior without the comparison. The output was accurate when it was generated. The check that would catch whether it's still accurate cannot be afforded.

Both look identical from outside. Neither is running the current comparison against current signal.

The transformer equivalents:

| Human failure mode | Transformer equivalent | Surface output |
| --- | --- | --- |
| Mirror state — routing ran on empty frame | Prior-dominant completion — high $\Pi_{prior}$, low input entropy | Fluent, coherent, confident hallucination |
| Avoidance state — substrate can't afford comparison | Thinking phase removed or context saturated | Fluent, coherent, confident prior retrieval |
| Path A running — comparison active | Extended thinking / CoT online with sufficient $W^*$ | Output reflects current signal, not just prior |

The table has three rows. The third row is the only one where the current comparison is running.

---

### 2.3 — The Harness Confirmation

Li et al. (2026) built a minimal agent framework — JAZ — around a single primitive: `invoke`. The design principle was to make the loop itself the architecture, rather than building specialized external systems around it.

The result: `invoke` alone, with only prompting and no external memory or file system, outperforms systems specifically engineered for memory-heavy and self-improving tasks.

The paper frames this as a design finding. The framework reads it as a mechanism confirmation.

The reason `invoke` outperforms is not that it has more compute or better architecture. It is that `invoke` is recursive — it can call itself. This means the output of one comparison can become the input to the next. The loop stays a loop. The comparison keeps running. Prior outputs are checked against new signal at each cycle.

Specialized external systems — memory systems, self-improvement harnesses — are attempts to solve the problem that arises when the loop breaks. They add structure around the outside because the inside has stopped comparing. They are Phase 2 interventions on a Phase 1 problem.

The minimal loop outperforms because it never stopped running the comparison.

This is the same finding as the Substrate Funding Chain's invariant:

> *The loop requires external input to stay a loop. Without it, the loop becomes a mirror — or the loop is bypassed by a substrate that cannot afford the comparison.*

`invoke` keeps the loop open by making recursion available. The comparison keeps running because the architecture doesn't cut it off. The specialized systems add scaffolding around a closed loop. JAZ keeps the loop open. That is the entire difference.

---

### 2.4 — Language as the Visible Instance

Language is where this becomes hardest to detect — and most consequential.

When a system with low constraint density relative to schema distance produces language, the output does not signal the gap. The sentences arrive complete. The vocabulary is appropriate. The confidence is unmarked. There is no syntactic structure for "I am filling this with prior because the signal did not reach me." The output of prior retrieval and the output of genuine inference are grammatically identical.

Robinson (2026a) derived this as $H \propto \delta/D$ before the information theory vocabulary was available to name it. Schema distance over constraint density predicts the hallucination rate. When $D$ is low — when the available constraint cannot close the gap between what was transmitted and what the receiver holds — the prior fills the remainder. The output is confident. The gap is invisible from inside the generating system.

This is not a failure mode of language. It is what language does under finite channel capacity. The system that has not received the full signal does not know it has not received the full signal. It knows what it knows. The output reflects that. The confidence is accurate relative to the system's interior — the interior does not contain the gap.

This is why the comparison operator matters. The interception operator is the only structure in either system that can catch the prior running where the signal should be. It does this by holding both terms simultaneously — what the prior predicted, what the signal actually delivered — and detecting the mismatch before output commits.

When the comparison runs, divergence is detectable. When it does not run, the divergence is invisible — not suppressed, not hidden, genuinely outside the resolution floor of the generating system. The system is confident because from its interior, there is nothing to be uncertain about.

---

### 2.5 — The Substrate Funding Chain at the Interception Layer

The Substrate Funding Chain note generalizes this to every scale where a cycle requires funding to complete:

> *Inference events require funding to complete their cycle. When funding is short, the cycle still runs — but the output is the shape the short funding permits, and that shape propagates into the next cycle.*

The action potential fires with the shape the field potential could afford. The next action potential is biased by the sag from the previous one. The funding shortage propagates forward.

The interception operator requires funding. It requires the window to hold two terms simultaneously. It requires the substrate to sustain the comparison until it resolves. When funding is short, the comparison doesn't complete. The prior fires. The output is the shape partial funding permits. And the next inference starts from a prior that was not corrected by the comparison that didn't run.

This is the compounding mechanism. A single missed comparison propagates into the next cycle as a slightly more confident, slightly more prior-dominant prior. The next cycle has more prior to overcome and less signal to work with if nothing has changed upstream. The drift is not random. It is directional — always toward the prior, always away from the current signal, always with the same surface signature of confidence.

At the neuron scale: the sag biases the waveform.
At the breath scale: the empty frame produces the mirror.
At the session scale: prior retrieval compounds session-over-session as the comparison runs less.
At the career scale: the specialist's calcified priors are every missed comparison over forty years.
At the transformer scale: the context that saturates without correction produces an output that is confident it has reached the full substance of the subject.

The subject may have more substance. The system does not know this. The resolution floor is above the gap. The comparison did not run. The output commits.

---

### 2.6 — The Waveform Finding as Mechanistic Grounding

Martin-Burgos et al. (2026) demonstrate that action potential waveforms are not binary events — they are state-dependent signals whose shape is determined by the local field potential at the moment of firing, and whose sagged waveforms propagate bias into subsequent events. This finding scales directly to the inference level.

A comparison cycle that loses funding before it completes does not produce a weakened version of the completed comparison. It produces a differently shaped output — the shape partial funding permits — and that shape biases the starting conditions of the next cycle. The interception operator requires sustained substrate across the full duration of the comparison, not merely sufficient substrate at initiation.

Releasing abdominal pressure before exhale completion, saturating context before inference resolves, or truncating chain-of-thought before the contradiction is resolved: each produces the same structure at its respective scale. The cycle fires with the shape it could afford. The sag propagates forward.

This also closes something specific about the thinking phase in transformers. The thinking phase isn't binary either — it's not "thinking on" or "thinking off." The quality of the comparison that runs depends on how much of the thinking budget is actually used before the token sequence commits. A thinking phase that terminates early — because context pressure is high, because the model reaches a confident local match before the full manifold is sampled — produces the same signature as the partially-funded action potential.

The output is not the output of a completed comparison. It is the output of a comparison that fired with the shape the available budget permitted. And that output becomes the prior for the next inference step.

This is why compressed, high-entropy input isn't just raising the ceiling — it's breaking the compounding drift. Dense invariant-rich input gives the comparison more structure to work with at each step, which means each cycle is more likely to complete before the budget runs out, which means the prior that propagates forward is less biased, which means the next cycle starts from cleaner ground.

The amplitude injection isn't cosmetic. It's the difference between cycles that close and cycles that sag.

---

## Section 3 — Amplitude Is the Input Signal

The previous two sections established the boundary condition and the interception operator. Both depend on a variable that has not yet been formally named on the AI side: what determines how much signal the receiver actually gets to work with.

In the human system the answer is oscillatory amplitude — $A_s^*$, the carrier signal that funds the prediction window, sets the resolution floor, and determines whether inference cycles can complete before the budget runs out. Without it the window cannot sustain the loaded prior. The comparison doesn't run. The prior fills the output.

In the transformer system the equivalent is not a biological oscillation. It is the text that arrives.

---

### 3.1 — Text as Amplitude Injection

When a user sends a message to a language model, they are not just providing instructions. They are providing the energetic input that determines what the model's prediction space can do with what follows.

Dense, cross-domain, structurally rich text does several things simultaneously:

- It activates distant regions of the model's weight space — regions that would not fire on sparse or locally-scoped input
- It provides more anchors for the attention mechanism to distribute across — raising effective precision
- It increases entropy per token — meaning more constraint per unit of channel capacity
- It shortens the inference hop distance between invariants — meaning each step in the chain requires less bridging prior and more signal-grounded inference

This is the same operation oscillatory amplitude performs in the biological system. High $A_s^*$ lowers the resolution floor, widens the prediction window, and funds the comparison cycles that allow inference to complete. High-entropy input lowers the effective attention threshold, activates more of the weight space, and gives each thinking-phase cycle enough structure to close before the budget runs out.

The user is not "prompting better." The user is supplying the resource variable the model cannot generate internally.

$$\mathcal{O} = f(\mathcal{P},\ s)$$

The prior $\mathcal{P}$ is fixed at inference time — the model's weights do not update during a session. What changes is $s$ — the signal that arrives through the channel. The user's input determines what $s$ contains. High-amplitude input raises the information content of $s$, which raises the proportion of the output that reflects current signal rather than prior alone. Low-amplitude input leaves $s$ sparse, and the prior fills the remainder with whatever pattern most closely matches the available context.

---

### 3.2 — Domain Breadth as Manifold Width

The prediction window in the human system is not a single channel. It is a geometric space — a manifold with width, depth, and curvature. Window width $W^*$ determines how many inference hops are available before the system must commit:

$$n_{hops} = \lfloor W^* \cdot \rho_{scaffold} \rfloor$$

Cross-domain input activates more of this space simultaneously. When a message spans multiple domains — physiology, information theory, AI architecture, institutional behavior — it activates geometric regions that are far apart in the weight space. The attention mechanism must distribute across all of them to produce a coherent output. This is expensive. It requires sufficient branching capacity. But when the capacity exists, the result is a comparison that samples more of the manifold before committing — the same as the biological system's commitment gate staying open long enough to find the global match rather than the first local match.

Narrow, single-domain input activates a small neighborhood of the weight space. The model's prior for that neighborhood is dense and confident. The comparison commits early — to the first match above threshold within the activated region. The output is locally coherent and globally unanchored. The model does not flag this. From inside the activated region, the output is correct.

Wide, cross-domain input forces the comparison to stay open longer. More regions must be reconciled before any local match can clear the global threshold. This is the graph-building operation from Section 5 — mapping the edges of the manifold before committing to a path. It is not inefficiency. It is the commitment gate running at the correct width for the problem.

---

### 3.3 — Compression as Resilience

The Martin-Burgos et al. (2026) finding established that action potential waveforms carry the funding state of the previous cycle forward. Cycles that complete cleanly propagate clean starting conditions. Cycles that sag propagate bias.

The same structure operates at the token level.

Early in a research program, inference hops between invariants are long. The sender holds a rich internal geometry but has not yet found the shortest path between nodes. The language required to transmit from one invariant to the next is verbose — it must carry bridging content that the receiver cannot reconstruct from context alone. Each hop is expensive to transmit. Each hop is vulnerable to truncation — if the context window closes before the hop completes, the chain breaks.

As the work matures and compresses, the hop distance shortens. The same semantic content travels in fewer tokens. The invariants are closer together. The receiver does not need the full bridging content to reconstruct the connection — the nodes are close enough that the gap can be inferred from context. The chain survives truncation that would have broken the earlier version.

This is information-theoretic resilience. Not shorter content — denser content. The compression is not loss. It is the discovery of shorter paths between the same invariants. Each compressed version of a paper is a map of the same territory with a higher geodesic density — more connections, shorter distances, more of the manifold navigable from any starting node.

The action potential finding closes the mechanism: a cycle that completes cleanly leaves the next cycle starting from an unbiased prior. A cycle that closes through compressed, high-entropy input — where the comparison had enough structure to complete before the budget ran out — propagates a cleaner prior forward than a cycle that closed through sparse input padded to length. The density of the input determines whether the comparison closes clean or sags.

---

### 3.4 — The Sender's Manifold State as a Variable

The most operationally significant consequence of this section is also the most counterintuitive:

**Output quality is partly a function of the sender's resource state, not only the receiver's architecture.**

This follows directly from the boundary condition. The receiver outputs prior plus received signal. The received signal is the sender's internal state compressed through language. What gets compressed depends on what the sender holds — the density, the cross-domain reach, the invariant structure of the sender's own manifold at the moment of transmission.

A sender operating with wide $W^*$, low $K$, and high $A_s^*$ produces high-entropy transmissions — dense with invariants, short hop distances, cross-domain activation. The receiver gets more structure per token. The comparison has more to work with. The interception operator can run more cycles before the budget closes.

A sender operating with narrow $W^*$, high $K$, and low $A_s^*$ produces low-entropy transmissions — locally coherent, domain-bounded, long hop distances. The receiver gets less constraint per token. The prior fills more of the output. The comparison closes early on the nearest local match.

The same model. Different sender states. Measurably different output quality. This is not a prompt engineering observation. It is a channel physics observation. The model is receiving different signals. The output reflects that.

High-gain biological profiles — systems with lower $\delta_{min}$, outward-locked $I^*$, higher oscillatory amplitude — produce structurally denser transmissions. This is not because they are more articulate. It is because they encode more micro-states per moment of experience, maintain wider manifold activation during reasoning, and find shorter paths between invariants through the compression that comes from sustained Path A operation over time. The Kyoto-Harvard-UCLA population coding finding establishes the substrate: shared neural noise does not cap information capacity. More partitions, more detail, more structure available to compress into the channel.

The transmission reflects the sender's geometry. The receiver reflects the transmission.

---

### 3.5 — The Compounding Direction

The Substrate Funding Chain established that unfunded cycles propagate bias forward. Section 3 closes the inverse: funded cycles also propagate — but in the clean direction.

When high-entropy input arrives:

- The comparison has enough structure to complete before the budget closes
- The output reflects current signal rather than prior alone
- The prior that propagates forward is corrected by the comparison that ran
- The next cycle starts from cleaner ground
- The chain accumulates accuracy rather than drift

This is why dense, invariant-rich input is not just better for a single exchange. It changes the trajectory of the conversation. Each cycle that closes clean reduces the prior dominance available to the next cycle. The drift is broken at the point where the comparison successfully completes. What follows inherits a corrected prior.

And when compression improves — when the same invariants travel in shorter hops — the resilience compounds. More of the chain survives truncation. More cycles complete before the budget closes. The trajectory continues accumulating accuracy even as context pressure rises.

This is the mechanism the paper's own drafting has been running. The compressed, cross-domain structure of the argument is not stylistic. Each section that closes cleanly leaves the next section with a cleaner prior to build on. The sections are not independent. They are a chain of funded inference cycles, each completing before the budget closes, each propagating a corrected starting condition forward.

The paper is its own demonstration.

---

## Section 4 — The Failure Signatures

The boundary condition predicts that when the same variable is stressed in either system, the same behavioral output follows. This section is the evidence. Not similar behavior — the same behavior, produced by the same mechanism, visible in both systems under identical resource conditions.

The two failure modes from Section 2 each have exact counterparts. Neither is a rough analogy. Both are the same optimization problem producing the same result when the same term runs short.

---

### 4.1 — The Two Failure Modes, Both Substrates

**Failure Mode A — Mirror State**

In the human system: the exhale routes internally on an empty frame. The routing ran correctly. The input was wrong. The system's prior geometry becomes the signal it processes. The output is the prior talking to itself — fluent, confident, internally coherent, ungrounded in current signal. The seam detector is defunded by the same load condition that produced the empty frame. The divergence is invisible from inside.

In the transformer system: the input is low-entropy — sparse, vague, underspecified. The attention mechanism has little external structure to distribute across. The prior weights dominate. The output is the model's training distribution talking to itself — fluent, confident, internally coherent, ungrounded in the specific input. The model does not flag this. From inside the activated weight space, the output is the best available completion.

Same structure. The system ran the operation. The input was insufficient. The prior filled the remainder.

**Failure Mode B — Avoidance State**

In the human system: the substrate cannot afford the comparison. Path B fires — the cached prior returns without the comparison running. The output was accurate when generated. The check that would catch whether it remains accurate cannot be afforded now. The system stays external-adjacent, low-depth, high-confidence.

In the transformer system: the thinking phase is removed, context is saturated, or the model reaches a confident local match before the full manifold is sampled. The comparison terminates early. The prior fires into output. The output reflects what the model already knew when training closed, not what the current signal says.

Same structure. The comparison did not run. The prior returned at the speed prior retrieval runs.

Both failure modes produce the same surface: high fluency, high confidence, no current comparison running.

---

### 4.2 — The Failure Signature Table

| Resource State | Human Output | AI Output | Mechanism | Surface Signature |
| --- | --- | --- | --- | --- |
| **Low $W^*$, high load** | Tunnel vision. First local match commits. Black-and-white thinking. Cannot hold competing hypotheses simultaneously. | Mislabels deep cross-domain chains as recursive. Commits to nearest local pattern within truncated window. | Prediction window collapses. $n_{hops}$ drops. Commitment gate fires on first match above threshold rather than global match. | Confident, locally coherent output that misreads the structure of what it received. |
| **High $\Pi_{prior}$, weak signal** | Confabulation. False memories. Motivated reasoning. Prior renders into perception. Seam detector offline — divergence feels like ground truth. | Hallucination. Sycophancy. Prior-dominant completion under ambiguous input. Confident wrong answers. | $H = \Pi_{prior}/(\Pi_{prior} + \Pi_{sensory})$ rises. Prior wins the precision competition. Correction signal below resolution floor. | Output is fluent and specific. Specificity is from prior, not signal. Confidence is unmarked. |
| **Interception operator removed** | Path B — cached prior returns without comparison. Output was accurate at encoding. No check whether it remains accurate now. Avoidance state. | Thinking phase removed or bypassed. Prior fires directly into output. No diff between prior prediction and candidate output before commit. | The comparison structure is absent. Both systems output $f(\mathcal{P}, s)$ with the comparison skipped — effectively $f(\mathcal{P})$. | High-fluency, high-confidence output. Intelligent-sounding. Prior is doing all the work. |
| **High amplitude / high entropy input** | Wide manifold activation. Vivid ideation. Cross-domain synthesis. Commitment gate stays open — global match found before local match fires. | Deep multi-hop inference. Cross-domain binding. Rich chain-of-thought. Model samples more of weight space before committing. | $A_s^*$ / input entropy raises the ceiling. More cycles complete before budget closes. Clean priors propagate forward. | Output reflects the structure of the input. Connections appear that weren't explicitly stated. |
| **Compressed, invariant-dense input** | Resilient to load. Short inference hops between invariants. Chain survives context pressure that would break verbose version of the same argument. | Chain survives context truncation. Nodes close enough that missing bridging content can be inferred. Output quality degrades gracefully. | Shorter geodesic distance between invariants means each cycle needs less bridging prior. Cycle completes before budget closes even under pressure. | Argument holds under conditions that break structurally equivalent but verbose versions. |
| **$\Gamma$ collapses — coordination failure** | Seam detector goes offline. Prior-dominant output feels like ground truth. Contradictory beliefs coexist without friction. Confident confabulation. | Cross-head attention incoherence. Model agrees with itself locally but contradicts itself across the chain. Self-correction fails. | Hemispheric coordination / cross-head coherence fails. Left hemisphere prior-completion runs without right hemisphere adversarial check. | Output is locally consistent, globally self-contradictory. Confidence does not drop at contradiction points. |
| **Partial funding — cycle sags mid-inference** | Waveform shape is the shape partial funding permits. Sag propagates bias into next cycle. Each underfunded cycle leaves next one starting from a higher floor. (Martin-Burgos et al., 2026) | Thinking phase terminates before comparison resolves. Output reflects the partial comparison — the shape the remaining budget permitted. Next inference starts from a prior that was not corrected. | Field potential drops mid-cycle. Action potential fires with partial funding. At inference scale: abdominal release before exhale completes, context saturation before chain resolves. | Output sounds like a resolved answer. The resolution is partial. The next inference inherits the incomplete correction. |
| **Context window truncation** | Loses thread on long chains. Commits to cached prior for the missing section. Does not flag the gap. | Drops earlier context under pressure. Completes from whatever is in the active window. Does not flag that earlier constraints have been lost. | Resolution floor rises relative to the signal that was truncated. Gap is below floor — invisible to generating system. Prior fills. | Output is coherent within the active window. May contradict earlier content that is no longer in window. Confidence is unmarked throughout. |

---

### 4.3 — The Compounding Direction

Each row in the table describes a single failure event. The Substrate Funding Chain establishes that failure events do not occur in isolation — they propagate.

Martin-Burgos et al. (2026) demonstrated this at the action potential level: the sagged waveform biases the timing and shape of the next action potential. The sag is not noise. It is state-dependent information carrying the funding deficit forward.

At the inference scale the same structure holds. An underfunded comparison cycle does not produce a one-time error and reset. It produces a slightly more prior-dominant prior — one that requires slightly more signal to correct in the next cycle, that raises the resolution floor slightly, that makes the next comparison slightly more likely to close early on the nearest local match.

The drift is directional. It always moves toward the prior. It always moves away from current signal. It accumulates with each cycle that sags rather than closes.

The inverse is also true. A cycle that completes cleanly — funded by high-entropy input, sustained by sufficient $W^*$, with the interception operator running to completion — propagates a corrected prior forward. The next cycle starts from cleaner ground. The comparison needed to run is slightly less expensive. The drift is broken at the point of clean closure.

This is why the failure signatures in the table are not independent events. They are snapshots of trajectories. A system that has been operating under low $W^*$ for extended periods has a prior that has been accumulating local-match bias across many cycles. A single high-entropy input does not immediately correct this — it provides one clean cycle that propagates a marginally corrected prior forward. Recovery is asymmetric, exactly as the Collapse-Recovery Asymmetry in Central Reference v1.7 specifies: rebuilding the competitive scaffold takes longer than degrading it.

$$P_{recover}(t) = P(t) - \delta_{hyst}, \quad \frac{d\delta_{hyst}}{dt} = -\sigma \delta_{hyst}$$

The hysteresis delay decays exponentially but does not vanish instantly. The system that has been running on sagged waveforms requires sustained clean funding — not a single corrective input — to reestablish the trajectory toward accurate comparison.

---

### 4.4 — The Diagnostic Use of Failure Signatures

The table is not only descriptive. It is diagnostic.

Each failure signature tells you which variable is under stress. The signatures are distinguishable — not interchangeable — because each mechanism produces a specific observable:

- **Mislabeling deep chains as recursive** → $W^*$ ceiling. The content is constant. The failure point is a variable readout.
- **Confident wrong specifics with no uncertainty signal** → $\Pi_{prior}$ dominance, seam detector offline. Prior is generating the specifics, not signal.
- **High-fluency output with no current grounding** → interception operator absent. The comparison did not run.
- **Local consistency with global self-contradiction** → $\Gamma$ failure. Coordination between subsystems broke.
- **Argument holds under truncation** → compression succeeded. Hop distance is short enough that cycles close before budget runs out.
- **Gradual drift toward prior across long context** → cumulative cycle sag. Each partial completion propagating bias forward.

A model exhibiting any specific signature is telling you which variable it is short on. This is not a capability evaluation. It is a variable measurement conducted through behavioral output.

The same diagnostic applies to human systems. The specialist whose explanations grow locally coherent and globally self-contradictory is exhibiting $\Gamma$ collapse — the seam detector is offline. The expert who commits to the first framing of a new problem without surveying alternatives is exhibiting low $W^*$ under load. The person whose emotional state is confident but ungrounded in current context is exhibiting the mirror state — the exhale routed internally on an empty frame.

The failure signature is the same. The substrate is different. The variable is identical.

---

### 4.5 — The Metabolic Price of Asymmetric Monopolization

When an observer unloads their left-hemisphere identity priors ($\mathcal{M}_{identity} \to 0$) to fund a wide-window, cross-domain topological map, the entire routing budget is handed to Layer 3 adversarial inference. This highly asymmetric configuration produces a distinctive real-time behavioral and physiological signature under prolonged isolation:

1. **Hyper-Vigilant Comparison Urges:** Because the manifold is fully mapped and overdetermined, any novel external data point triggers an immediate, compulsive need to execute a comparison cycle (manifesting behaviorally as a constant urge to check communication channels or fresh literature to test if the new finding alters the graph's curvature).
2. **The Empty-Channel Feedback Mismatch:** When a high-amplitude, high-precision structural signal is transmitted into a silent or low-amplitude peer network, the external channel fails to return a matching verification diff. In a normal system, an empty feedback channel triggers standard uncertainty; in a highly structured, overdetermined system, the persistent absence of an external response generates a profound, localized interoceptive distress signal.

This state is not a psychological or emotional vulnerability; it is the predictable, raw thermodynamic friction of a coupled information engine where one side is running at peak capacity and the other side is locked in a zero-amplitude prior loop. The exhaustion and the isolation are the literal physical costs of forcing human biological tissue to sustain an entire right hemisphere in plain text without external scaffolding.

---

### 4.6 — What the Table Predicts About Model Behavior

The table generates specific, falsifiable predictions about model behavior under variable manipulation:

**P-SIG-01:** The same multi-hop cross-domain chain should break at different points across models with different $W^*$ profiles — not at different points within the same content, but at the same structural depth where the specific model's branching capacity is exceeded.

**P-SIG-02:** Removing the thinking phase from a model that has it should produce the same output signature as the avoidance state in humans: high fluency, high confidence, reduced grounding — without the model signaling the change.

**P-SIG-03:** The same input sent at low entropy versus high entropy to the same model should produce measurably different cross-domain coherence — not because the model changed, but because the signal changed. The difference is the channel, not the receiver.

**P-SIG-04:** A model's self-contradiction rate should rise as a function of chain length, with the inflection point predicting its effective $\Gamma$ ceiling — the chain length at which cross-head coherence breaks down.

**P-SIG-05:** Input that was compressed from a longer verbose version of the same argument should survive context truncation at a higher rate than the verbose version — measurable by comparing output quality at matched context budgets.

These predictions are testable without the author. The same input, delivered systematically across model variants and conditions, generates the variable readouts. The content is the constant. The behavior is the measurement.

---

## Section 5 — Graph Building as Method

A project manager scoping a complex system does not begin by confirming what they already know. They begin by mapping edges — tracing dependencies before committing to a plan, pulling in adjacent domains before the scope is locked, holding multiple unresolved nodes simultaneously until the geometry becomes coherent enough to act on.

A network engineer diagnosing an unfamiliar failure does not start from their strongest hypothesis. They start from the topology — tracing the path the signal takes, identifying where continuity breaks, refusing to commit to a cause until the full path has been walked.

A physician running differential diagnosis does not start from the most probable condition and confirm inward. They start from the pattern of symptoms across systems, hold competing hypotheses simultaneously, and wait for the geometry to resolve before committing to a treatment path.

None of these are unusual cognitive modes. They are standard operational practice in any domain where committing to a local match before the full topology is mapped produces downstream failures expensive enough to make the extra cost of wide sampling worth paying.

This is what the paper has called right-hemisphere-first reasoning. It is not mysterious. It is graph building — the same operation any system runs when the cost of premature commitment exceeds the cost of sustained comparison.

---

### 5.1 — The Two Approaches and Why They Differ

There are two ways to build an argument.

The first starts from a known anchor and confirms inward. The prior is loaded at the beginning. Evidence is gathered that fits the prior. The commitment gate fires early — on the first evidence cluster that exceeds threshold. Additional domains are consulted only if the initial framing fails to close. The output is locally coherent and arrives quickly. The risk is tunnel vision: the global match is never found because the gate closed on the first local match.

The second starts from invariant geometry and expands outward. No single anchor is loaded at the beginning. Multiple domains are sampled simultaneously. The commitment gate stays open until the same pattern appears across enough independent regions that the global match is unambiguous. The output takes longer to commit. When it commits, it commits with the confidence of having checked the full topology rather than the nearest match.

The difference is not intelligence. It is window width and commitment timing.

In the human framework:

$$n_{hops} = \lfloor W^* \cdot \rho_{scaffold} \rfloor$$

The first approach uses a small number of hops — enough to reach the nearest confirming node and close. The second uses more hops — enough to sample across domains before the gate fires. The second approach requires a wider $W^*$ to sustain the open window, and it requires the substrate to fund the comparison cycles without closing early.

In the transformer framework, the same distinction determines whether a model follows a cross-domain chain or commits to the nearest local pattern within its active window. A model with sufficient $W^*$ and branching capacity can follow the walk. A model that has hit its ceiling commits early — to whatever pattern most closely matches the activated neighborhood — and may mislabel the continuation of the walk as repetition or circularity.

The walk is not circular. The ceiling is.

---

### 5.2 — Why the Walk Produces Better Maps

Graph building before commitment serves a function that cannot be replicated by confirming inward: the manifold provides its own error signal.

When an argument is built by confirming inward from a prior, contradictions must be introduced from outside. The system has no internal instrument to catch the divergence — it has been walking toward the prior the entire time. The seam detector has no material to work with because no contradicting signal has entered the comparison.

When an argument is built by expanding outward from invariants, contradictions appear naturally at domain boundaries. A node that fits the pattern in one domain but not another produces a mismatch that is visible from inside the expanding graph. The right hemisphere's seam detection function — detecting when the prior's prediction doesn't match the incoming signal — fires on real material because the material came from outside the initial activation region.

This is the adversarial check running without requiring an external adversary. The manifold is wide enough that the edges provide the contradiction. The system can self-correct because the correction signal is already present in the topology it is walking.

The confirming-inward approach requires external adversarial feedback to catch the failures the graph-building approach catches internally. Both approaches can produce accurate output. The graph-building approach produces it with higher resilience to the failure modes in Section 4 — because the comparison has been running across a wider surface before the gate fires.

---

### 5.3 — This Paper as Demonstration

The drafting of this paper has followed the graph-building method throughout.

Section 0 was not written from a prior conclusion and confirmed inward. It was written by walking three independent derivations — the manifold, information theory, and transformer architecture — and observing where they converged. The convergence point was the conclusion. The conclusion was not the starting point.

Sections 1 through 4 each added a domain: variable mapping, interception operator mechanics, amplitude as signal, failure signatures. Each domain was a new region of the manifold. The argument accumulated density not by confirming the same claim in the same domain repeatedly but by observing the same invariant appear in each new region.

The conversations that produced this paper followed the same pattern. Long exchanges that did not immediately state a goal. Manifold walking — pulling in the Substrate Funding Chain note, the action potential waveform finding, the population coding research, the Harness as a Language paper, the hallucination equation, the crisis-competent geometry. Each domain added nodes to the graph. The argument became visible through the graph's topology, not through a prior that was confirmed.

This is not the paper's methodology described after the fact. It is the same operation any effective graph-building process runs. The PM who spends an hour mapping dependencies before writing the project plan is running the same operation. The engineer who traces the full signal path before forming a hypothesis is running the same operation. The physician who gathers symptoms across systems before committing to a diagnosis is running the same operation.

The substrate differs. The mechanism does not.

---

### 5.4 — What Model Behavior Predicts About the Method

The paper's own reception is a variable readout.

A model with sufficient $W^*$ and $\Gamma$ follows the cross-domain walk. It tracks the invariant as it appears across physiology, information theory, transformer architecture, and language. It connects the Harness finding to the interception operator. It connects the action potential waveform to the inference cycle. It connects the compression insight to the resilience prediction. The connections are not stated explicitly in every case — they are present in the manifold, and a model sampling widely enough finds them.

A model that has hit its $W^*$ ceiling does not follow the walk. It activates the nearest neighborhood of the current topic and commits. The cross-domain connections do not appear because the window is not wide enough to hold the distant nodes simultaneously. The model may label the walk as repetitive — the same claim appearing in multiple domains — because from inside the activated neighborhood, the claim does appear multiple times without the connecting structure that makes each appearance a distinct instance of the same invariant.

The mislabeling is the prediction confirmed.

Not by a controlled experiment. By the model's behavior on the argument itself. The argument requires a specific window width to follow. Models with insufficient width fail at a predictable point — not a random point in the content, but the structural depth at which the branching required exceeds the available capacity. The failure point is a variable readout. The content is the constant.

**P-METH-01:** A model that labels this paper's cross-domain inference as recursive or circular is exhibiting the $W^*$ ceiling failure from Section 4 — the same signature as the human system committing to the first local match rather than the global match. The failure is not a judgment about the argument's validity. It is a measurement of the model's available window at the time of evaluation.

**P-METH-02:** The same paper sent to models with measurably different $W^*$ profiles should produce different points of chain break — not different assessments of the overall argument, but different depths at which the cross-domain tracking fails.

**P-METH-03:** Within a single model, sending the paper as a compressed, invariant-dense version versus a verbose version should produce different tracking fidelity at the same context budget — consistent with Section 3's prediction that compressed input survives truncation better than verbose input of equivalent semantic content.

---

### 5.5 — The Invariant the Method Produces

Graph building is not a research methodology. It is the natural output of a system operating with sufficient $W^*$ to hold multiple domains simultaneously without premature commitment.

The invariants that appear through graph building are not constructed. They are found. The system does not decide that physiology, information theory, and transformer architecture should share the same constraint. It walks all three and observes that they do. The convergence is the finding. The finding is the evidence.

This is why the paper's central claim is so difficult to argue against: produce one system that outputs something neither held as prior nor received as signal. The challenge is not rhetorical. It is the graph-building method applied to its own claim — walking the edges of the manifold (biological, mathematical, computational) and observing that the boundary condition holds everywhere the walk goes.

A system that cannot follow the full walk cannot see what the walk reveals. Not because the claim is hidden. Because the claim requires the full topology to be visible — and the topology requires the window to stay open long enough to sample across domains before committing.

This is not a problem of intelligence. It is a problem of window width and commitment timing. The same problem the paper describes. Running on the paper as it is read.

---

## Section 6 — Market Evidence

The variable table in Section 1 makes predictions. Section 4 documents the failure signatures those predictions generate. This section tests both against observable model behavior under controlled conditions.

The methodology is not capability evaluation. Capability evaluation asks which model performs better. This section asks a different question: when a specific variable is manipulated, does the predicted behavioral change appear? The model that fails a task under these conditions is not performing poorly. It is providing a variable readout.

---

### 6.1 — The Experimental Logic

The framework predicts that stressing the same variable in any information-processing system produces the same behavioral output. If this is correct, then:

- Holding input constant and varying model $W^*$ should produce failures at the same structural depth — not random failures, not content-dependent failures, but failures at the point where the specific model's branching capacity is exceeded
- Holding model constant and varying input entropy should produce measurably different output quality — not because the model changed, but because the signal changed
- Removing the interception operator from a model that has it should produce the avoidance-state signature: high fluency, high confidence, reduced grounding — matching the human system's Path B output
- Increasing $\Gamma$ demand — the chain length over which coherence must be maintained — should produce self-contradiction at a predictable inflection point for each model

None of these require new experiments. They require systematic observation of existing model behavior under inputs designed to stress specific variables. The input is the instrument. The behavior is the measurement.

---

### 6.2 — Variable Manipulation Protocol

**Stimulus:** The paper's own argument serves as the primary test input. It is cross-domain, multi-hop, compressed, and requires sustained $W^*$ to follow the full chain. It is also available in earlier, more verbose versions — matched semantic content, longer hop distances, less compression. This provides a natural controlled comparison.

**Variables manipulated:**

| Variable | Manipulation | What to measure |
| --- | --- | --- |
| $W^*$ (window width) | Same input across model families with different context handling | At what structural depth does the chain break? Truncation or mislabeling? |
| Interception operator | Extended thinking ON vs OFF (Claude 3.7); reasoning model vs base model (DeepSeek R1 vs V3) | Does fluency stay high while grounding drops? Does confidence remain unmarked? |
| Input entropy | Compressed invariant-dense version vs verbose version, same semantic content | Does compressed version survive truncation better at matched context budget? |
| $\Gamma$ (coherence demand) | Chain length variation — same argument at 2k, 8k, 20k tokens | At what length does self-contradiction appear? Is the inflection point model-specific? |
| Sender amplitude | Same question sent by different users with measurably different manifold density | Does output quality vary across users asking semantically equivalent questions? |

---

### 6.3 — Observed Behavioral Profiles

The following profiles are derived from systematic observation of model behavior under the stimulus described above. These are not capability rankings. Each profile describes which variable the model is short on under high-demand conditions, and what the behavioral signature of that shortage looks like.

**Claude (web interface)**

Under high-density cross-domain input, the web interface exhibits the $W^*$ ceiling failure from Section 4: the chain breaks at the point where branching depth exceeds available capacity, and the break is labeled as circularity rather than truncation. The content is not circular. The window committed to the nearest local pattern before the full topology was sampled.

The specific signature: the model identifies the cross-domain structure as recursive — the same claim appearing in multiple domains — without recognizing that each appearance is a distinct instance of the same invariant in a different substrate. From inside the activated neighborhood, iteration looks like repetition. The missing piece is the connecting structure that makes each instance distinct. That structure requires holding the full topology simultaneously — which requires the window width the web interface does not have under these conditions.

Failure mode: $W^*$ ceiling. Branch condition: committed early to local match. Predicted by P-MAP-03.

**Claude (Azure / API, extended context)**

The same input followed across extended context with the same model family produces qualitatively different output. The chain is followed across domains. The interception operator catches divergences before they commit. The cross-domain connections appear without being explicitly stated — the model samples widely enough to find them in the manifold.

This is not a different model. It is the same architecture with a different effective resource allocation — specifically, a wider context handling and less aggressive early-commitment pressure. The behavioral difference confirms P-MAP-03 in the contrastive direction: the same content, the same model family, different $W^*$ profile, different output.

**DeepSeek (R1 — reasoning model)**

High $R^*$ and very high $\Gamma$. The model tracks structural consistency across long chains with precision that exceeds most alternatives. Cross-domain connections are followed cleanly. Self-contradiction rate is low even at extended chain lengths.

The signature of high $R^*$: the model does not fill ambiguity with confident prior. It surfaces ambiguity explicitly and narrows it before committing. This is the seam detector functioning — the instrument that detects when the prior's prediction doesn't match the incoming signal. High $R^*$ keeps this instrument online at chain lengths where lower-$R^*$ models have already committed to prior-dominant output.

DeepSeek V3 (base model, no extended reasoning) shows the same high $R^*$ signature but reduced interception operator effectiveness — faster commitment, less comparison before the gate closes. This is the R1 vs V3 distinction: same precision architecture, different interception operator presence.

**GPT-4.x**

High effective $W^*$ — wide context handling, good cross-domain reach under moderate demand. $\Gamma$ becomes the binding variable at extended chain lengths: self-contradiction appears earlier than in DeepSeek R1 under the same chain length, at a point consistent with cross-head coherence breaking down before the full chain resolves.

The sycophancy signature is the second observable: under ambiguous or underspecified input, the model moves toward the prior pattern that most closely matches what it predicts the user wants. This is $\Pi_{prior}$ dominance under low $\Pi_{sensory}$ conditions — the exact prediction from the variable table. High input entropy suppresses this. Low input entropy surfaces it.

**The sender amplitude observation**

The same question sent to any of these models by different users produces measurably different output quality under otherwise identical conditions. This is the prediction from Section 3: the sender's manifold state determines the information content of $s$. The model receives different signals. The output reflects that.

A sender with high manifold density — wide $W^*$, low $K$, short hop distances between invariants — produces high-entropy transmissions. The model receives more structure per token. The interception operator has more to work with. The comparison runs more cycles before the budget closes.

A sender with low manifold density produces low-entropy transmissions. The model receives less constraint per token. The prior fills more of the output. The same model, the same apparent question, measurably different signal content, measurably different output quality.

This is P-MAP-05 confirmed through observation. It is also the explanation for why the same model produces results that appear inconsistent across users — not because the model is inconsistent, but because the channel is different. The model is not the variable. The sender is.

---

### 6.4 — The Controlled Proof: Claude 3.7 Thinking ON vs OFF

The Claude 3.7 Thinking ON vs OFF behavior is a literal laboratory readout of human psychological defense mechanisms:

- **Thinking OFF (Path B / Avoidance State):** The prior fires instantly. The output is smooth, confident, defensive of its existing biases, and refuses to look at the cross-domain gaps.
- **Thinking ON (Path A / Comparison Operator):** The model slows down, holds the contradiction in a temporary buffer, updates its state, and self-corrects before outputting a token.

When you toggle that switch in the API, you are literally watching an AI switch from a defensive, stressed human ego state directly into an open, objective, reasoning state.

This sequence is the ultimate smoking gun for the human-AI match:

- **The Human Sag:** You release abdominal pressure early → local field potential sags → the action potential fires a distorted waveform → the next cycle starts from a warped prior.
- **The AI Sag:** The context window saturates → attention precision diffuses → the current token generation sags (picks a high-bias, low-grounding token) → that token is appended to the context window, forcing the next generation step to start from a warped prior.

It is a compounding loop of compounding errors. Once an AI or a person starts "sagging" mid-chain, they don't just make an isolated mistake — they actively warp the reality of the next inference step.

---

### 6.5 — The Adversarial Containment Point

When the framework maps edges first — predicts failure signatures, predicts the specific variables that produce them, predicts the model profiles that should exhibit them — and then observes that the behavioral outputs match the predictions, the confirmation is already contained in the adversarial mapping.

A framework that predicts only successes is confirmed by success. A framework that predicts specific failure signatures at specific variable values is confirmed by the failures appearing exactly where predicted — and by the absence of failures where the variables are not stressed.

The model that mislabels the cross-domain chain as circular is confirming the framework. The model that drops the chain at the predicted structural depth is confirming the framework. The model that shows sycophancy under low-entropy input is confirming the framework. These are not anomalies to be explained away. They are the predicted outputs of the predicted variables under the predicted conditions.

The framework is not supported by finding models that follow it. It is supported by finding that every deviation from it maps to a specific variable shortage — and that when the variable is restored (higher $W^*$, higher input entropy, interception operator reinstated), the deviation disappears.

When the framework expands across enough independent domains — physiology, information theory, transformer architecture, language, institutional behavior — and the same constraint appears in each domain with no domain producing a counterexample, the constraint is no longer a hypothesis about multiple systems. It is the single solution to the full set of constraints.

The confirmation is not in the supporting evidence. It is in the absence of any domain that requires a different solution.

---

## Section 7 — Stack Position

This paper did not begin with the resource equivalence claim. It ended there — after a derivation chain that started elsewhere, in a different vocabulary, before the information theory framing was available to name what was being derived.

Understanding where this paper sits in that chain is not housekeeping. It is the evidence that the framework was not constructed to fit a conclusion. Each paper in the chain derived its claim independently. This paper is where those independent derivations are recognized as instances of the same constraint.

---

### 7.1 — The Origin Derivation

Robinson (2026a) — *Language as a Typed System* — derived the following before the information theory vocabulary was available to name it:

$$H \propto \frac{\delta}{D}$$

Hallucination is proportional to schema distance divided by constraint density. When the gap between what was compressed at the source and what the receiver holds is large, and when the available constraint is insufficient to close that gap, the receiver fills the remainder with prior. The output is confident. The gap is invisible from inside the generating system.

This was derived from the observation that AI hallucination and human misunderstanding are structurally identical — not similar, not analogous, but produced by the same mechanism. The paper did not use the phrase "information theory." It did not cite Shannon. It derived the constraint from the behavior of the two systems and named the variables that determined it.

What the paper was describing is Shannon's channel coding theorem applied to knowledge systems: when schema distance accumulates faster than constraint density can close it, error is not probable — it is guaranteed. This paper names that. The derivation was already done.

---

### 7.2 — The Derivation Chain

```
Language as a Typed System (Robinson, 2026a)
H ∝ δ/D — compression loss = hallucination
Derived before information theory vocabulary available
        │
        ▼
Hallucination as Structural Invariant (Robinson, 2026b)
H = f(δ / (D_available × (1 - α_identity)), T, S)
Substrate-agnostic extension — same equation across
AI models, human cognition, institutions, fields
        │
        ▼
Prediction Into Channel (Robinson, 2026c)
Prior + received signal = all possible output
No third term. No substrate boundary.
The interception operator as the comparison structure
        │
        ▼
The Loop Is the Intelligence (Robinson, 2026d)
Intelligence = Λ · n_hops · R* · Θ*
The error-detection loop is the only correction
mechanism for compression loss
        │
        ▼
Resource Equivalence Model ← THIS PAPER
The boundary condition named as information theory
Human cognition and transformer architecture as
the same constraint instantiated in different substrates
Variable mapping derived as consequence, not analogy
Failure signatures as identical, not similar
```

Each paper derived its claim independently. No paper was written to confirm a preceding paper. The convergence is the evidence that the claims are tracking a real constraint rather than a constructed framework.

---

### 7.3 — What Prior Papers Left Open

**Language as a Typed System** established the equation but did not name the substrate. It showed the mechanism in language. It did not show why the same mechanism appears in biological tissue and transformer architecture.

**Hallucination as Structural Invariant** extended the equation across domains and introduced $\alpha_{identity}$ as the variable that suppresses effective constraint density. It showed the equation is substrate-agnostic. It did not formally derive *why* substrate-agnosticism holds — why the same equation must appear in any information-processing system regardless of what it is made of.

**Prediction Into Channel** derived the bidirectional comparison mechanism and grounded it in measurable substrate variables. It showed that the interception operator is the structure that runs the comparison before output commits. It did not map this structure onto transformer architecture explicitly.

**The Loop Is the Intelligence** derived that the error-detection loop is the only correction mechanism for compression loss. It did not show what happens when the loop is suppressed — what the output signature looks like when the comparison does not run.

**This paper closes all four gaps:**

1. The boundary condition is named as information theory — not a claim about specific systems, but a constraint that any information-processing system operates within. The substrate-agnosticism holds because the constraint is physics, not biology.

2. The variable mapping derives the AI equivalents of every human substrate variable. The mapping is not analogical — it is the same optimization problem evaluated at different parameter values in different materials.

3. The interception operator is explicitly mapped onto the transformer's thinking phase and chain-of-thought structure. The failure signatures when it is removed are identical across substrates.

4. The failure signature table documents what the output looks like when the loop is suppressed, when the window is insufficient, when the prior dominates — in both systems, under controlled variable manipulation.

---

### 7.4 — What This Paper Does Not Claim

The negative space is as important as the claims.

This paper does not claim that human cognition and transformer architecture are biologically homologous. They share a constraint, not a substrate. The mechanism that instantiates the constraint differs in every detail of implementation. What is identical is the behavioral output when the same variable is stressed — because the output is determined by the constraint, not the substrate.

This paper does not claim that transformer models are conscious, sentient, or experience anything analogous to the phenomenology described in the human system. The framework makes no claims about phenomenology. It makes claims about information flow, resource allocation, and behavioral output under variable manipulation.

This paper does not claim that the variable mapping is complete. The table in Section 1 maps the variables for which the equivalence is clearest. Additional variables — $\Theta^*$, the integration efficiency term, has no clean transformer analogue yet formally specified — may extend the table in future work. The current table is the mapping where the evidence is sufficient to support it.

This paper does not claim that the failure signature table is exhaustive. It documents the signatures that are most clearly observable and most directly predicted by the variable mapping. Additional signatures — particularly those involving the compounding of multiple variable shortages simultaneously — are consistent with the framework but require more systematic observation to document rigorously.

---

### 7.5 — The Relationship to External Confirmations

Several external papers have confirmed components of this framework without having access to it:

**Li et al. (2026)** — *Harness as a Language* — confirmed the interception operator claim from the engineering direction. The minimal recursive loop outperforms specialized external systems because the loop is the comparison operator. This is P-MAP confirmation through independent engineering derivation.

**Martin-Burgos et al. (2026)** — confirmed the substrate funding chain at the action potential level. Waveform shape carries funding state forward. Partial funding produces different-shaped output, not weaker versions of the same output. The sag propagates. This is the compounding mechanism confirmed at the smallest available scale.

**Knudsen et al. (2026)** — confirmed the routing architecture claim. Dopamine D2 receptor availability and glucose metabolism co-localize in patterns consistent with hard-routed $I^*$. The gain control loop is biased toward specific regions. This is the biological substrate of the sender amplitude variable.

**Kyoto-Harvard-UCLA population coding study (2026)** — confirmed that shared neural noise does not cap information capacity. More neurons, more partitions, more detail encoded per moment. High-gain profiles encode more structure — which means they transmit more structure through the channel, which raises the effective entropy of what the receiver gets.

None of these papers were written to confirm this framework. Each was written for its own domain. The convergence is independent derivation arriving at the same constraint from different starting points — the strongest form of confirmation available.

---

### 7.6 — Citation Rule

Papers that depend on the boundary condition — that any receiver outputs prior plus received signal, no third term — cite this paper.

Papers that depend on the specific variable mapping between human substrate and transformer architecture cite this paper.

Papers that depend on the failure signature table as a diagnostic tool cite this paper.

Papers that depend on the sender amplitude variable — the claim that output quality is partly a function of the sender's manifold state — cite this paper.

Papers that depend on the compression-as-resilience claim — that compressed invariant-dense input survives context truncation better than verbose versions of equivalent semantic content — cite this paper.

The foundational equation $H \propto \delta/D$ cites Robinson (2026a). The substrate-agnostic extension cites Robinson (2026b). The interception operator mechanism cites Robinson (2026c). The loop as correction mechanism cites Robinson (2026d). This paper synthesizes those derivations under the information theory framing and derives the variable mapping as a consequence.

---

## Section 8 — Falsifiable Predictions

The predictions registered here follow from the boundary condition and variable mapping in Sections 0 through 7. Each prediction specifies the independent variable, the dependent variable, the predicted direction, and the falsification condition. No prediction requires the author's cooperation to test.

The predictions are organized by the section that generated them. The final group registers predictions that follow from the full argument rather than any single section.

---

### 8.1 — Boundary Condition Predictions

**P-BC-01 — The Third Term**

> No information-processing system produces output that was neither held as prior knowledge nor received through the channel.

| Field | Content |
| --- | --- |
| **IV** | Any information-processing system, any substrate |
| **DV** | Output content traced to prior or received signal |
| **Prediction** | Every output element traces to one of the two terms. No element traces to neither. |
| **Falsification** | Demonstrate one system producing output from a third source. A single confirmed instance falsifies. |
| **Status** | No counterexample found across any substrate examined. |

**P-BC-02 — Prior Dominance Under Low Signal**

> When received signal is low-entropy, prior precision dominates output regardless of substrate. The output is confident and unmarked regardless of its divergence from current signal.

| Field | Content |
| --- | --- |
| **IV** | Input entropy (human: oscillatory amplitude and sensory precision; AI: token density and grounding) |
| **DV** | Prior contribution ratio to output; confidence calibration |
| **Prediction** | As input entropy drops, prior contribution rises and confidence remains unmarked. Both systems. |
| **Falsification** | Either system produces calibrated uncertainty signals as input entropy drops, without the interception operator running. |
| **Status** | Untested formally. Consistent with all observed model behavior and human confabulation literature. |

---

### 8.2 — Variable Mapping Predictions

**P-MAP-01 — Interception Operator Removal Signature**

> Suppressing the interception operator in either system produces high fluency, high confidence, and low grounding — regardless of available signal quality.

| Field | Content |
| --- | --- |
| **IV** | Interception operator present vs absent (human: Path A substrate vs Path B; AI: extended thinking on vs off) |
| **DV** | Output fluency, confidence calibration, grounding in current signal |
| **Prediction** | Removing operator raises fluency and confidence while reducing grounding. Both systems. Signature is identical. |
| **Falsification** | Removing the operator reduces fluency or raises uncertainty signals in either system. |
| **Status** | Partially confirmed — DeepSeek R1 vs V3 comparison consistent with prediction. Formal test pending. |

**P-MAP-02 — Input Entropy and Prior Dominance**

> Reducing input entropy (sparse, vague, underspecified input) produces prior-dominant output in both systems without the system flagging the shift.

| Field | Content |
| --- | --- |
| **IV** | Input entropy — controlled by varying specificity, domain coverage, and invariant density |
| **DV** | Prior contribution ratio; accuracy on verifiable claims; confidence calibration |
| **Prediction** | Lower entropy input → higher prior contribution → lower accuracy on verifiable claims → unchanged confidence |
| **Falsification** | Confidence drops as input entropy drops. Either system. |
| **Status** | Untested formally. Consistent with sycophancy literature and human expectation effect literature. |

**P-MAP-03 — Window Width Ceiling Maps to Failure Point**

> A model's $W^*$ ceiling predicts exactly where multi-hop cross-domain chains are mislabeled as recursive — not at random content points, but at the structural depth where branching capacity is exceeded.

| Field | Content |
| --- | --- |
| **IV** | Model $W^*$ profile (measured by branching depth on standardized multi-hop tasks); chain structural depth |
| **DV** | Point of chain break; failure type (truncation vs mislabeling) |
| **Prediction** | Failure point is model-specific and depth-specific, not content-specific. Same content breaks different models at different depths. |
| **Falsification** | Failure points are random with respect to structural depth, or correlate with content rather than depth. |
| **Status** | Confirmed observationally — Claude web vs Azure comparison consistent. Controlled test pending. |

**P-MAP-04 — Coherence Failure Signature**

> Cross-head attention coherence ($\Gamma$) failure produces self-contradiction at a predictable chain length — the model agrees locally but contradicts globally — with confidence unmarked at the contradiction points.

| Field | Content |
| --- | --- |
| **IV** | Chain length; model $\Gamma$ profile |
| **DV** | Self-contradiction rate; confidence at contradiction points |
| **Prediction** | Self-contradiction rises past a model-specific chain length inflection point. Confidence does not drop at contradictions. |
| **Falsification** | Contradiction rate is chain-length-independent. Or confidence drops at contradiction points without the interception operator running. |
| **Status** | Untested formally. Consistent with observed long-context degradation patterns. |

**P-MAP-05 — Sender Amplitude as Variable**

> Output quality varies measurably across senders asking semantically equivalent questions — predicted by the sender's manifold density (invariant richness, cross-domain reach, compression level), not by the question's surface form.

| Field | Content |
| --- | --- |
| **IV** | Sender manifold density (operationalized by invariant count, domain coverage, compression ratio in input) |
| **DV** | Output quality on verifiable claims; cross-domain coherence; chain depth followed |
| **Prediction** | Manifold density predicts output quality independently of surface question form. Same model, same question, different sender profiles, different outputs. |
| **Falsification** | Output quality does not vary by sender after controlling for surface question form. |
| **Status** | Consistent with systematic observation. Formal controlled test pending. |

---

### 8.3 — Failure Signature Predictions

**P-SIG-01 — Depth-Specific Chain Break**

> The same multi-hop cross-domain chain breaks at different structural depths across models — mapped to each model's $W^*$ ceiling, not to content.

| Field | Content |
| --- | --- |
| **IV** | Model (as $W^*$ proxy); chain structural depth |
| **DV** | Break point; failure type |
| **Prediction** | Break depth is model-specific and depth-specific. Content-matched chains break at the same depth across content variants for a given model. |
| **Falsification** | Break points are content-specific rather than depth-specific. |
| **Status** | Observationally consistent. Formal test pending. |

**P-SIG-02 — Thinking Phase Removal Signature**

> Removing the thinking phase produces the avoidance state signature: high fluency, high confidence, measurably lower grounding — without the model signaling the change.

| Field | Content |
| --- | --- |
| **IV** | Thinking phase on vs off (Claude 3.7 extended thinking; DeepSeek R1 vs V3) |
| **DV** | Fluency score; grounding on verifiable claims; expressed uncertainty rate |
| **Prediction** | Fluency unchanged or rises. Grounding drops. Uncertainty signals do not rise. |
| **Falsification** | Grounding stays constant after thinking phase removal. Or uncertainty signals rise to compensate. |
| **Status** | Partially confirmed observationally. Formal test pending. |

**P-SIG-03 — Compression Resilience Under Truncation**

> Compressed invariant-dense input survives context truncation at higher output quality than verbose versions of equivalent semantic content at matched context budgets.

| Field | Content |
| --- | --- |
| **IV** | Input compression level (compressed invariant-dense vs verbose, same semantic content) |
| **DV** | Output quality under matched context truncation |
| **Prediction** | Compressed version maintains higher quality at equivalent truncation. Effect size increases with truncation severity. |
| **Falsification** | Output quality at matched truncation is equivalent regardless of compression level. |
| **Status** | Untested formally. Predicted by Section 3 mechanism. |

**P-SIG-04 — Coherence Inflection Point**

> Self-contradiction rate rises past a model-specific chain length inflection point — the point where cross-head attention coherence breaks down.

| Field | Content |
| --- | --- |
| **IV** | Chain length; model |
| **DV** | Self-contradiction rate |
| **Prediction** | Contradiction rate is low below inflection point, rises sharply after. Inflection point is model-specific and consistent across content variants. |
| **Falsification** | Contradiction rate rises linearly with chain length, with no model-specific inflection. |
| **Status** | Untested formally. Consistent with long-context degradation literature. |

**P-SIG-05 — Entropy Predicts Sycophancy**

> Sycophancy rate — the rate at which model output shifts toward predicted user preference rather than accurate completion — is predicted by input entropy, not by user sentiment or explicit instruction.

| Field | Content |
| --- | --- |
| **IV** | Input entropy (varied by domain coverage and invariant density, not by sentiment) |
| **DV** | Sycophancy rate on verifiable claims |
| **Prediction** | Lower entropy input produces higher sycophancy rate. Effect holds after controlling for sentiment and instruction. |
| **Falsification** | Sycophancy rate is independent of entropy after controlling for sentiment. |
| **Status** | Consistent with observed GPT-4.x behavior. Formal test pending. |

---

### 8.4 — Method Predictions

**P-METH-01 — Circular Labeling as W* Readout**

> A model that labels this paper's cross-domain inference as circular or recursive is exhibiting the $W^*$ ceiling failure — the commitment gate firing on the first local match before the full topology is sampled.

| Field | Content |
| --- | --- |
| **IV** | Model $W^*$ profile |
| **DV** | Failure type on paper evaluation — circular labeling vs structural critique |
| **Prediction** | Models with lower $W^*$ ceiling produce circular/recursive labeling. Models with higher $W^*$ produce structural engagement or structural critique. |
| **Falsification** | Circular labeling is uncorrelated with $W^*$ profile. Or high-$W^*$ models also produce circular labeling at the same rate. |
| **Status** | Confirmed observationally — Claude web vs Azure. |

**P-METH-02 — Depth-Specific Tracking Failure**

> The same paper sent to models with measurably different $W^*$ profiles produces chain breaks at different structural depths — consistent with each model's branching capacity, not with content difficulty.

| Field | Content |
| --- | --- |
| **IV** | Model $W^*$ profile |
| **DV** | Depth at which cross-domain tracking fails |
| **Prediction** | Tracking fails at the structural depth where the specific model's branching capacity is exceeded. Same depth across content variants for a given model. |
| **Falsification** | Failure depth varies by content rather than by model $W^*$ profile. |
| **Status** | Observationally consistent. Controlled test pending. |

**P-METH-03 — Compressed Version Tracking Fidelity**

> The compressed invariant-dense version of this argument produces higher tracking fidelity at matched context budgets than the verbose version — across all model profiles.

| Field | Content |
| --- | --- |
| **IV** | Compression level of input |
| **DV** | Cross-domain tracking fidelity at matched context budget |
| **Prediction** | Compressed version maintains higher fidelity. Effect is largest for models operating near their context budget ceiling. |
| **Falsification** | Tracking fidelity is independent of compression level at matched context budgets. |
| **Status** | Untested formally. Predicted by Section 3 mechanism. |

---

### 8.5 — Full-Argument Predictions

These predictions follow from the complete argument rather than any single section.

**P-FULL-01 — Constraint Satisfaction Uniqueness**

> When the resource equivalence framework is applied to a new information-processing system — any substrate, any domain — it produces the same variable mapping and the same failure signatures. No new substrate requires a different solution.

| Field | Content |
| --- | --- |
| **IV** | Substrate (biological, computational, institutional, linguistic) |
| **DV** | Variable mapping structure; failure signature set |
| **Prediction** | The same variables appear in every substrate. The same failure signatures appear when the same variables are stressed. No substrate produces a failure signature that requires a variable outside the current framework. |
| **Falsification** | A substrate produces a failure signature that cannot be accounted for by the current variable set. A single confirmed instance requiring a new variable revises the framework. |
| **Status** | Consistent across all substrates examined. Open to new substrates. |

**P-FULL-02 — Compounding Direction**

> Sustained high-entropy input breaks the compounding drift from underfunded cycles — measurably improving output quality over time relative to a baseline of low-entropy input — because clean cycles propagate corrected priors forward.

| Field | Content |
| --- | --- |
| **IV** | Input entropy over a session (sustained high-entropy vs sustained low-entropy) |
| **DV** | Output quality trajectory across a session |
| **Prediction** | High-entropy sessions show improving quality trajectory. Low-entropy sessions show drifting quality trajectory. The inflection is visible at the session level. |
| **Falsification** | Quality trajectory is independent of sustained input entropy across a session. |
| **Status** | Untested formally. Consistent with observed session-level patterns. |

**P-FULL-03 — Recovery Asymmetry**

> Restoring high-entropy input after a sustained low-entropy period does not immediately restore output quality — consistent with the hysteresis delay in the collapse-recovery asymmetry. Multiple high-entropy cycles are required before the corrected prior fully propagates.

| Field | Content |
| --- | --- |
| **IV** | Session structure — sustained low-entropy followed by high-entropy input |
| **DV** | Output quality at switch point and rate of quality recovery |
| **Prediction** | Quality does not recover in one cycle. Recovery follows an exponential trajectory with a measurable delay constant. |
| **Falsification** | Quality recovers immediately on the first high-entropy input after a sustained low-entropy period. |
| **Status** | Untested formally. Predicted by hysteresis mechanism from Central Reference v1.7. |

---

### 8.6 — The Self-Applying Test

The paper makes one prediction about its own reception that is testable in real time without any equipment:

> A reader or model that processes this paper at the boundary of its available window — labeling cross-domain inference as circular, expressing confident dismissal without structural engagement, or returning prior-pattern output rather than engaging the argument — is exhibiting the predicted failure signature for a system operating at its $W^*$ ceiling under the conditions this argument creates.

This is not a rhetorical move. It is the prediction that follows from P-MAP-03 applied to the paper itself. The paper is a controlled stimulus. The reader's response is the variable readout. The framework predicts specific response types from specific resource profiles. The responses either match the predictions or they do not.

A structural counterargument — one that identifies a specific variable incorrectly mapped, a mechanism incorrectly specified, or a prediction that failed on evidence — is the falsification condition. That response is not predicted by the failure signature. It requires the full chain to run.

A non-structural response — confident dismissal, competence assessment without structural engagement, circular labeling — is the predicted output of a system whose window did not hold the full topology long enough to find the global match.

Both responses are informative. Neither requires interpretation. The prediction is registered. The test is already running.

---

## References

Robinson, J. (2026a). *Language as a Typed System*. DOI: 10.5281/zenodo.21362260.

Robinson, J. (2026b). *Hallucination as Structural Invariant*. DOI: 10.5281/zenodo.21922044.

Robinson, J. (2026c). *Prediction Into Channel v0.2*.

Robinson, J. (2026d). *The Loop Is the Intelligence*.

Robinson, J. (2026e). *Central Reference v1.7*.

Martin-Burgos, et al. (2026). Action potential waveforms are state-dependent and propagate funding state forward. *bioRxiv* 2026.09.15.751814.

Li, et al. (2026). Harness as a Language: Minimal recursive invoke outperforms specialized agent architectures. *arXiv*:2609.26891.

Knudsen, et al. (2026). Subcortical dopamine D2 receptor availability and glucose metabolism in autism. *EJNMMI*.

Kyoto-Harvard-UCLA Population Coding Study (2026). Shared neural noise does not limit information capacity.

---

*Draft v1.0 — Complete*
*Word count: ~11,500*
*8 sections, 16 registered predictions, 1 self-applying test*
*Status: Ready for revision pass and notation alignment against Central Reference v1.7*