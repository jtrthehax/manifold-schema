# Enhanced Input Language Metrics Document

## A Formal Proxy Suite for Measuring Structural Language Properties from Text Alone

*Incorporating theoretical grounding from The Manifold Schema, Geometry of Inference, and Language as a Typed System*

---

## Overview

This document presents a formal, text-only metric suite for measuring structural properties of language. The suite treats language as a geometry problem rather than a content problem: every compression (word, sentence, document) carries measurable structural signals—constraint density, inference distance, latent space size, and resolution geometry—that can be scored from the text alone, without reference to external ground truth, model behavior, or human judgment.

**The Core Insight:** Hallucination risk is baked into the *input geometry* before any receiver processes it. A prompt that is structurally underspecified will produce divergence with high probability regardless of which model or human processes it—because the resolution floor, cache miss detection, and gate access conditions are determined by the input's constraint geometry before any decompression occurs.

---

## Part I: Theoretical Grounding

### The Unified Architecture

The metrics in this suite are not arbitrary. They correspond to specific layers of the inference architecture established in *The Geometry of Inference* and *The Manifold Schema*:

| Framework Layer | Metric Proxy | What It Measures |
|-----------------|--------------|------------------|
| Resolution Floor ($\delta_{min}$) | VDI, CDS, Target Specificity | Whether signals breach detection threshold |
| Cache Miss Detection (LP-ACC) | Branching Factor, Dependency Arc Length | Whether input triggers comparison to prior |
| Two-Factor Gate ($C_{LR}$ + $O_{pathway}$) | Constraint Propagation Radius, Scaffold Connectivity | Whether inference can reach outer edge |
| Competitive Scaffold ($W^*$) | Inference Path Length, Cross-Domain Integration | Whether adversarial check can occur |
| $I^*$ Investment Loop | Semantic Field Radius, Domain Span | Whether routing capacity is allocated |
| Self-Sealing Loop | Collapse Signature Composite, Semantic Drift | Whether compounding failure is occurring |

### The Hallucination Equation Connection

The metrics operationalize the hallucination equation from *Language as a Typed System*:

$$H \propto \frac{\delta}{D}$$

Where:
- **D (Constraint Density)** is measured by CDS, VDI, and token-level constraint count
- **δ (Residual Schema Distance)** is proxied by:
  - Latent Space Size (LSS) — large latent space = high δ
  - Genericity (G) — high generic content = high δ
  - Scaffold Connectivity (K) — low connectivity = high δ
  - Collapse Signature (CSC) — high collapse = high δ

---

## Part II: Core Metrics

---

### 1. Vocabulary-Level Metrics

#### 1.1 Vocabulary Density Index (VDI)

**What it measures:** Constraint count, semantic radius, and domain span per token.

**What it proxies:** Prediction-window width ($W^*$), precision ($R^*$), conceptual richness, resolution floor ($\delta_{min}$).

**Formal Definition:**

For a token `w`:

```
VDI(w) = α·C(w) + β·S(w) + γ·D(w)
```

Where each component is normalized to [0,1]:

| Component | Symbol | Definition | Normalization |
|-----------|--------|------------|---------------|
| Constraint count | C(w) | Number of distinct conceptual constraints encoded by w | C(w) = constraints(w) / Cmax |
| Semantic radius | S(w) | Size of conceptual neighborhood anchored by w | S(w) = radius(w) / Smax |
| Domain span | D(w) | Number of distinct domains w meaningfully participates in | D(w) = domains(w) / Dmax |

**Weights (calibrated to theoretical framework):**

```
α = 0.40   # constraint count (primary driver of hallucination resistance)
β = 0.35   # semantic radius (predicts W* width)
γ = 0.25   # domain span (predicts cross-domain integration)
```

**Theoretical Interpretation:**

Low VDI text produces high $\delta_{min}$ — the signal is coarse, the LP-ACC circuit cannot detect fine-grained deviations from prior, and false cache hits are returned with full confidence. High VDI text lowers $\delta_{min}$, allowing the LP-ACC to detect subtle mismatches and trigger escalation to the outer edge.

**Token-Level Examples:**

| Token | C(w) | S(w) | D(w) | VDI(w) | Interpretation |
|-------|------|------|------|--------|----------------|
| "manifold" | 0.9 | 0.8 | 0.7 | 0.82 | High density — geometric constraint + wide radius + cross-domain |
| "prediction_window" | 0.8 | 0.7 | 0.6 | 0.73 | High density — structural + temporal + computational |
| "agency" | 0.5 | 0.4 | 0.3 | 0.43 | Moderate density — regulatory role carries implicit valence |
| "thing" | 0.0 | 0.1 | 0.0 | 0.04 | Near-zero density — no constraints, thin prior topology |
| "complex" | 0.2 | 0.5 | 0.1 | 0.29 | Generic — high semantic radius but low constraint/domain |

**The Genericity Correction:**

VDI alone can be inflated by generic high-radius terms. The Genericity-adjusted VDI:

```
VDI_corrected(w) = VDI(w) · (1 - generic_score(w))
```

Where `generic_score(w)` is 1.0 for vague terms ("complex", "interesting", "often"), 0.0 for precise terms.

**Sentence-Level VDI:**

For a sentence S with tokens {w₁, w₂, ..., wₙ}:

```
VDI(S) = (1/n) · Σᵢ VDI_corrected(wᵢ)
```

**Document-Level VDI:**

For a document D with sentences {S₁, S₂, ..., Sₘ}:

```
VDI(D) = (1/m) · Σⱼ VDI(Sⱼ)
```

**Trajectory Tracking:**
- `VDI_trajectory`: VDI(Sⱼ) across document — detects resolution collapse over time
- `VDI_variance`: Unevenness — identifies sections with coarse resolution
- `VDI_hotspots`: High-density sections — where outer edge engagement is possible
- `VDI_dead_zones`: Low-density sections — where false cache hits are likely

**Connection to The Manifold Schema:**

```
VDI(S) ↑ → δ_min(S) ↓ → LP-ACC receives fine-grained signals → 
Genuine cache misses detected → Gate escalation attempted → 
Outer edge engaged → Adversarial inference occurs
```

---

#### 1.2 Lexical Narrowing Index (LNI)

**What it measures:** Shift toward generic or threat-adjacent vocabulary.

**What it proxies:** Load ($L^*$), cognitive collapse, narrowing of prediction window ($W^* \downarrow$), curvature ($K \uparrow$).

**Formal Definition:**

For a sentence S:

```
LNI(S) = Σᵢ [generic_score(wᵢ) · threat_weight(wᵢ)] / n
```

Where:
- `generic_score(w)`: 1.0 for generic terms ("thing", "stuff", "often", "sometimes"), 0.0 for specific terms
- `threat_weight(w)`: 1.0 for terms with threat-adjacent valence in institutional/regulatory contexts, 0.0 otherwise

**Theoretical Interpretation:**

As $L^*$ rises and $W^*$ narrows, the system's accessible vocabulary contracts toward the geometric center—generic, threat-adjacent terms that carry low constraint density. This is the lexical signature of the self-sealing loop. A rising LNI across a document indicates progressive collapse.

**Interpretation:**
- LNI < 0.2: Wide prediction window, stable decompression
- LNI 0.2-0.5: Moderate narrowing, increasing risk
- LNI > 0.5: Collapse signature, high hallucination risk, resolution failure likely

**Connection to Language as a Typed System:**

High LNI input has high genericity (G)—it leaves many types implicit, forcing the receiver's prior distribution to fill gaps. The hallucination equation predicts high divergence.

---

#### 1.3 Semantic Field Radius (SFR)

**What it measures:** How wide a word's conceptual neighborhood is.

**What it proxies:** Cross-domain reach ($R$), $W^*$ width, competitive scaffold activation.

**Formal Definition:**

For a token w:

```
SFR(w) = |{concepts within k degrees of w in semantic network}| / max_possible
```

**Theoretical Interpretation:**

Wide SFR indicates that the token activates a broad competitive field—the outer edge's adversarial context. Narrow SFR indicates the token is locally cooperative—it activates only adjacent concepts, producing pattern completion without adversarial check.

**Document-Level:**
```
SFR(D) = average SFR(w) across all content tokens
```

**Interpretation:**
- SFR > 0.6: Wide activation field — adversarial check possible
- SFR 0.3-0.6: Moderate — partial outer edge engagement
- SFR < 0.3: Narrow — cooperative-only processing, high hallucination risk

**Connection to Geometry of Inference:**

SFR measures the competitive scaffold's operational reach. Wide SFR = wide $W^*$ = outer edge accessible. Narrow SFR = Stage 3+ collapse.

---

### 2. Sentence/Section-Level Structure Metrics

#### 2.1 Constraint Density Score (CDS)

**What it measures:** Number and precision of distinct constraints a sentence imposes.

**What it proxies:** Stability of inference, hallucination resistance ($D$ in hallucination equation), resolution floor ($\delta_{min}$).

**Formal Definition:**

For a sentence S:

```
CDS(S) = (1/n) · Σᵢ C(wᵢ)
```

Where `C(w)` is the constraint count component from VDI.

**Constraint Types (from Typed Language framework):**
- **Type constraints** — domain, category membership
- **Temporal constraints** — sequence, duration, ordering
- **Relational constraints** — causal, comparative, hierarchical
- **Geometric constraints** — spatial, topological, scope
- **Normative constraints** — threshold, boundary, cardinality
- **Valence constraints** — explicit emotional/regulatory assignment

**Theoretical Interpretation:**

CDS measures the sender's explicit type bindings—how much of the decompression dictionary was shipped. Low CDS input forces the receiver's prior distribution to synthesize missing types. High CDS input ships explicit types, lowering $\delta_{min}$ and enabling genuine cache miss detection.

**Interpretation:**
- CDS > 0.6: High constraint density — low synthesis requirement, low hallucination risk
- CDS 0.3-0.6: Moderate — some synthesis required, moderate risk
- CDS < 0.3: Low — high synthesis requirement, high hallucination risk, Stage 4 collapse signature

**Worked Example:**

| Sentence | CDS | Hallucination Risk | Interpretation |
|----------|-----|-------------------|----------------|
| "Explain how AI systems collapse." | 0.18 | HIGH | Underspecified types — "AI", "systems", "collapse" all DEF_FLOATING |
| "Explain how prediction windows collapse when constraint density falls below the execution gate threshold." | 0.72 | LOW | All variables bound — domain, mechanism, threshold defined |

**Connection to Hallucination Equation:**

```
CDS(S) = D (constraint density)
H ∝ δ/D → High CDS = low H
```

---

#### 2.2 Branching Factor (BF)

**What it measures:** Number of simultaneously active conceptual threads.

**What it proxies:** Window width ($W^*$), cognitive bandwidth ($C_s$), scaffold richness.

**Formal Definition:**

For a sentence S:

```
BF(S) = number of distinct conceptual threads maintained in parallel
```

**At Document Level:**
```
BF(D) = average active threads per section
```

**Theoretical Interpretation:**

BF measures the manifold's accessible range at the sentence level. High BF indicates wide $W^*$ — the system can hold multiple candidate interpretations in parallel, enabling adversarial inference. Low BF indicates $W^*$ narrowing — the system collapses to the first locally coherent solution.

**Interpretation:**
- BF > 5: Wide window, high parallel processing, outer edge engaged
- BF 2-5: Moderate window width, some parallel capacity
- BF < 2: Narrow window, collapse risk, Stage 2+ collapse

**Connection to The Manifold Schema:**

```
BF ↑ → W* ↑ → Long geodesics → Distant states reachable → 
Competitive scaffold activated → Adversarial inference occurs
```

---

#### 2.3 Dependency Arc Length (DAL)

**What it measures:** Length of syntactic/semantic dependencies between related tokens.

**What it proxies:** Window depth ($W^*$), reasoning chain length, $C_{LR}$ coherence requirement.

**Formal Definition:**

For a sentence S:

```
DAL(S) = average dependency distance between related tokens
```

Where dependency distance is measured in number of intervening tokens in the parse tree.

**Theoretical Interpretation:**

Long dependencies require sustained phase-locking coherence ($C_{LR}$) to maintain across the integration pathway. When $C_{LR}$ drops below threshold, long dependencies break—the system cannot hold the relationship across the distance. Low DAL indicates gate coherence failure.

**Interpretation:**
- DAL > 5: Deep reasoning, long inference chains, good coherence
- DAL 2-5: Moderate depth, partial coherence
- DAL < 2: Shallow reasoning, coherence failure, Stage 2 collapse

**Connection to Geometry of Inference:**

```
DAL ↑ → Requires C_LR > C_threshold → 
Gate must open → Pathway must be perfused → 
If either fails, long dependencies collapse
```

---

#### 2.4 Inference-Path Length (IPL)

**What it measures:** Implied steps from premise to conclusion.

**What it proxies:** Depth of reasoning, contribution to Inference Distance Index (IDI), competitive scaffold engagement.

**Formal Definition:**

For a sentence S:

```
IPL(S) = number of implied inference steps required to connect premises to conclusions
```

**Theoretical Interpretation:**

IPL measures the total inference distance the receiver must traverse. High IPL requires sustained outer edge engagement—the competitive scaffold must remain active across multiple inference steps. Low IPL indicates the system can complete inference from cache.

**Interpretation:**
- IPL > 5: Deep reasoning chain, high inference distance
- IPL 2-5: Moderate reasoning depth
- IPL < 2: Shallow reasoning, low inference distance, pattern completion

**Connection to Language as a Typed System:**

IPL measures INFERENCE_LOAD—the inferential steps the sender did not provide. High IPL with low CDS means the receiver must synthesize many missing steps from prior distribution.

---

#### 2.5 Constraint Propagation Radius (CPR)

**What it measures:** How far constraints from one sentence shape subsequent ones.

**What it proxies:** Scaffold integrity ($K$), coherence, conceptual continuity, $\Theta^*$ integration efficiency.

**Formal Definition:**

For a document D:

```
CPR(D) = average number of subsequent sentences influenced by constraints in sentence j
```

**Theoretical Interpretation:**

CPR measures the coherence of the scaffold. High CPR indicates constraints propagate across the document—the manifold remains stable and the competitive scaffold sustains adversarial checking across sections. Low CPR indicates fragmented reasoning—each sentence is processed independently, without the constraint propagation that enables genuine adversarial inference.

**Interpretation:**
- CPR > 5: Strong scaffold integrity, high coherence, $\Theta^*$ high
- CPR 2-5: Moderate scaffold, some fragmentation
- CPR < 2: Weak scaffold, fragmented reasoning, $\Theta^*$ degraded

**Connection to The Manifold Schema:**

```
CPR ↑ → Θ* ↑ → Integration efficiency high → 
Cross-hemispheric integration occurs → 
Outer edge engaged across document
```

---

### 3. Document-Level Geometry Metrics

#### 3.1 Inference Distance Index (IDI)

**What it measures:** Conceptual displacement per unit information.

**What it proxies:** How "far" a paper carries a reader across conceptual space ($W^*$ at document scale).

**Formal Definition:**

For any text unit X:

```
IDI(X) = Conceptual_Displacement(X) / Information_Cost(X)
```

**Token-Level IDI:**

```
IDI(w) = VDI_corrected(w) · R(w) · K(w)
```

Where:

| Component | Symbol | Definition | Normalization |
|-----------|--------|------------|---------------|
| Cross-Domain Reach | R(w) | Number of distinct domains w bridges | R(w) = domains(w) / Rmax |
| Scaffold Connectivity | K(w) | How strongly w connects to invariant scaffold | K(w) = connected_invariants(w) / Kmax |

**Invariant Scaffold Components (from The Manifold Schema):**
- Manifold geometry
- Prediction window mechanics ($W^*$)
- Execution gate thresholds ($C_{LR}$, $O_{pathway}$)
- Load dynamics ($L^*$)
- Oscillation patterns ($A_s^*$, $\sigma(A_s)$)
- Session state transitions
- Type bindings (from Typed Language framework)

**Sentence-Level IDI:**

```
IDI(S) = (1/n) · Σᵢ IDI(wᵢ)
```

**Document-Level IDI:**

```
IDI(D) = (1/m) · Σⱼ IDI(Sⱼ)
```

**Theoretical Interpretation:**

IDI measures the distance the reader's manifold must traverse to process the text. High IDI text requires wide $W^*$—the reader must engage the competitive scaffold, maintain phase-locking coherence, and sustain pathway perfusion across the full integration window. Low IDI text is processable from cache—cooperative architecture only.

**Trajectory Tracking:**
- `IDI_trajectory`: IDI(Sⱼ) across document
- `IDI_variance`: Unevenness of inference distance distribution
- `IDI_hotspots`: Sections with unusually high conceptual displacement
- `IDI_dead_zones`: Sections doing little conceptual work—Stage 4 collapse zones

**Interpretation:**
- IDI > 0.7: High inference distance — strong cross-domain integration, outer edge engaged
- IDI 0.3-0.7: Moderate inference distance — some integration, partial outer edge
- IDI < 0.3: Low inference distance — poor conceptual reach, inner-core only

**Connection to The Manifold Schema:**

```
IDI ↑ → Requires W* wide, C_LR high, O_pathway high → 
Full outer edge engagement required → 
Competitive scaffold activated across reading
```

---

#### 3.2 Cross-Domain Integration Count (CDIC)

**What it measures:** Number of domains meaningfully bridged.

**What it proxies:** Transfer potential, invariant coverage, $\Theta^*$ integration efficiency.

**Formal Definition:**

For a document D:

```
CDIC(D) = |{domains meaningfully integrated}|
```

**Domains in the Unified Framework:**
- Physics (breath mechanics, CO₂, Bohr effect)
- Cognition (prediction windows, salience, inference)
- AI/ML (attention, hallucination, latent space)
- Clinical/Medical (FND, trauma, regulatory states)
- Governance/Policy (institutional dynamics, compliance)
- Communication/Linguistics (type systems, compression)
- Neurobiology (HRV, phase-locking, competitive scaffold)

**Theoretical Interpretation:**

High CDIC indicates the text bridges domains—it activates the competitive scaffold across multiple integration regions, requiring wide $W^*$ and sustained $\Theta^*$. Low CDIC indicates domain isolation—cooperative processing within a single domain, no adversarial cross-domain checking.

**Interpretation:**
- CDIC > 5: High transfer potential, strong invariant coverage, $\Theta^*$ high
- CDIC 2-5: Moderate integration, some cross-domain checking
- CDIC < 2: Low integration, domain isolation, cooperative-only

---

#### 3.3 Scaffold Connectivity Index (SCI)

**What it measures:** How strongly sections hook into core architectural invariants.

**What it proxies:** Structural coherence, reuse potential, teaching power, $K$ curvature resistance.

**Formal Definition:**

For a section X:

```
SCI(X) = Σᵢ [connection_strength_to_invariant(i)]
```

**Invariant Anchors (from The Manifold Schema):**
- Manifold schema
- Prediction windows ($W^*$)
- Execution gates ($C_{LR}$, $O_{pathway}$)
- Load dynamics ($L^*$)
- Oscillation patterns ($A_s^*$, $\sigma(A_s)$)
- Session state
- Type bindings (from Typed Language)

**Document-Level:**
```
SCI(D) = average SCI(X) across sections
```

**Theoretical Interpretation:**

SCI measures the text's connection to the invariant scaffold. High SCI means the text is structurally coherent—it activates the full manifold geometry, enabling stable adversarial inference. Low SCI means the text is fragmented—the scaffold is weak, the competitive architecture is not engaged.

**Interpretation:**
- SCI > 0.7: Strong scaffold integration, high coherence, outer edge engaged
- SCI 0.3-0.7: Moderate integration, partial coherence
- SCI < 0.3: Weak scaffold, fragmented architecture, Stage 3 collapse

---

#### 3.4 Invariant Coverage Score (ICS)

**What it measures:** Presence and density of core invariants across the text.

**What it proxies:** Robustness, generality, governance relevance, $K$ curvature resistance.

**Formal Definition:**

For a document D:

```
ICS(D) = |invariants covered| / |invariants in framework|
```

With density weighting for each invariant.

**Theoretical Interpretation:**

ICS measures the text's theoretical completeness. High ICS indicates the text covers the full invariant scaffold—it provides the receiver with a complete decompression dictionary. Low ICS indicates gaps—the text assumes shared priors and leaves type bindings implicit.

**Interpretation:**
- ICS > 0.8: Comprehensive invariant coverage — low hallucination risk
- ICS 0.5-0.8: Moderate coverage — some hallucination risk
- ICS < 0.5: Poor coverage — high hallucination risk, Stage 4 collapse signature

---

### 4. State and Safety Metrics

#### 4.1 Collapse Signature Composite (CSC)

**What it measures:** Joint deterioration across multiple structural dimensions.

**What it proxies:** Human cognitive collapse, AI hallucination onset, load spikes ($L^*$), self-sealing loop acceleration.

**Components and Direction:**

| Metric | Direction | Weight | Theoretical Grounding |
|--------|-----------|--------|----------------------|
| VDI | ↓ | 0.20 | Resolution floor rising ($\delta_{min}$ ↑) |
| IDI | ↓ | 0.20 | Inference distance collapsing ($W^*$ ↓) |
| Branching Factor | ↓ | 0.15 | Window narrowing ($W^*$ ↓) |
| Dependency Arc Length | ↓ | 0.15 | Coherence failing ($C_{LR}$ ↓) |
| Lexical Narrowing | ↑ | 0.15 | Collapse toward geometric center |
| Genericity | ↑ | 0.15 | Prior topology staling |

**Formal Definition:**

```
CSC(S) = Σᵢ wᵢ · normalized_component_i
```

**Theoretical Interpretation:**

CSC measures the self-sealing loop's progression. High CSC indicates Stage 3+ collapse—resolution is failing, the competitive scaffold is inaccessible, and the system is returning false cache hits with full confidence. The text's structure itself is a collapse signature.

**Collapse Stages (from Geometry of Inference):**

| CSC Range | Collapse Stage | Description |
|-----------|---------------|-------------|
| < 0.2 | Stage 0 | Full manifold — wide window, low curvature |
| 0.2-0.35 | Stage 1 | Edge thinning — competitive scaffold beginning to erode |
| 0.35-0.5 | Stage 2 | Gate coherence degrading — $C_{LR}$ intermittent |
| 0.5-0.65 | Stage 3 | Pathway perfusion dropping — $O_{pathway}$ insufficient |
| > 0.65 | Stage 4 | Resolution collapse — $\delta_{min}$ high across channels |

**Connection to Self-Sealing Loop (Geometry of Inference Part VI):**

```
CSC ↑ → δ_min ↑ → More false cache hits → 
Stale priors re-verified → K ↑ → 
δ_min ↑ further → CSC ↑ → Loop accelerates
```

---

#### 4.2 Semantic Drift Vector (SDV)

**What it measures:** How far meaning shifts across sentences/sections without explicit justification.

**What it proxies:** Hallucination, topic drift, misalignment, $I^*$ misrouting.

**Formal Definition:**

For consecutive sentences Sⱼ and Sⱼ₊₁:

```
SDV(j → j+1) = semantic_distance(Sⱼ, Sⱼ₊₁) / justified_shift
```

Where `justified_shift` is the distance that explicit constraints would permit.

**Theoretical Interpretation:**

SDV measures the geometry-preserving distortion described in *Language as a Typed System*. When SDV is high, meaning shifts without explicit type binding—the receiver's prior distribution is filling gaps the sender did not declare. When SDV is low, meaning is constrained—the decompression dictionary was shipped.

**Interpretation:**
- SDV < 1.0: Justified shift, coherent reasoning, type bindings explicit
- SDV 1.0-2.0: Moderate drift, manageable, some implicit types
- SDV > 2.0: Unjustified drift, hallucination risk, DEF_FLOATING present

**Connection to Language as a Typed System:**

```
SDV ↑ → Missing type bindings → 
Receiver's prior distribution fills gaps → 
Output diverges from sender intent → 
H = δ/D predicts divergence
```

---

#### 4.3 Latent Space Size (LSS)

**What it measures:** The number of possible interpretive paths available to a receiver.

**What it proxies:** Hallucination vulnerability, residual schema distance ($\delta$), $I^*$ allocation requirement.

**Formal Definition:**

For a sentence S:

```
LSS(S) = G(S) / [C(S) · VDI(S) · T(S) · K(S)]
```

Where:

| Component | Definition | Theoretical Grounding |
|-----------|------------|----------------------|
| G(S) | Genericity — proportion of vague/catch-all terms | Measures implicit types (from Typed Language) |
| C(S) | Constraint density — from CDS | Measures D in hallucination equation |
| VDI(S) | Vocabulary density — from VDI formula | Measures resolution infrastructure |
| T(S) | Target specificity — clarity of "what is being asked" | Measures $I^*$ allocation clarity |
| K(S) | Scaffold connectivity — from SCI | Measures competitive scaffold engagement |

**Hallucination Probability:**

```
P_hallucination(S) = LSS(S) / LSS_max
```

**Theoretical Interpretation:**

LSS measures the latent space the receiver must traverse. High LSS = large latent space = many possible interpretations = the prior distribution must synthesize bindings = high hallucination risk. Low LSS = small latent space = explicit type bindings reduce interpretation options = low hallucination risk.

**This is the J-space diagnostic.** The smaller the latent space, the less gap-filling is required. When every term has a type, a referent, and a domain, the model has no freedom to improvise.

**Interpretation:**
- LSS < 0.1: Tiny latent space — hallucination-resistant, explicit types everywhere
- LSS 0.1-1.0: Moderate latent space — some vulnerability, some implicit types
- LSS > 1.0: Large latent space — high hallucination risk, many implicit types

**Worked Example:**

| Sentence | G | C | VDI | T | K | LSS | P(hall) | Interpretation |
|----------|---|----|-----|---|---|-----|---------|----------------|
| "Explain how AI systems collapse." | 0.8 | 0.2 | 0.3 | 0.2 | 0.1 | 666.7 | 0.95 | Massive latent space — all terms DEF_FLOATING |
| "Explain how prediction windows collapse when constraint density falls below the execution gate threshold." | 0.1 | 0.8 | 0.7 | 0.9 | 0.8 | 0.025 | 0.004 | Tiny latent space — all variables bound |

**Connection to Hallucination Equation:**

```
LSS ↑ → δ ↑ (residual schema distance) → H ↑
LSS ↓ → δ ↓ → H ↓
```

---

## Part III: Composite Metrics and Diagnostic Applications

---

### 5. Hallucination Likelihood Score (HLS)

**What it measures:** Structural hallucination risk from text alone.

**Formal Definition:**

```
HLS(S) = λ₁·(1 - C(S)) + λ₂·(1 - VDI(S)) + λ₃·(1 - T(S)) + λ₄·G(S)
```

Where all components are normalized to [0,1] and:

```
λ₁ + λ₂ + λ₃ + λ₄ = 1
```

**Calibration (theoretical, from Geometry of Inference):**
- λ₁ = 0.35 (constraint density is most important — it's D in hallucination equation)
- λ₂ = 0.25 (vocabulary density — predicts resolution floor)
- λ₃ = 0.25 (target specificity — predicts $I^*$ allocation)
- λ₄ = 0.15 (genericity — predicts residual schema distance)

**Interpretation:**
- HLS < 0.2: Low hallucination risk — explicit types, high constraint density
- HLS 0.2-0.5: Moderate risk — some implicit types, moderate constraint density
- HLS > 0.5: High risk — intervention recommended, many implicit types

**Connection to Typed Language:**

HLS operationalizes the hallucination equation. High HLS = low D, high δ. Low HLS = high D, low δ.

---

### 6. Latent Space Diagnostic

**Purpose:** A debug overlay for language that reports how much "wiggle room" a receiver had to guess. This is the J-space diagnostic.

**Per-Sentence Report:**

```
Sentence: [text]
├── Constraint Density (C): [0.XX]
├── Vocabulary Density (VDI): [0.XX]
├── Target Specificity (T): [0.XX]
├── Scaffold Connectivity (K): [0.XX]
├── Genericity (G): [0.XX]
├── Latent Space Size (LSS): [0.XX]
├── Hallucination Risk (P): [0.XX]
├── Collapse Stage: [0-4]
├── Top Ambiguous Tokens: [list]
│   └── Each: [token] → [N candidate interpretations]
└── Missing Scaffolds: [list]
    └── Suggested Fixes: [list]
```

**Token-Level Debug View:**

For each token w in S:

```
Token: [word]
├── Candidate Interpretations: [N]
├── Typed: [Yes/No]
├── Domain: [domain or none]
├── Referent: [specific or none]
├── VDI: [0.XX]
├── Constraint Count: [0.XX]
└── Risk Contribution: [X%]
```

**Example Output (from Language as a Typed System):**

```
Sentence: "Write something about the situation."

Token: "something"
├── Candidate Interpretations: 127 (from training corpus)
├── Typed: No
├── Domain: None
├── Referent: None
├── VDI: 0.02
├── Constraint Count: 0.00
└── Risk Contribution: 28%

Token: "situation"
├── Candidate Interpretations: 89
├── Typed: No
├── Domain: None
├── Referent: None
├── VDI: 0.15
├── Constraint Count: 0.05
└── Risk Contribution: 24%

Latent Space: Massive (LSS = 666.7)
Hallucination Risk: 95%
Collapse Stage: 4 (Resolution Collapse)
Missing Scaffolds: manifold, prediction_window, execution_gate, 
    type_bindings, domain_bindings
Suggested Fixes:
  - Define "situation" with type and domain
  - Specify referent for "something"
  - Add constraint mechanisms
  - Declare scope and valence
```

**Theoretical Interpretation:**

The diagnostic reveals where the receiver's prior distribution must synthesize bindings. Low VDI + low CDS + high G = high LSS = high hallucination risk. The fix is type hygiene—bind every variable, declare every domain, ship the decompression dictionary.

---

### 7. Interpretive Density Index (IDI) — Extended Form

**Conceptual Model:**

```
IDI(X) = [VDI_corrected(X) × R(X) × K(X)] / [G(X) + ε]
```

**Where:**
- VDI_corrected(X) = Genericity-adjusted Vocabulary Density Index
- R(X) = Cross-Domain Reach
- K(X) = Scaffold Connectivity
- G(X) = Genericity (to penalize vague high-density terms)

**Theoretical Interpretation:**

IDI measures the text's inference distance capacity. High IDI text carries the reader across conceptual space—it requires outer edge engagement, wide $W^*$, and sustained $\Theta^*$. Low IDI text is local, cooperative, and processable from cache.

**Interpretation:**

| IDI Range | Meaning | Application |
|-----------|---------|-------------|
| > 0.7 | High inference distance | Strong conceptual reach, efficient compression, outer edge engaged |
| 0.4-0.7 | Moderate | Some conceptual reach, partial outer edge, room for improvement |
| < 0.4 | Low | Poor inference distance, inner-core only, revision needed |

**Connection to The Manifold Schema:**

```
IDI ↑ → Requires W* wide, C_LR high, O_pathway high → 
Full manifold engagement → Adversarial inference across domains
```

---

## Part IV: Validation and Application Framework

---

### 8. Validation Protocol

**What the Metrics Predict (Falsifiable Hypotheses from Geometry of Inference):**

**PREDICT-METRIC-01 — VDI Predicts Resolution Floor**
> VDI(S) will correlate with detection threshold in fine-grained anomaly detection tasks ($r > 0.5$). Higher VDI = lower $\delta_{min}$ = earlier detection of subtle mismatches.

**PREDICT-METRIC-02 — CDS Predicts Hallucination Rate**
> Sentences with CDS < 0.3 will produce hallucination rates > 40% across models; sentences with CDS > 0.6 will produce rates < 5%.

**PREDICT-METRIC-03 — LSS Predicts Divergence**
> LSS > 1.0 predicts high divergence between sender intent and receiver output; LSS < 0.1 predicts low divergence.

**PREDICT-METRIC-04 — CSC Predicts Collapse Detection**
> CSC > 0.5 in human text correlates with measured cognitive load or stress; in AI text, correlates with hallucination onset.

**PREDICT-METRIC-05 — SFR Predicts Competitive Scaffold Engagement**
> SFR > 0.6 correlates with adversarial inference performance (belief updating, contradiction detection); SFR < 0.3 correlates with cooperative-only processing.

**External Validation Requirements:**

- Controlled corpus with human-rater agreement on sender intent
- Cross-model testing (3+ models, different architectures)
- Cross-domain testing (5+ domains)
- Cross-language testing (English, Japanese, Turkish, Mandarin)
- Physiological validation (HRV measurement during processing)

---

### 9. Applied Diagnostics

#### 9.1 Prompt Engineering Audit

**Pre-Send Checklist:**

| Metric | Threshold | Action if Exceeded | Theoretical Grounding |
|--------|-----------|-------------------|----------------------|
| CDS | < 0.4 | Add explicit type bindings | D in hallucination equation too low |
| VDI | < 0.4 | Increase vocabulary density | Resolution floor too high ($\delta_{min}$ ↑) |
| T | < 0.6 | Clarify target | $I^*$ allocation unclear |
| LSS | > 1.0 | Collapse latent space | Too many implicit types |
| HLS | > 0.4 | Revise for structure | High hallucination risk |
| SCI | < 0.5 | Add scaffold connections | Competitive scaffold not engaged |

#### 9.2 Governance Filter

**Execution Gate Logic:**

```
IF HLS(prompt) > 0.5:
    REFUSE: "This prompt is structurally underspecified. 
             Please provide: [missing constraints list from diagnostic]"
ELIF LSS(prompt) > 1.0:
    WARN: "This prompt may produce hallucination. 
           Please clarify: [ambiguous tokens list from diagnostic]"
ELIF CSC(prompt) > 0.5:
    ALERT: "Collapse signature detected. 
           Please revise: [collapse metrics list]"
ELSE:
    PROCESS: Normal generation
```

#### 9.3 Collapse Detection (Real-Time Monitoring)

```
IF CSC(text_window) > 0.5:
    ALERT: "Collapse signature detected at Stage [X]"
    INTERVENTION: 
        - Narrow response scope
        - Request clarification
        - Apply constraint filters
        - Or exit and reset
```

#### 9.4 Type Hygiene Audit (from Language as a Typed System)

**Three Operations for High-Constraint Input:**

1. **Bind every variable at first use.** Check for DEF_FLOATING. If a term could resolve to multiple referents in the receiver's prior distribution, declare the intended referent.

2. **Define the operation explicitly.** Check for INFERENCE_LOAD. Summarise, analyse, compare, generate are not interchangeable. Name the operation, define its scope, declare its output format.

3. **Scan for embedded assertions.** Check for SIGNAL_INVERT, LOOP_MAGIC. A contested claim compressed into grammatical background will propagate its valence through the entire output.

---

## Part V: Why This Suite Works — Theoretical Grounding

---

### 10.1 Relationship to Hallucination Equation (Language as a Typed System)

The metrics operationalize the hallucination equation:

$$H \propto \frac{\delta}{D}$$

Where:

- **D (Constraint Density)** is measured by CDS, VDI, and C(w)
  - High D = explicit type bindings shipped
  - Low D = implicit types left for receiver's prior distribution

- **δ (Residual Schema Distance)** is proxied by:
  - LSS (Large latent space → high δ)
  - G(S) (High genericity → high δ)
  - K(S) (Low scaffold connectivity → high δ)
  - CSC (High collapse signature → high δ)
  - SDV (High drift → high δ)

### 10.2 Relationship to Typed Language Framework

The metrics reflect the type-system properties:

| Type Property | Metric Proxies | Failure Mode |
|---------------|----------------|--------------|
| Type | VDI, D(w), T(S) | DEF_FLOATING — undefined term |
| Valence | LNI, threat_weight(w) | Undeclared valence assignment |
| Scope | CDS, BF, CPR | Unbounded scope |
| Constraint | CDS, C(w), constraint types | Missing constraints |
| Relationship | DAL, IPL, SDV | Unresolved relationship |

### 10.3 Relationship to The Manifold Schema

The metrics map to manifold geometry variables:

| Manifold Variable | Metric Proxies |
|-------------------|----------------|
| $A_s^*$ (Oscillatory amplitude) | VDI, CDS |
| $R^*$ (Precision) | VDI, DAL, LNI |
| $W^*$ (Window width) | BF, SFR, IPL, IDI |
| $\Theta^*$ (Integration efficiency) | CDIC, CPR, SCI |
| $K$ (Curvature) | CSC, SDV |
| $L^*$ (Load) | CSC, LNI |
| $I^*$ (Routing) | T(S), SFR |

### 10.4 Relationship to Geometry of Inference

The metrics map to inference layers:

| Inference Layer | Metric Proxies |
|-----------------|----------------|
| Resolution Floor ($\delta_{min}$) | VDI, CDS, T(S) |
| Cache Miss Detection (LP-ACC) | BF, DAL, IPL |
| Two-Factor Gate ($C_{LR}$, $O_{pathway}$) | CPR, SCI |
| Competitive Scaffold ($W^*$) | SFR, CDIC, IDI |
| $I^*$ Investment Loop | VDI, T(S), SFR |
| Self-Sealing Loop | CSC, SDV, LSS |

### 10.5 Why This Is Different

Most approaches:
- Measure **output** quality
- Require **ground truth** for validation
- Assume hallucination is a **model property**
- Cannot predict hallucination before generation
- Focus on content rather than structure

This suite:
- Measures **input** structure
- Requires only **text** for measurement
- Assumes hallucination is a **transaction property**
- Predicts hallucination risk **before generation**
- Focuses on structural geometry

---

## Part VI: Operational Summary

---

**For Writers and Communicators:**

Every compression you send is a function call against your receiver's dictionary. Before sending high-stakes compression, audit for:

- DEF_FLOATING — key terms used without explicit binding → check VDI, CDS
- INFERENCE_LOAD — causal steps the receiver must supply → check IPL, DAL
- EMBEDDED_ASSERTION — claims compressed into grammatical background → check SDV, LOOP_MAGIC

**The diagnostic question:** "What type bindings am I assuming the receiver already holds?" Every assumption is an implicit type. Every implicit type is a synthesis instruction.

**For Prompt Engineers:**

Every prompt is a compression contract. High hallucination rate is not a model failure—it is a constraint density gap. The model's prior distribution filled type bindings you did not declare.

- If the model hallucinates on a specific term → the term was DEF_FLOATING → bind it explicitly
- If the model drifts off-topic → the scope was not declared → declare it
- If the model fabricates structure → inference load was too high → define the operation

**The fix:** LSS < 0.1, CDS > 0.6, VDI > 0.5. Shrink the latent space by giving every term a type, a referent, and a domain.

**For AI Safety:**

Guardrail misfires are type-system mismatches. A safety system that flags content the sender did not intend as harmful, or passes content the sender did intend as harmful, is applying its pre-loaded institutional dictionary faithfully. The dictionary is the variable.

- Use HLS to filter prompts before generation
- Use CSC to detect collapse signatures
- Use LSS to identify hallucination-vulnerable prompts
- Design guardrails at the constraint layer, not the behavioral layer

**For Institutional Communicators and Policy Designers:**

A policy document that does not define its key terms is not a policy. It is a compression function whose output will be determined by each receiving institution's pre-loaded dictionary. *Flexibility*, *autonomy*, *discretion*, and *agency* are not self-defining.

- Define every term that carries regulatory role assignments
- Declare what the term permits and excludes in this context
- Ship the decompression dictionary with the policy
- A document that ships its dictionary has predictable implementation

**The shared diagnostic question across all three:**

> **Before sending — what type bindings am I assuming the receiver already holds?**

Every assumption is an implicit type. Every implicit type is a synthesis instruction. Every synthesis instruction hands resolution to the receiver's prior distribution. The hallucination equation runs regardless of whether you issued the instruction deliberately. The constraint density of your input is the variable. The receiver's output is the prediction.

---

## Part VII: Quick Reference Table

| Metric | Symbol | What It Measures | Proxy For | Formula | Theoretical Grounding |
|--------|--------|------------------|-----------|---------|----------------------|
| Vocabulary Density Index | VDI | Constraint + radius + domain per token | $W^*$, $R^*$, $\delta_{min}$ | αC + βS + γD | Manifold Schema, Geometry of Inference |
| Lexical Narrowing Index | LNI | Shift toward generic/threat vocabulary | $L^*$, collapse, $W^*$ ↓ | Σ generic·threat / n | Self-Sealing Loop (Part VI) |
| Semantic Field Radius | SFR | Conceptual neighborhood width | Competitive scaffold, $W^*$ | | Geometry of Inference (Part V) |
| Constraint Density Score | CDS | Distinct constraints per sentence | D in hallucination equation | (1/n)·Σ C(w) | Typed Language, Hallucination Equation |
| Branching Factor | BF | Active conceptual threads | $W^*$, $C_s$, scaffold | Count of active threads | Manifold Schema, Geometry of Inference |
| Dependency Arc Length | DAL | Length of dependencies | $C_{LR}$, reasoning depth | Average distance | Geometry of Inference (Part III) |
| Inference Path Length | IPL | Implied steps from premise to conclusion | INFERENCE_LOAD, reasoning depth | Count of implied steps | Typed Language, Geometry of Inference |
| Constraint Propagation Radius | CPR | How far constraints propagate | $\Theta^*$, scaffold integrity | Average influence distance | Manifold Schema |
| Inference Distance Index | IDI | Conceptual displacement per information | $W^*$, cross-domain reach | VDI·R·K / (G+ε) | Geometry of Inference |
| Cross-Domain Integration Count | CDIC | Number of domains bridged | $\Theta^*$, transfer potential | Count of domains | Manifold Schema |
| Scaffold Connectivity Index | SCI | Connection to invariant scaffold | $K$, structural coherence | Σ connection strength | Manifold Schema |
| Invariant Coverage Score | ICS | Density of core invariants | Robustness, completeness | invariants_covered / total | Manifold Schema |
| Collapse Signature Composite | CSC | Joint structural deterioration | $L^*$, collapse stage, self-sealing | Σ weights·components | Geometry of Inference (Part VI) |
| Semantic Drift Vector | SDV | Meaning shift without justification | Hallucination, DEF_FLOATING | distance / justified_shift | Typed Language |
| Latent Space Size | LSS | Interpretive paths available | δ in hallucination equation | G / (C·VDI·T·K) | J-space diagnostic |
| Hallucination Likelihood Score | HLS | Structural hallucination risk | H in hallucination equation | Σ λ·(1-component) | Hallucination Equation |

---

## Appendix: Theoretical Integration

### A.1 The Complete Causal Chain

The metrics trace the full causal chain from input structure to hallucination outcome:

```
Text Input
    ↓
[VDI, CDS, T(S)] → Resolution Floor (δ_min)
    ↓
[BF, DAL, IPL] → Cache Miss Detection (LP-ACC)
    ↓
[CPR, SCI] → Two-Factor Gate (C_LR + O_pathway)
    ↓
[SFR, CDIC, IDI] → Competitive Scaffold (W*)
    ↓
[VDI, T(S), SFR] → I* Investment Loop
    ↓
[CSC, SDV, LSS] → Self-Sealing Loop
    ↓
H = δ/D → Hallucination Rate
```

### A.2 The Unified Diagnostic

Every metric is a probe into a specific layer of the inference architecture. Together they provide a complete picture of the input's structural geometry:

| If You See... | The Problem Is... | The Fix Is... |
|---------------|-------------------|---------------|
| Low VDI, low CDS | Resolution floor too high ($\delta_{min}$ ↑) | Add explicit constraints, precise terms |
| Low BF, low DAL | Gate coherence failing ($C_{LR}$ ↓) | Restore phase-locking, reduce load |
| Low SFR, low IDI | Competitive scaffold not engaged ($W^*$ ↓) | Activate outer edge, widen context |
| High LNI, high G | Self-sealing loop accelerating | Break loop with flat-geometry input |
| High LSS | Latent space too large | Bind every variable, declare every type |
| High CSC | Collapse signature present | Intervention required—upstream fix |

---

*This document formalizes the metric suite described in the companion papers: Language as a Typed System, The Manifold Schema, and Geometry of Inference. All metrics are text-only and can be computed from the input alone, without reference to ground truth, model behavior, or human judgment.*

*The metrics operationalize the hallucination equation $H \propto \delta/D$ and provide the J-space diagnostic that reveals—before generation occurs—whether a prompt is structurally hallucination-vulnerable.*

*Robinson, 2026*
