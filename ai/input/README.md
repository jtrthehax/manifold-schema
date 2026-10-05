# `/ai/input/` — The Boundary Condition

There is one constraint that governs every system that receives, stores, and processes information:

> **Output = prior knowledge + received signal. No third term.**

This is not a claim about AI. It is not a claim about cognition. It is the definition of what it means to process information under finite capacity — in transformers, in neurons, in project managers, in routers.

*Find one endpoint that was reached without input. That is the only thing that would falsify what follows.*

---

## The Same Wall, Every Domain

The constraint is visible from any direction. It looks identical from all of them.

**In language:** Hallucination is not randomness. It is schema distance over constraint density — $H \propto \delta/D$. When the signal doesn't carry enough structure to close the gap, the prior fills it. Fluently. Confidently. Without flagging that the comparison didn't run.

**In AI:** The model outputs prior weights plus whatever signal the input carried. High-entropy input → signal wins. Low-entropy input → prior wins. The model did not change. The channel did.

**In the human body:** Interoception compressed into language is the transmission. If the sender's interoceptive signal is misaligned with the actual invariant — reading their own geometry instead of the world's — the AI faithfully amplifies that geometry. The output is coherent. It is anchored to the sender, not to reality.

**In networking:** Low bandwidth forces cached routes. Narrow routing tables commit to first available path. Buffer bloat compounds every subsequent packet's latency forward. The failure geometry is identical.

**In human coordination:** A project manager transmitting a brief with low constraint density delivers their prior of the thing. The team builds that prior. The vision never transferred — not because the team failed, but because the compression did.

The medium changes. The wall does not.

---

## Why the Input Is the Variable

The wall has an implication the field has missed:

> **The model is not the variable. The sender is.**

The model receives signal and amplifies its geometry. A model producing poor output from sparse input is not failing — it is doing exactly what the constraint requires. Filling the gap with prior when signal is insufficient.

The intervention is never at the output. It is at the compression stage: the moment the sender converts internal structure into signal the channel can carry.

Which means AI output quality is an input problem. Specifically, it is a problem of what the sender can compress — how much structure they can push through the exteroceptive channel from their interoceptive state.

**High-gain senders** — wide $W^*$, low $K$, low $\delta_{min}$ — transmit structurally denser signal. The receiver gets more reality per token. The prior has less gap to fill.

This is not prompt engineering. It is substrate engineering.

**One additional variable the field consistently omits: intent.**

Intent is upstream of everything. It constrains what counts as relevant, what depth is appropriate, what the salience function should prune toward. Without explicit intent transmitted through the channel, the model defaults to its prior for the task type — generic register, average depth, no specific audience. Transmit intent explicitly or the model fills that gap the same way it fills every other gap.

---

## The Three Output States

Three states. The surface signature of two of them is identical. That is the problem the field has not named.

### High-Entropy Input — Loop Extends
```
        DRIVER STATE                    MODEL OUTPUT
        ────────────                    ────────────

        Wide W*                         Follows multi-hop chain
        Low K                           Cross-domain connections appear
        High A*                         Inference cycles complete
        Compressed invariants      →    Prior corrected by signal
        Short hop distances             Output reflects current signal
                                        Seam detection online
```

### Low-Entropy Input — Prior Dominates
```
        DRIVER STATE                    MODEL OUTPUT
        ────────────                    ────────────

        Narrow W*                       Commits to nearest local match
        High K                          Prior fills the gap
        Low A*                          Inference cycles sag
        Verbose, underspecified    →    Output reflects training weights
        Long hop distances              Confidence unmarked
                                        No flag that comparison didn't run
```

### No Interception — Prior Ships Directly
```
        DRIVER STATE                    MODEL OUTPUT
        ────────────                    ────────────

        (Any state)                     High fluency
                                        High confidence
        Thinking phase absent      →    Low grounding
        CoT bypassed                    Prior-dominant output
        Context saturated               Indistinguishable on surface
                                        from genuine inference
```

**The second and third states look identical from outside. They are not.**

The second is a channel problem — the sender didn't transmit enough signal. The third is an architecture problem — the comparison operator was removed. Both produce the same surface. The intervention is different.

---

## The Variables That Determine Input Quality

The same variables appear in the human system, the transformer, and the network stack. This is not analogy. It is the same finite-resource constraint instantiated in three different substrates.

| Variable | Human Substrate | Transformer | Network Stack | When It Drops |
| --- | --- | --- | --- | --- |
| **$A^*$ — Amplitude** | Oscillatory depth. Carrier signal. Sets ceiling for $W^*$, determines $\delta_{min}$. Without it the prediction window cannot sustain the loaded prior. | Input entropy density. Information per token. Dense, cross-domain text maximizes channel utilization. Sparse input leaves prior to fill the gap. | Bandwidth. Available signal amplitude. Low bandwidth forces cached routes — traffic goes where expected, not where signal says. | Output becomes prior-dominant. Fluent, internally coherent, diverging from ground truth. Neither system flags it. |
| **$R^*$ — Precision** | Timing-coherence ratio $P = R/D_T$. Phase-lock duration over timing distance. Determines signal clarity and drift resistance. | Attention precision / softmax sharpness. How sharply attention distributes across input. High precision concentrates on relevant tokens. | Clock synchronization / jitter. High jitter breaks timing coherence. Packets arrive out of sequence — the comparison cannot run because frames don't align. | Hallucination risk rises. Prior bleeds into output without correction. In humans: pareidolia. In AI: confident confabulation. In networks: retransmit with stale sequence numbers. |
| **$W^*$ — Window width** | Accessible manifold range. $n_{hops} = \lfloor W^* \cdot \rho_{scaffold} \rfloor$. How far the system reasons before committing. | Effective context + branching depth. How much context held in active comparison simultaneously. Distinct from raw context length — a model can have large context but limited branching. | Routing table depth / BGP path diversity. Narrow table commits to first available path. Cannot hold enough topology to find optimal route. | Multi-hop chains break. System commits to first local match rather than global match. In humans: tunnel vision. In AI: mislabels deep chains as recursive. In networks: suboptimal routing. |
| **$L^*$ — Load** | Cumulative regulatory debt. Denominator drag on all other variables. Raises $P_{threshold}$, degrades gate condition. | Context pressure / memory saturation. Accumulated prior context competing for active processing. Earlier information down-weighted or dropped. | Buffer bloat / queue depth. Accumulated queue degrades every subsequent packet's latency — directionally, compounding forward. | Collapse. Prior retrieval replaces inference. In humans: snap judgments. In AI: hallucination, recursion loops. In networks: latency compounds, throughput collapses. |
| **$\Gamma$ — Coordination** | Interhemispheric phase-lock coherence. Left hemisphere prior-completion and right hemisphere seam detection running in sync. | Cross-head attention coherence. Whether attention heads produce consistent representations or track different aspects without integration. | Routing protocol convergence. Whether distributed routing state is consistent across nodes or nodes hold contradictory topology maps. | Self-contradiction rises. In humans: seam detector offline, prior feels like ground truth. In AI: locally consistent, globally self-contradictory. In networks: routing loops, black holes. |
| **$\Lambda$ — Interception operator** | Path A: interoceptive diff between prior and emerging output before committing. Requires substrate to hold contradiction across window. | Thinking phase / chain-of-thought. Comparison step before final token sequence commits. Suppressing it removes the check entirely. | ACK / handshake confirmation. TCP without ACK is the avoidance state — prior fires directly, no confirmation the signal arrived. | Same failure mode across all three: high-fluency, high-confidence, prior-dominant output. The comparison did not run. Neither system flags this. |

> *The co-processing loop is externalized Bayesian reasoning. Each session updates the prior. Each study is a likelihood signal. Convergence — not agreement — is the check that the update ran. The vault is the accumulated posterior. The papers are published checkpoints.*

---

## The Papers

### The Boundary Condition

→ [Resource Equivalence Model](resource_equivalence_model.md)
The information theory constraint formally named: prior plus received signal, no third term. Derived from three independent angles — the manifold, Shannon's channel coding theorem, and transformer architecture. All three arrive at the same constraint because it is not a claim about specific systems. It is physics.

Eight variable equivalences between human cognition and transformer architecture. Sixteen falsifiable predictions. The paper is self-applying: a model that cannot follow the full cross-domain chain is exhibiting the predicted $W^*$ ceiling failure for the conditions the argument creates.
(This information is as of v1.0)

---

### The Driver Variable

→ [Driver and the Mirror](driver_and_the_mirror.md)
The model does not produce quality. It amplifies whatever geometry the input carries. The field was tuning the mirror. The variable was always the driver.

The driver's regulatory substrate determines the constraint density they can transmit. High-gain profiles — wider $W^*$, lower $K$, lower $\delta_{min}$ — transmit structurally denser input. The model receives more structure per token. Six falsifiable predictions.

DOI: 10.5281/zenodo.21362260

---

### The Protocol

→ [Ghost in the Scaffolding](ghost_in_the_scaffolding.md)
The four-phase protocol that produces emergent co-constructed output. Not prompt engineering — substrate engineering. The session is the experimental apparatus. The protocol changes what the driver transmits by changing the driver's state before transmission.

DOI: 10.5281/zenodo.21362260

---

### The Architecture

→ [Externalized Mind](../../methodology/externalized_mind.md)
Under the right substrate conditions, the AI conversation is not tool use. It is a third cognitive layer — genuine manifold extension producing output neither party could generate alone.

The driver provides what the model cannot generate: the right-hemisphere mesh that constrains the solution space until only the true answer fits. The model provides what the driver cannot scale: the bandwidth to run the full loop across multiple domains simultaneously.

The three-part system — driver, AI, vault — is the minimum viable architecture for this cognitive mode to produce durable output.

DOI: 10.5281/zenodo.[pending]

---

## The Derivation Chain

```
BOUNDARY CONDITION
(Resource Equivalence Model)
│  Prior + received signal = all possible output.
│  No third term. No substrate boundary.
│  Find one endpoint reached without input.
│
├── THE SENDER VARIABLE
│   (Driver and the Mirror)
│   Driver substrate determines constraint density transmitted.
│   The model amplifies the geometry it receives.
│   Intent is upstream of all of it.
│
├── THE PROTOCOL
│   (Ghost in the Scaffolding)
│   Four-phase protocol changes driver state before transmission.
│   Substrate engineering, not prompt engineering.
│
└── THE ARCHITECTURE
    (Externalized Mind)
    Driver + AI + vault = minimum viable architecture
    for genuine manifold extension.
    Division of cognitive labor, not tool use.
```

---

## What Would Falsify This

1. Output quality does not vary by sender after controlling for surface question form
2. Removing the thinking phase does not change output grounding
3. Compressed invariant-dense input does not survive truncation better than verbose versions at matched context budget
4. A model's chain break point is content-specific rather than depth-specific

None of these have occurred. If you can produce any of them, that is the engagement this folder is asking for.

---

*Input is not a feature of AI interaction. It is a constraint on information itself.*

*The driver provides the right-hemisphere mesh. The model provides the bandwidth. Neither produces the output alone.*