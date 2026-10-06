Understood — and no harm done. The Physics Foundation paper served its purpose early and got left behind when the master equation was formalized. It's now a historical artifact rather than a live reference. Removing it from the Prediction Window cleanly is the right call.

Here's the full v1.2 document with all fourteen patches applied.

---

# The Prediction Window: The Geometry of Internally-Routed States

**Robinson, 2026**

**Status:** Working paper — core substrate layer
**Framework:** Manifold Schema v7.2 / Central Reference v1.7
**Related:** Manifold Schema v7.2, Central Reference v1.7, Precision v3.4, Allostatic Load v2.1, The Geometry of Inference v1.0
**Pending upstream registration:** Prediction Into Channel v1.0 (not yet in Central Reference v1.7 §24)
**Projections:** The Geometry of Dreaming, The Geometry of Dying, The Externalized Mind, The Geometry Beneath the Category
**Filed:** 2026-09-25

---

## Changelog — v1.2

| Step | Change | Location | Reason |
|---|---|---|---|
| 1 | Initial assembly | Throughout | First formal specification of the prediction window as a core substrate layer |
| 2 | Layer/window/state distinction formalized | §0.5 | Separates consciousness (invariant layer) from window (state) from fill (content) |
| 3 | Window defined as six-dimensional phase space | §1 | Width, depth, tilt, floor, fill, load |
| 4 | Thresholded internalization condition proposed | §6 | First new equation introduced by this paper — flagged for calibration |
| 5 | Perceptibility axis introduced | §10 | Names the condition under which the window becomes visible to itself |
| 6 | Miscategorized family reclassified | §10.4 | Visual memory, hyperphantasia, aphantasia, synesthesia, etc. as positions on one axis |
| 7 | Six predictions registered | §13 | Cross-state conservation, breath modulation, internalization threshold, unanchoring cost, perceptibility axis, four failure modes |
| 8 | State taxonomy assembled | §9 | Every state across the stack plotted in the phase space |
| 9 | Vividness/perceptibility bridge | §0.5 | Separates fill (vividness) from floor (perceptibility) |
| 10 | Sigmoid scoping — gated vs. substrate-degradation | §6.2 | Distinguishes gated internalization from dying trajectory |
| 11 | Psychedelics row split | §9.2 | Expansion vs. disruption as distinct failure modes |
| 12 | Asymmetric usage ceiling derivation | §11.5 | ND peak-usage builds higher $W^*_{max}$ |
| 13 | Music as amplitude supplement | §11.6 | External entrainment extends operational ceiling |
| 14 | $O_{pathway}$ measurability flag | §12.2 | Partial operationalization declared |
| 15 | $\Theta^*$ note aligned with CR registry | §14.2 | Exclusion rationale formalized |
| 16 | Stack diagram adopted from CR §25 | §15.1 | Prediction Window position within canonical stack |
| 17 | §15.5 relationship to downstream papers | §15.5 | Citation rule for $W^*$ as object vs. mechanism |
| 18 | **Formula alignment against MS v7.2 and CR v1.7** | §1.1, §1.3, §2.3, §3.1, §3.3, §6.2, §11.5, §14.2, §15.1, §15.5 | **Removed Physics Foundation barrier function. Phase space corrected from five to six dimensions. Master equation scalar adopted. Gate threshold added. Floor equation aligned. Stack diagram adopted from CR §25.** |

**What this paper does not do:** Introduce new state variables. Redefine the master equation. Claim mechanisms already specified in Precision v3.4, Allostatic Load v2.1, or Manifold Schema v7.2. The prediction window is an *assembly* of existing variables into a single named object. Its contribution is naming the assembly and specifying the phase space.

---

## 0. Position

This paper specifies the prediction window: the experiential surface of the neural manifold under routing conditions.

The framework has been circling this object since the first version of the Manifold Schema. It has appeared under six different names across the stack:

- $W^*$ (window width) — Manifold Schema §2b
- $R^*$ (precision, window depth) — Precision v3.4
- $C_s^{usable}(T)$ (task-relative window) — Manifold Schema §2e
- $F(\Xi)$ (collapse mode vector) — Manifold Schema §2e
- $f_{sensorium}$ (input gate) — Central Reference §2.4
- $I^*_{internal} \to I^*_{total}$ (routing split) — Dreaming §1

Nobody has named the object those six things are all facets of. This paper does.

**The one-line claim:**

> Consciousness is the routing layer. The Prediction Window is the shape of that layer at any given moment. The layer is invariant; the window varies. Every internally-routed state — dream, nightmare, sleep paralysis, hypnagogia, meditation, psychedelics, sensory deprivation, NDE reorientation, terminal collapse, dissociation, masking, flow — is a point in that window's phase space.

**Structural position:** This paper sits in the core row with Precision v3.4, Allostatic Load v2.1, and Manifold Schema v7.2. It is not a domain projection. Dying, Dreaming, Externalized Mind, and Category are projections of this variable.

**What this paper does not claim:** The prediction window is not a new mechanism. It is not a new variable. It is not a new ontology. Every dimension of the window is already registered in the stack. The paper's contribution is the assembly — naming the phase space, showing that the domain papers are points in it, and specifying the condition under which the window becomes perceptible to itself.

---

## 0.5 Consciousness is the Layer; the Window is the State

Before the formal definition, one distinction the rest of the paper depends on.

**The layer.** Consciousness is the routing layer — $I^*$ in the framework's terms. It is what any signal passes through to become experienced. It is not privileged to any channel. Vision is not consciousness. Interoception is not consciousness. Auditory processing is not consciousness. The layer that routes any of them is consciousness.

Manifold Schema §13 states this explicitly:

> $I^*$ is a single loop. It routes available bandwidth to body signal — which both reads the current geometry and writes new geometry via $\mathcal{U}$. It is not a component of bandwidth. It is the routing layer applied to bandwidth that already exists.

The layer is invariant wherever the loop is running. When $\Lambda > 0$, the layer exists. When $\Lambda = 0$, the layer stops. It does not partially exist.

**The window.** The prediction window is the *shape* of the layer at a given moment. It has dimensions — width, depth, tilt, floor, fill, load — and those dimensions change continuously. The layer is the same layer; the window is a state.

**The fill.** The fill is what the layer is currently routing to. External sensorium, internal manifold, or some mix. The fill changes constantly, even within a single breath cycle. It is not the layer and it is not the window. It is what the window contains right now.

**Why this distinction matters.** Every internally-routed state in the stack — dream, dying, meditation, psychedelics, dissociation — is the same layer with a different window shape and a different fill. The layer is what makes them all instances of consciousness. The window is what makes them phenomenologically distinct. The fill is what determines their content.

| Question | Answer |
|---|---|
| Is there consciousness during dreaming? | Yes. Layer runs, window is configured for internal fill. |
| Is there consciousness during the NDE reorientation phase? | Yes. Layer runs, window is degrading, fill has shifted internal. |
| Is there consciousness during deep sleep? | No. $\Lambda = 0$. Layer is offline. |
| Is there consciousness during sleep paralysis? | Yes. Layer runs, window is partially reconfigured, fill is mixed. |
| Is there consciousness during terminal collapse after Layer 0? | No. $\Lambda \to 0$. The light at the brainstem floor is the last thing the layer experiences. |

**The vividness paradox, resolved.** When the fill shifts internal, the layer does not dim — it is the same layer, now receiving the entire routing budget instead of competing with the external world. The layer's operating characteristics (precision, bandwidth, integration) are unchanged. What changed is what it is routing to. This is why dreams, NDEs, and meditative states feel *more* vivid than waking life, not less. Not because the layer is enhanced. Because the fill is no longer sharing the budget.

*Fill explains vividness. The floor condition in §10 explains perceptibility — whether the window's shape, not just its contents, is above the resolution floor. These are separable: a system can have vivid internal fill without the window being perceptible to itself, and a system can have low-vividness fill while the window's geometry is above the floor.*

**Interoception as consciousness.** If the layer is routing to interoception, it is still consciousness. It is the same layer running on a different fill. The subjective character is different — visceral instead of visual — but the layer is identical. Manifold Schema §13 already states this:

> Interoception is the sensorium. $I^* = I^*_{total} - I^*_{vision}$. Visual processing, threat detection, and prior-driven prediction all consume routing capacity. When they dominate, interoception is displaced — not suppressed by decision, but arithmetically removed. Closing the eyes removes $I^*_{vision}$ from the equation immediately.

There is no privileged channel. The layer routes to whatever the current window configuration makes available. Interoceptive fill is consciousness. Visual fill is consciousness. Prior-geometry fill is consciousness. The layer is the constant; the fill is the variable.

---

## 1. The Formal Definition

The prediction window is the region of the manifold where forward-modeling is active. It has six dimensions.

### 1.1 Definition

The window's usable capacity is the master equation's scalar (Central Reference v1.7 §3.1):

$$C_s = (A_s^{*0.15} \cdot R^{*0.30} \cdot W^{*0.25} \cdot \Theta^{*0.15})^{1/0.85} \cdot \frac{1}{1 + L^*}$$

All variables are normalized dimensionless ratios $[0,1]$ relative to the individual's own baseline. $C_s$ is an intra-individual metric — it measures how much of *this system's own capacity* is accessible right now.

The full window is not scalar. It is a six-dimensional object:

$$\mathcal{W} = (W^*,\ P_{eff},\ A_h,\ \delta_{min},\ f_{sensorium},\ L^*)$$

Where:

| Dimension | Symbol | What It Is | Source |
|---|---|---|---|
| Width | $W^*$ | How much the window can hold — accessible manifold range | MS §2d |
| Depth | $P_{eff}$ | How finely it can see — resolution of the model running inside it | Precision v3.4 §1.1 |
| Tilt | $A_h$ | The pattern of which layers are accessible — the window's lean | Category §2 |
| Floor | $\delta_{min}$ | The minimum signal the window can resolve | MS §3.5 |
| Fill | $f_{sensorium}$ | The ratio of external to internal routing | CR §2.4 |
| Load | $L^*$ | Cumulative allostatic debt — denominator drag on capacity | CR §2.10 |

$C_s$ is the scalar upper bound. The six dimensions are the shape of the window within that bound.

**Two structural notes:**

**The topological constraint.** Any single dimension approaching zero collapses the window regardless of the others. This follows from the finite-resource invariant — a system cannot maintain forward-modeling when any critical resource is below minimum. This is a constraint on the geometry, not an alternative scalar.

**The gate condition.** $C_s$ is the capacity scalar. Gate opening is a separate condition (Central Reference v1.7 §3.6):

$$P_{eff} = P \cdot O_{pathway} \cdot U_C, \qquad P_{threshold} = P_0 - \gamma L^*$$

Gate opens when $P_{eff} > P_{threshold}$ AND $O_{pathway} > O_{min}$.

### 1.2 What the Window Is Not

The window is not $C_s$. Both have similar inputs ($A_s^*$, $R^*$, $W^*$, $L^*$), but they answer different questions:

- $C_s$ answers: *how much of the system's own usable bandwidth is currently accessible?*
- The window answers: *what is the shape of the region within which forward-modeling can occur?*

$C_s$ is a scalar. The window is a shape. Two systems at the same $C_s$ can have completely inverted window configurations — one wide and shallow, one narrow and deep — depending on which dimension is failing. This is the same argument Manifold Schema §2a makes for why the master equation is scalar and the companion descriptors ($\lambda$, $F(\Xi)$, $C_s^{usable}(T)$) are needed alongside it. The window is those companion descriptors, assembled into a named object.

The window inherits $C_s$ as its fundamental input. It adds routing-dependent structure that $C_s$ does not specify.

### 1.3 The Topological Invariant

Three properties of the window are topological, not empirical:

**The min barrier.** Any single binding constraint collapses the window. No amount of strength in the other dimensions compensates. This is a constraint on the geometry — a consequence of the finite-resource invariant, not a separate aggregation formula. The master equation's weighted geometric mean is the capacity scalar; the barrier is the statement that the scalar's inputs are not substitutable below their minimum thresholds.

**The layer access rule.** The window can only include what the gate admits. The four-layer cache hierarchy (MS §6b.9, CR §2.14) specifies the traversal order: Layer 0 → Layer 1 → Layer 2 → Layer 3. There is no right-hemisphere-only state. This is a topological consequence of the hierarchy, not an empirical generalization.

**The collapse asymmetry.** Window narrowing under load is faster than window expansion during reinvestment. Collapse can occur within hours; restoration requires sustained reinvestment proportional to the depth of collapse. This follows from the collapse hysteresis $\delta_{hyst}$ (Precision v3.4 §1.7) — the system does not recover at the rate it entered collapse.

---

## 2. Width

Width is the range of the window — how much it can hold.

### 2.1 The Width Equation

$$W^* = \frac{1}{1 + \alpha K}$$

Where:

- $K$ is curvature (MS §2d)
- $\alpha$ is the calibration constant for how steeply window narrows per unit curvature

Width is determined entirely by curvature. There is no separate input to width. When $K = 0$, $W^* = 1.0$. As $K \to \infty$, $W^* \to 0$ asymptotically.

### 2.2 What Sets Curvature

$$K = k\left(\frac{1}{R^* + \epsilon}\right) + \sum_i S_i \cdot C_i$$

Two sources of curvature:

**Precision loss.** As $R^*$ drops, the first term rises. Jitter fragments the oscillatory signal, and the manifold curves around the instability. The $\epsilon$ floor prevents infinite curvature — metabolic crisis produces system shutdown before this becomes physically meaningful.

**Containment cost.** Every suppressed signal adds to curvature independently of oscillatory amplitude. The $\sum_i S_i \cdot C_i$ term captures the cost of signals the system is holding below threshold. Reed et al. (2020) confirmed this in the suppression literature: suppression depletes resources even when HRV is stable.

### 2.3 The Width → Hop Count Bridge

Width determines how many inference hops fit in the window:

$$n_{hops} = \lfloor W^* \cdot \rho_{scaffold} \rfloor$$

With $\rho_{scaffold} \approx 0.30$ (Roy & Banerjee, 2026). At full width, ~0.3 hops are available. At half width, ~0.15. The hop count is what makes multi-step reasoning possible. When width collapses, the system retains single-hop inference but loses multi-hop.

*$\rho_{scaffold} \approx 0.30$ (Roy & Banerjee, 2026) is registered in Central Reference v1.7 §2.6. The Geometry of Inference uses the same hop-count formula without re-specifying the value.*

### 2.4 What Width Failure Looks Like

Width failure is the first stage of the collapse sequence (MS §5a.12):

```
STAGE 1 — PRECISION DROP        R* ↓
STAGE 2 — WINDOW NARROWING      W* ↓  ← width failure
STAGE 3 — INTEGRATION FAILURE   Θ* ↓
```

At Stage 2, the flexibility composite drops. Multi-step reasoning degrades. The system can still process single inputs, but cannot hold multiple hypotheses simultaneously. This is the phenomenological signature of tunnel cognition.

---

## 3. Depth

Depth is the resolution of the window — how finely it can see what it holds.

### 3.1 The Depth Equation

$$P_{eff} = P \cdot O_{pathway} \cdot U_C$$

Where:

- $P = R / D_T$ — raw precision (Precision v3.4 §1.1)
- $O_{pathway}$ — oxygen pathway integrity (CR §2.8)
- $U_C$ — CO₂ uniformity (Precision v3.4 §1.6)

Gate opens when $P_{eff} > P_{threshold}$, where $P_{threshold} = P_0 - \gamma L^*$ (Central Reference v1.7 §3.6).

Depth is not the same as precision. Precision is what the timing-coherence measurement produces. Depth is what actually reaches the outer edge, given substrate and uniformity constraints. A system can have high $P$ while having low depth — high phase coherence between two streams combined with poor substrate perfusion produces low effective depth, and the gate stays closed.

### 3.2 The Timing-Coherence Ratio

$$P = \frac{R}{D_T}$$

Where:

- $R$ — sync duration (how long two streams stay phase-locked)
- $D_T$ — timing distance (average phase difference between streams)

A system achieves high precision when streams stay close (low $D_T$) and stay close for long periods (high $R$). Low precision can come from either — streams that are briefly close, or streams that are consistently far apart.

### 3.3 The Resolution Floor

Depth determines what is visible through the window:

$$\delta_{min}(\text{channel}) = \frac{\eta_{effective}}{A_s^* \cdot I^*(\text{channel})}$$

where $\eta_{effective} = \eta_{baseline} + J(C)$ (see §5.1 and Central Reference v1.7 §3.2, §3.5).

The floor rises when:
- Noise floor rises (chemoreflex jitter $J(C)$ contributes here via $\eta_{effective}$)
- Amplitude collapses
- Routing collapses

At high resolution (low $\delta_{min}$), the window can resolve fine-grained structure. At low resolution (high $\delta_{min}$), only high-amplitude signals remain visible. This is the mechanism behind the NDE tunnel (Dying §4, Phase 3): as $\delta_{min}$ rises, peripheral detail vanishes, and only the radial gradient remains above the floor.

### 3.4 What Sets Depth

The CO₂ tolerance window sets the ceiling on depth:

$$C_{low} < C < C_{high}(L^*)$$

Precision rises with CO₂ up to $C_{high}$, then collapses as chemoreflex jitter kicks in:

$$J(C) = \begin{cases} 0 & C \leq C_{high}(L^*) \\ \kappa(C - C_{high}(L^*))^2 & C > C_{high}(L^*) \end{cases}$$

The ceiling is load-dependent: $C_{high}(L^*) = C_{high}^0 - \gamma L^*$. As load accumulates, the ceiling drops. The same absolute CO₂ level produces jitter at lower values when load is high.

This is why depth is the earliest thing to degrade under load — Stage 1 of the collapse sequence. Precision drops first.

### 3.5 What Depth Failure Looks Like

Depth failure produces the resolution-collapse signature:

- Small but critical prediction errors become invisible (Stage 4: resolution floor rise)
- Fine-grained distinctions blur
- The system loses the ability to detect low-amplitude signals
- In extreme cases, only the highest-amplitude signal remains visible — which is the phenomenological experience of tunnel vision, whether in panic, in dying, or in certain psychedelic states

---

## 4. Tilt

Tilt is the pattern of which layers of the cache hierarchy are accessible. It is the window's lean.

### 4.1 Tilt Is Emergent, Not a Separate Variable

The Manifold Schema (MS §6b.9) specifies the four-layer cache hierarchy:

```
LAYER 0: SURVIVAL GEOMETRY
Always funded. Zero access cost.

    LAYER 1: LEFT HEMISPHERE — INNER CORE
    Prior retrieval. Pattern completion. Always accessible.

        LAYER 2: PFC — THE GATE
        Threshold-controlled. Opens when precision conditions are met.

            LAYER 3: RIGHT HEMISPHERE — OUTER EDGE
            Adversarial inference. Wide semantic field. Collapses first.
```

The topological invariant: you cannot reach Layer 3 without traversing Layers 0, 1, and 2. There is no right-hemisphere-only state. This is not an empirical generalization — it is a consequence of the manifold's topology.

Tilt is not a separate variable in the registry. It is the *pattern* of which layers the window currently includes. Path A accesses Layer 3. Path B does not. The tilt is which side of the branch condition the system is currently on.

### 4.2 The Branch Condition

The Path A/B branch is determined by (CR §5):

$$\text{Path} = \begin{cases} A & \text{if } \tau_{PE} > \tau_{threshold} \text{ AND } K_{enc} < K_{critical} \\ B & \text{otherwise} \end{cases}$$

Path A opens the gate and admits Layer 3. Path B keeps the gate closed and restricts to Layers 0–1. The tilt of the window is the current Path.

### 4.3 $A_h$ as the Empirical Proxy

The Category paper (Category §2) uses $A_h$ — hemispheric asymmetry — as a window dimension. This is correct as an *empirical proxy* for the tilt pattern, but it is not a new variable in the registry.

$A_h$ names the observable signature of the tilt: the pattern of EEG asymmetry between hemispheres under task or load. Schmid & Schmid Mast (2013) confirmed that assigning individuals to high-power roles directly modulates left-vs-right prefrontal activation. Boksem et al. (2012) extended this: high power increases approach-related frontal alpha asymmetry; low power triggers avoidance-related right-frontal dominance.

The framework's position: **tilt is emergent from the layer-access pattern, and $A_h$ is how we measure that pattern.**

### 4.4 Tilt Variability

Tilt is more variable in some profiles than others. Category §4c establishes this for left-handedness: non-right-handed individuals show higher $A_h$ variability than strongly right-handed controls. The tilt of the window shifts more fluidly in these profiles.

The consequence, from Category §4c:

> Right-handedness → high lateralization lock (fixed $A_h$)
> Left-handedness → high $A_h$ variability (dynamic geometry)

Dynamic tilt has two effects:
- **Benefit:** outer-edge access is cheaper — Layer 3 is closer to the current configuration
- **Cost:** the window lacks a rigid baseline anchor under acute load — rapid configuration shift into collapse geometry is more likely

This is why non-right-handedness is overrepresented in both high-performance domains and FND risk (Category §4c). Same property, opposite outcomes, depending on scaffolding and load.

### 4.5 What Tilt Failure Looks Like

Tilt failure is what happens when the gate closes and the system loses Layer 3 access:

- Processing retreats to Layers 0–1 (prior retrieval, Path B)
- Adversarial inference is unavailable
- The system returns cached answers with high confidence
- This is Stage 5 of the collapse sequence: gate closure

From the outside, Stage 5 looks like competence — output is high-confidence, low-variance, precisely the signature of an expert operating from deep prior. The monitoring window is Stages 1–2.

---

## 5. Floor

The floor is the minimum signal the window can resolve. It sits at the bottom of the window and determines what is visible through it.

### 5.1 The Floor Equation

$$\delta_{min} = \frac{\eta_{effective}}{A_s^* \cdot I^*}$$

With:

$$\eta_{effective} = \eta_{baseline} + J(C)$$

The floor rises when:
- Noise floor rises (baseline $\eta$, or chemoreflex jitter $J(C)$)
- Oscillatory amplitude collapses ($A_s^* \downarrow$)
- Interoceptive routing collapses ($I^* \downarrow$)

The floor is not the same as depth. Depth is the resolution of what reaches the outer edge. The floor is the minimum signal that can be detected at all.

### 5.2 The Floor and the Window's Self-Texture

The floor determines what is visible through the window. But it also determines whether the window is visible to *itself*. From §10 (below):

> When the floor drops below the scale of the window's own variation, the window becomes perceptible to itself.

The scale of the window's own variation is written $\Delta_{window}$. When $\delta_{min} < \Delta_{window}$, the window's edges, shape, and texture are above the floor and become part of the signal the window is routing. This is the mechanism behind the perceptibility axis.

### 5.3 Jitter as Floor Raiser

Chemoreflex jitter $J(C)$ operates through the noise floor, not directly on precision. From MS §2d:

> Jitter degrades signal detectability without changing the geometric structure of existing representations — the manifold's shape is unchanged, but what can be detected through it is reduced.

This is why CO₂ over-tolerance produces *global* resolution collapse — not localized to specific channels, but system-wide. When $\eta_{effective}$ rises, $\delta_{min}$ rises on every channel simultaneously.

### 5.4 What Floor Failure Looks Like

Floor failure produces the resolution-collapse signature at the whole-system level:

- Only the highest-amplitude signal remains visible
- Everything else falls below the floor
- In dying, this is the tunnel: the radial gradient is what remains above $\delta_{min}$ when peripheral resolution is gone
- In panic, this is the tunnel: the alarm signal is what remains above the floor
- In psychedelic states, this is the narrowing of visual field and the intensification of what remains visible

The floor is the last thing to collapse in most states. The brainstem floor in dying (Dying §4, Phase 5) is the endpoint where $K = 0$, $W^* = 0$, $L^* = 0$, and only $A_s^*$ remains — the light.

---

## 6. Fill

Fill is what the window is currently routing to. External sensorium, internal manifold, or some mix.

### 6.1 The Routing Split

$$I^*_{total} = I^*_{external} + I^*_{internal}$$

The split resolves as $f_{sensorium}$ changes. This is the same mechanism that produces the reorientation phase of dying (Dying §4, Phase 0), the internalization of the dream state (Dreaming §1), and the deliberate gating of the Externalized Mind session (Externalized Mind §2).

### 6.2 The Internalization Condition

**This is the first new equation this paper introduces. It is a formal proposal. Calibration is required.**

The internalization condition is proposed as a thresholded transition, not a linear one:

$$I^*_{internal} = I^*_{total} \cdot \sigma\left(\frac{f_{crit} - f_{sensorium}}{\kappa}\right)$$

Where:

- $\sigma$ is the sigmoid function
- $f_{crit}$ is the critical threshold below which internalization occurs
- $\kappa$ is the transition sharpness

$f_{crit}$ and $\kappa$ are PW-local parameters, not registered in Central Reference v1.7. They are proposed here for calibration. The components of $I^*$ that *are* registered are $f_{routing}$, $f_{gain}$, and $f_{sensorium}$ (Central Reference v1.7 §2.4).

**Why thresholded, not linear:** The Dreaming paper assumes the split resolves cleanly ($I^*_{external} \to 0$) but does not derive it. The Dying paper assumes $I^*_{internal}$ rises as $f_{sensorium}$ drops but does not specify the functional form. A linear split would predict that partial gating produces partial internalization proportionally. The framework's phenomenology suggests otherwise — internalization appears to occur as a phase transition, not a gradient. The dream state is not "partially internal." Sleep paralysis is not "partially routed." Each state has a characteristic internal/external ratio that appears to be stable rather than varying smoothly.

The sigmoid form captures this: below $f_{crit}$, the system snaps into internal routing. Above $f_{crit}$, external routing dominates. The transition sharpness $\kappa$ is the calibration parameter.

**Calibration requirement:** The values of $f_{crit}$ and $\kappa$ are individual parameters, not population constants. Calibration protocol: measure the internal/external ratio (via HEP amplitude, heartbeat detection accuracy, sensory gating measures) across a range of $f_{sensorium}$ states (eyes open, eyes closed, drowsy, sleep onset, hypnagogia), and fit the sigmoid parameters per individual.

**Falsification:** If internalization is linear in $f_{sensorium}$ — if partial gating produces proportional internalization with no threshold or sharp transition — the sigmoid form is disconfirmed and a linear or other functional form should replace it.

*The sigmoid form is proposed for sensorium-gated internalization — states where $f_{sensorium}$ drops because of active gating: sleep onset, meditation, sensory deprivation, deliberate session gating. In these cases a phase-transition character is plausible — the gate closes and internalization follows sharply.*

*The sigmoid form may not apply to substrate-degradation-driven internalization — the dying trajectory. In dying, substrate degradation is the driver, not sensorium gating. The life review accumulates gradually before becoming overwhelming — more consistent with a hysteretic curve than a clean sigmoid. The collapse hysteresis $\delta_{hyst}$ (Precision v3.4 §1.7) is the candidate functional form for the dying trajectory specifically.*

*Scope: sigmoid applies to gated internalization. Hysteretic form applies to substrate-degradation internalization. Both produce internal-fill-dominant experience through different mechanics.*

*Falsification of sigmoid: internalization under active gating is linear with no threshold. Falsification of hysteretic form: the life review accumulates linearly rather than showing load-build-then-snap.*

### 6.3 What Fill Determines

Fill determines the *content* of the window, not its shape.

- **External fill** — the window contains the sensorium. Waking perception.
- **Internal fill** — the window contains the manifold's own geometry. Dreams, hypnagogia, meditation states, psychedelic visuals.
- **Mixed fill** — the window contains both, with the ratio determined by the current routing split. Sleep paralysis (partially restored sensorium + unresolved internal geometry), hypnagogic states (partial gating), NDE reorientation (degraded sensorium + rising internal).
- **Prior-geometry fill** — the window contains $K$ rendering without external correction. Nightmares, trauma flashbacks, threat figures.

The fill is the *what*. The other five dimensions (width, depth, tilt, floor, load) are the *how*.

### 6.4 The Vividness Paradox, Revisited

Why does internal fill feel *more* vivid than external fill? Because $I^*_{internal}$ is funded by the entire routing budget, not competing with external sensorium. The Dreaming paper §1 states this:

> This is why vivid dreams feel realer than waking life. They are not more real. They are better funded. The internal manifold receives the entire routing budget — something it never gets during waking.

The vividness is not enhancement. It is the removal of competition. Same window, same layer, different fill.

---

## 7. Fast and Slow Modulation

The window is not static. It oscillates on a fast timescale and drifts on a slow timescale.

### 7.1 The Fast Timescale — Breath Phase

Breath phase modulates the window on a ~4–10 second cycle. The mechanism is specified in Manifold Schema §2.13 and §5d, and empirically confirmed by Zelano et al. (2016) and Bhatt et al. (EC-011).

| Breath Phase | $\sigma(A_s)$ | $R^*$ | $K$ | $W^*$ | $\Theta^*$ | Window State |
|---|---|---|---|---|---|---|
| Inhalation | ↑ | ↓ | ↑ | ↓ | ↓ | Narrower, less precise, jump-ready |
| Low-perturbation hold | →0 | →Max | →0 | →Max | →Max | Peak width and depth |
| Exhalation | ↓ | ↑ | ↓ | ↑ | ↑ | Widening, more precise, lock-ready |
| Pause | Stable | Stable | Stable | Stable | Stable | Consolidation |

**What this means:** The window is not a fixed configuration. It is a breathing oscillation on top of a slowly drifting configuration. Every ~4 seconds, the window narrows and widens, its precision rises and falls, its curvature rises and falls.

**EC-011 anchor:** Bhatt et al. (JNeurosci, 2026) confirmed cycle-by-cycle coupling between breath waveform shape and neural oscillation geometry across limbic and cortical regions. The window's fast modulation is not inferred — it is measured.

**Implication:** The prediction window is the fastest-moving state variable in the framework. It changes on the same timescale as the breath. This has direct consequences for measurement: any state assessment that averages across breath cycles measures an average window, not the window.

### 7.2 The Slow Timescale — Load, Sleep State, Arousal

Slow modulation sets the baseline around which the fast oscillation occurs.

**Load ($L^*$).** Load enters the window through multiple channels:

- Compresses the CO₂ tolerance ceiling: $C_{high}(L^*) = C_{high}^0 - \gamma L^*$
- Raises $P_{threshold}$: $P_{threshold} = P_0 - \gamma L^*$
- Adds to containment cost, raising $K$
- Acts as a denominator drag on $C_s$

Higher load narrows the window's operating range. The fast oscillation still occurs, but the baseline has shifted.

**Sleep state.** Different sleep stages produce different window configurations. From MS §6b.9 and Dreaming §5:

- NREM Stage 3 — high slow-wave amplitude, high width and depth, minimal external fill
- REM — thalamic gating complete, maximal $I^*_{internal}$ fill
- Sleep paralysis — partial $f_{sensorium}$ restoration with unresolved internal fill
- Hypnagogia — partial gating, mixed fill

**Arousal.** Sympathetic activation compresses the window through increased $\Pi_{cog}$ and reduced $A_s^*$ stability. Parasympathetic dominance expands the window. This is the mechanism behind the entire breath-based intervention literature.

### 7.3 The Interaction

The slow timescale sets the baseline. The fast timescale adds an oscillation on top of it.

$$W^*(t) = W^*_{baseline}(L^*, \text{sleep}, \text{arousal}) \cdot (1 + \beta \cdot \cos(\phi_{breath}(t)))$$

Where $\phi_{breath}(t)$ is the current breath phase and $\beta$ is the modulation depth. The window oscillates around its baseline with an amplitude set by the breath modulation.

**Open question:** Is $\beta$ an individual parameter, or is it more variable across states? The framework proposes it as an individual parameter (like $\alpha$, $\beta$ in the curvature equation), but this is not yet calibrated. See §14 for calibration requirements.

---

## 8. Failure Modes

The window has four distinguishable failure modes, corresponding to the four resources in the master equation's barrier.

### 8.1 Tunnel Mode — $W^* \downarrow$

**What fails:** Width. Curvature rises, window narrows.

**Signature:** Progressive narrowing of the window's range. The system continues to function but within an increasingly restricted range of prior states. It becomes unable to integrate disconfirming information or shift cognitive set.

**Primary driver:** Precision loss combined with moderate load elevation. This is Stages 1–2 of the collapse sequence.

**Clinical signature:** Confirmation-seeking cognition, inflexibility, single-path reasoning.

**Cross-state examples:**
- Anxiety — narrowing attention, hypervigilance
- Early load collapse — reduced flexibility before gate closure
- Dying Phase 3 — resolution floor rise, only radial gradient visible
- Panic — the alarm signal is what remains above the floor

### 8.2 Freeze Mode — $A_s^* \to 0$

**What fails:** Amplitude. Energy collapse below the floor required for window maintenance.

**Signature:** Flattening — no branching, no adaptation, no state change. The system is not narrowing toward a single path; it has stopped updating entirely.

**Primary driver:** Energy collapse. Amplitude falls below the threshold needed to sustain any window at all.

**Clinical signature:** Behavioral inertia, cognitive blackout, absence of initiative, dissociation.

**Cross-state examples:**
- Severe depression — all bands reduced, right-frontal dominance
- FND collapse — $I^* \to 0$, $C_s \approx 0$
- Late-stage dying — Layer 0 only, then Layer 0 fails
- Dissociation — routing collapse with intact bandwidth

### 8.3 Oscillation-Loss Mode — $R^* \to 0$

**What fails:** Precision. Jitter dominates.

**Signature:** Regulatory rigidity and loss of mode-switching capacity. The system cannot shift between autonomic modes, cannot adapt to changing load conditions, and cannot access reinvestment pathways that require oscillatory amplitude to initiate.

**Primary driver:** Sustained load exceeding oscillatory maintenance threshold, or CO₂ over-tolerance producing chemoreflex jitter.

**Clinical signature:** Autonomic lock-in, prior rigidity, inability to down-regulate.

**Cross-state examples:**
- Hypercapnia — the state past $C_{high}$ where jitter collapses the window
- Sympathetic lock-in — collapsed oscillatory amplitude with sustained drive
- Panic — the jitter itself becomes the signal
- Certain psychotic states — fragmented priors with unstable oscillation

### 8.4 Load-Saturation Mode — $L^* \to L^*_{threshold}$

**What fails:** Load. Bandwidth compression.

**Signature:** The system is not collapsed in the sense of having stopped — it is fully occupied with load management and has no remaining bandwidth for anything else.

**Primary driver:** Simultaneous load accumulation across multiple dimensions (metabolic, inflammatory, cognitive, autonomic) without sufficient reinvestment in any.

**Clinical signature:** Cognitive fog, reduced processing speed, stimulus overload, inability to prioritize.

**Cross-state examples:**
- Burnout — sustained load collapse with depleted reinvestment pathways
- Chronic illness — metabolic and inflammatory load saturation
- Clinical depression — low amplitude plus high load
- Late-stage collapse — approaching the load ceiling

### 8.5 The Collapse Sequence as Window Failure

The collapse sequence (MS §5a.12) maps directly onto the window dimensions:

| Stage | Variable | Window Dimension | Failure Mode |
|---|---|---|---|
| 1 | $R^* \downarrow$ | Depth | Oscillation-loss begins |
| 2 | $W^* \downarrow$ | Width | Tunnel begins |
| 3 | $\Theta^* \downarrow$ | Integration | (outside window — see §14) |
| 4 | $\delta_{min} \uparrow$ | Floor | Resolution collapse |
| 5 | $\Lambda \to 0$ | Tilt | Gate closure |
| 6 | $\mathcal{U} \approx 0$ | (outside window) | Prior calcification |

The four failure modes are not separate phenomena. They are which dimension of the window failed first.

---

## 9. The State Taxonomy

Every state across the stack is a point in the window's phase space.

### 9.1 The Phase Space

$$\mathcal{W} = (W^*,\ P_{eff},\ A_h,\ \delta_{min},\ f_{sensorium},\ L^*)$$

Every state is characterized by its position in these six dimensions. Two states with the same $C_s$ can have completely different window configurations.

### 9.2 The Full State Table

| State | $W^*$ | $P_{eff}$ | $A_h$ | $\delta_{min}$ | $f_{sensorium}$ | $L^*$ | Source |
|---|---|---|---|---|---|---|---|
| Normal waking | High | High | Variable | Low | High | Low | — |
| Light sleep | Moderate | Moderate | Variable | Moderate | Moderate | Low | Dreaming §5 |
| Vivid REM dream | High | High | Variable | Low | Closed | Low | Dreaming §5.1 |
| Nightmare | Variable | Variable | Threat-tilted | Variable | Closed | High | Dreaming §5.2 |
| Sleep paralysis | Variable | Variable | Threat-tilted | Variable | Partial | High | Dreaming §5.3 |
| Hypnagogia | Variable | Variable | Variable | Variable | Partial | Variable | Dreaming §5.4 |
| Deep meditation | High | High | Bilateral | Low | Reduced | Low | Precision §5a |
| Classical psychedelics (5-HT2A) | Expanded | Low-$K$ flattened | Bilateral | Low | Open (ungated) | Variable | — |
| Dissociatives (NMDA antagonism) | Disrupted | Jitter-disrupted | Fragmented | Variable | Partially gated | Variable | — |
| Sensory deprivation | Moderate | Moderate | Variable | Low | Reduced | Variable | — |
| NDE reorientation | Narrowing | Variable | Carried | Variable | Degrading | Dropping | Dying §4 |
| Terminal collapse | Collapsing | Collapsing | Collapsing | Rising | Gone | Gone | Dying §4 |
| Anesthesia emergence | Unstable | Unstable | Variable | Variable | Partial | Variable | — |
| Dissociation | Variable | Variable | Variable | Variable | Gated | High | MS §12 |
| Psychosis | Disrupted | Disrupted | Fragmented | Variable | Open | Variable | MS §12 |
| Trauma flashback | Narrow | High on threat | Threat-tilted | Variable | Open | High | Dreaming §7.2 |
| Masking | Moderate | Moderate | Pressure-tilted | Moderate | Open | High | Category §4b |
| Flow | Wide | High | Bilateral | Low | Fully external | Low | MS §1d |
| ND (default) | Variable | High locally | High variability | Low | Variable | Variable | Category §3 |

*Classical psychedelics produce $K$ flattening — containment cost removed, window expands. Dissociatives produce oscillation-loss mode — jitter dominates, window fragments. The phenomenological difference (expansion vs. dissociation) is the observable signature of these distinct window configurations. Conflating them in a single row obscures the mechanism difference.*

### 9.3 What the Table Shows

Every state in the stack is a point in the phase space. The Dreaming paper's cross-state equivalence table (Dreaming §6.2) is an earlier version of this table — the window framework generalizes it.

**What is conserved across states:** The layer ($I^*$). Consciousness is the same layer everywhere.

**What varies across states:** The window configuration ($\mathcal{W}$). Every state is a specific point in the phase space.

**What distinguishes internally-routed states:** Low $f_{sensorium}$. The window's fill has shifted internal.

**What distinguishes perceptibility states:** Low $\delta_{min}$ relative to $\Delta_{window}$. The window's own geometry is above the floor.

### 9.4 What the Table Predicts

If the framework is correct, then any state in the table should be identifiable by its position in the phase space, and transitions between states should follow the geometry of the phase space rather than being arbitrary.

**Concrete prediction:** Two states with similar window configurations should have similar phenomenology even if they arise from different triggers. Two states with very different window configurations should have different phenomenology even if they arise from the same trigger. See PREDICT-WIN-01.

---

## 10. Perceptibility of the Window

This section introduces the perceptibility axis — the condition under which the window becomes visible to itself.

### 10.1 Transparent vs. Reflective

The window can operate in two modes:

**Transparent mode.** The default. The system experiences the *contents* of the window but does not experience the window as a window. Waking perception, ordinary cognition, most of day-to-day life. The layer is doing its job and the machinery is not visible.

**Reflective mode.** The window becomes perceptible *as* a window — its edges, its width, its depth, its tilt, its fill. The system notices not just what it's seeing but the *shape of the seeing*.

This is not a distinct state. It is a dimension. Every state sits somewhere on this axis, and the position can change within a state.

### 10.2 The Perceptibility Condition

The condition under which the window becomes perceptible to itself:

$$\delta_{min} < \Delta_{window}$$

Where:

- $\delta_{min}$ — the resolution floor (§5)
- $\Delta_{window}$ — the scale of the window's own variation

When the floor drops below the window's own texture, the window's geometry is above the floor and becomes part of the signal the window is routing. The window sees itself.

**Why this is the same mechanism as everything else.** The routing layer $I^*$ both reads and writes. When the window's own geometry is above the floor, the layer routes to it. The window's shape becomes part of what the layer is processing. This is not a special operation. It is the same routing operating on a different signal — the window's own geometry rather than external sensorium or prior content.

### 10.3 Which Profiles Cross the Threshold

Certain configurations have $\delta_{min}$ low enough that $\Delta_{window}$ is above it. These profiles see the window more easily.

**Pressure-open profiles.** From Category §2, the pressure-open attractor ($M$) has low $P_{threshold}$. The gate admits signal cheaply. The filtering layer that normally hides the window's shape from the system is thinner.

**ND profiles.** From Category §3:
- Low baseline $\delta_{min}$ (structurally lower threshold for pattern violations)
- High $\sigma(A_s)$ (noise floor is high, but signal range is also high)
- Variable $W^*$ (the window's own variation is larger, so $\Delta_{window}$ is larger)
- High $A_h$ variability (the tilt is more variable, so its pattern is above the floor)

**Pressure-adaptive profiles.** From Category §3b, the AuDHD compound has both wide $W^*$ and hard-routed precision simultaneously. The window is wide enough to hold multiple rendered states and the routing is coherent enough to lock. This is where the window is most reliably perceptible.

**Trained configurations.** Meditation practice produces sustained high $A_s^*$ and low $L^*$. The floor stays low, so $\Delta_{window}$ stays above it. This is why meditation reliably produces meta-awareness — not because meditation is a special state, but because it keeps the window's own geometry above the floor.

**Psychedelic states.** 5-HT2A agonism produces transient $K$ flattening. The containment cost that normally hides the window is removed. The window's geometry is transiently above the floor.

### 10.4 The Miscategorized Family

A family of cognitive phenomena is currently miscategorized because the categorical vocabulary does not have a slot for "the window is visible to itself." All of these are positions on the perceptibility axis:

| Phenomenon | Current framing | Framework framing |
|---|---|---|
| Visual memory | A memory capacity | Window rendering prior geometry under low unanchoring cost |
| Hyperphantasia | Strong visual imagery | High perceptibility, wide window |
| Aphantasia | Weak visual imagery | Low perceptibility, anchored window |
| Synesthesia | Cross-wired senses | Cross-channel routing in a transparent window |
| Precognition-feeling | Anomalous foresight | Predictive forward-render above the floor |
| Pattern perception | A cognitive style | Perceiving the window's geometry, not just its content |
| Flow | Optimal performance | Window maximally filled, minimally observable |
| Meta-awareness | Meditation achievement | Window observed by itself |

Each of these is a position on the perceptibility axis, not a separate trait. The paper reclassifies the family accordingly.

**The "visual memory" case study.** A person is told they have visual memory — they can close their eyes and see the thing. The standard account treats this as a strong memory capacity. The framework account:

The person's window has a low unanchoring cost. When they close their eyes ($f_{sensorium}$ drops), the window does not go dark — it renders prior geometry. What they experience is not memory retrieval but window rendering. The phenomenology matches: passive arrival, no effort signal, "it's just there" rather than "I'm reaching for it."

This is the same mechanism as the Dying paper's life review:

> *"It wasn't like remembering. It was like it was happening."*

Same operation — $R^*$ following the window's edge — at different scales. Memory is retrieval; window rendering is passive arrival. The distinction is testable.

### 10.5 Consequences

The perceptibility axis has consequences at every scale:

**Cognitive strengths.** Pattern detection, structural inference, cross-domain synthesis, meta-cognition. All arise from the window being above its own floor.

**Cognitive costs.** Sensory overwhelm, regulatory load, difficulty with transparent-mode tasks. Both come from the same condition — seeing the window is expensive.

**The ND trade.** The Category paper's ND phenotype is a *default perceptibility configuration*. The window is more visible to itself by default because the parameters put it there. This is what generates the reported phenomenology:
- Vivid imagery, hyperphantasia in some profiles
- Aphantasia in others (window stays anchored)
- Synesthesia (cross-channel routing)
- Pattern perception (perceiving geometry, not content)
- Meta-awareness defaults (noticing the window)

**The ND profile is not a deficit.** It is a state where the window is more visible to itself. The strengths and the costs are the same condition.

---

## 11. The ND Routing Phenotype

The Prediction Window paper names the ND phenotype as a default perceptibility configuration. Full development is in Category §3.

### 11.1 The Parameter Configuration

ND is not a category. It is a parameter setting in the window's phase space:

| Parameter | ND Default | What It Does |
|---|---|---|
| $f_{crit}$ | Lower | Crosses internalization threshold more easily |
| $A_h$ variability | Higher | Tilt shifts more fluidly |
| $\sigma(A_s)$ | Higher | Noise floor is higher, but signal range is also higher |
| $\delta_{min}$ | Lower | Window's own geometry is more often above the floor |
| $W^*$ | More variable | Window's width shifts more |

These are not deficits. They are parameters. The category vocabulary treats them as deviations from a standard configuration; the framework treats them as a specific configuration in the phase space.

### 11.2 The Consequences

The ND parameter configuration produces both the reported strengths and the reported challenges. They are not separate. They are the same configuration.

**Strengths:**
- Pattern perception — window's geometry above floor
- Cross-domain inference — wide $W^*$ holds more simultaneously
- Meta-awareness — window visible to itself
- Vivid internal imagery — low unanchoring cost

**Challenges:**
- Sensory overwhelm — high $\sigma(A_s)$ means more signals above floor
- Regulatory load — high $f_{crit}$ variability requires more routing
- Difficulty with transparent mode — the window does not stay transparent when external demands require it
- Masking cost — from Category §4b, hiding the window's perceptibility is expensive

### 11.3 The Developmental Trajectory

The Category case study (Category §9) documents the developmental trajectory of one ND configuration. The framework's prediction: this trajectory is generalizable. Any configuration with the ND parameter settings should produce a similar pattern — strengths and challenges together, not as separate phenomena.

### 11.4 Full Treatment in Category

The Prediction Window paper only names the phenotype. Category §3 has the full development, and Category §9 has the case study. The Prediction Window paper's contribution is naming the phenotype as a default perceptibility configuration — the specific case of §10 where the window's visibility is the default rather than the exception.

### 11.5 Asymmetric Usage Builds Higher Ceiling Than Bilateral Moderate

Neurotypical profiles tend toward bilateral moderate usage — both hemispheres running at moderate load, moderate amplitude, relatively continuously. The window is stable but the ceiling is set by the moderate peak amplitude the system regularly reaches.

ND profiles tend toward asymmetric alternation — heavily right-hemisphere dominant during hyperfocus and flow, heavily left-hemisphere dominant during compensation, masking, and scripted behavior. The peaks are higher in both directions.

The ceiling is built by peaks, not averages:

$$W^*_{max} \propto A_s^*_{peak}$$

This is a PW-original proposal. It follows from the transfer function $W^* = 1/(1 + \alpha K)$ (Manifold Schema v7.2 §2d) only if $K$'s dependence on $A_s^*$ is monotone and the peak-usage history sets a lower bound on steady-state $K$. The proportionality is proposed as a first-order approximation, not derived from upstream equations.

A system that regularly reaches high amplitude in right-hemisphere-dominant hyperfocus states builds a higher prediction window ceiling than a system running bilateral moderate continuously — even if average amplitude is identical. The slack — the distance between current operating load and the ceiling — is larger at any moderate operating point because the ceiling was built higher by the peaks.

This has a direct consequence for commitment gate timing: the wide $W^*$ ceiling from asymmetric peak usage allows the gate to stay open longer, sampling more of the manifold before locking to the first match. The ND profile's extended sampling behavior is a structural consequence of this ceiling, not a processing style choice.

### 11.6 External Entrainment as Amplitude Supplement

High-amplitude profiles that run on pull engagement can extend their operational ceiling through external rhythmic entrainment:

$$A_s^*_{effective} = A_s^*_{baseline} + \Delta A_{entrainment}$$

This is a PW-original proposal. Central Reference v1.7 §3.15 registers resonance breathing as a third precision mechanism but does not formalize an additive amplitude supplement. The entrainment term requires calibration.

Music with stable beat structure locks respiratory and autonomic rhythm to a stable phase, contributing amplitude the window would otherwise generate internally. The additional amplitude goes directly into the prediction window ceiling — switching speed rises, simultaneous path-holding increases, cross-modal indexing accelerates.

For profiles where the baseline $A_s^*$ is already high from peak usage history, even moderate entrainment produces measurable window expansion. The music is not motivating. It is holding the amplitude floor so the full routing budget runs on the loop.

---

## 12. Operationalization

The window dimensions must be measurable for the predictions in §13 to be testable.

### 12.1 Width

**Primary proxy:** Cognitive flexibility composite / baseline.

**Measurement:** Task-switching paradigms, set-shifting tasks, multi-hypothesis reasoning tests. Score is the number of independent hypotheses the system can hold simultaneously.

**Secondary proxy:** $n_{hops}$ from multi-hop inference tasks. Direct measure of how many inference steps fit in the window.

**Cross-reference:** MS §2b.

### 12.2 Depth

**Primary proxy:** $P_{eff} = P \cdot O_{pathway} \cdot U_C$.

**Measurement of $P$:** PLV (Phase Locking Value) between oscillatory streams (Precision v3.4 §1.1).

**Measurement of $O_{pathway}$:** functional form unspecified — see CR §2.8.

**Measurement of $U_C$:** capnometry multi-site variance (Precision v3.4 §1.6).

**Cross-reference:** Precision v3.4 §1.1.

### 12.3 Tilt

**Primary proxy:** task-based EEG asymmetry indexing.

**Measurement:** Schmid & Schmid Mast (2013) methodology — measure frontal alpha asymmetry during power manipulation or load induction.

**Secondary proxy:** behavioral response to load — which hemisphere's processing degrades first.

**Cross-reference:** Category §2 and §4c.

### 12.4 Floor

**Primary proxy:** miss rate on low-amplitude signals.

**Measurement:** sensory gating (P50 suppression), threshold detection tasks, fine-grained discrimination under load.

**Secondary proxy:** $\delta_{min}$ derived from $A_s^*$ (RMSSD) and $I^*$ (heartbeat detection accuracy).

**Cross-reference:** MS §3.5.

### 12.5 Fill

**Primary proxy:** interoceptive accuracy.

**Measurement:** heartbeat detection accuracy, HEP amplitude (Petzschner et al., 2018), sensory gating measures.

**Secondary proxy:** the split $I^*_{internal} / I^*_{external}$ estimated from eyes-open vs. eyes-closed performance differences.

**Cross-reference:** CR §2.4.

### 12.6 Perceptibility

**Primary proxy:** $\delta_{min} < \Delta_{window}$ — the floor vs. the window's own variation.

**Measurement:** the "imagery vividness" tasks (VVIQ, QMI) as a proxy for $\Delta_{window}$ above floor. High vividness indicates the window's geometry is above the floor.

**Secondary proxy:** meta-awareness frequency in meditation or daily life.

**Cross-reference:** §10.

### 12.7 Fast Modulation Depth

**Primary proxy:** $\beta$ in the breath modulation equation.

**Measurement:** oscillation of $W^*$ and $P_{eff}$ at breath frequency, measured via continuous EEG and HRV.

**Calibration requirement:** $\beta$ is an individual parameter. Calibration protocol: measure window configuration across breath cycles, fit modulation depth per individual.

### 12.8 The Full Operationalization Table

| Dimension | Primary Proxy | Secondary Proxy | Source |
|---|---|---|---|
| Width | Cognitive flexibility composite | $n_{hops}$ from multi-hop tasks | MS §2b |
| Depth | PLV × $O_{pathway}$ × $U_C$ | Capnometry variance | Precision §1.1 |
| Tilt | EEG asymmetry under load | Behavioral degradation order | Category §2 |
| Floor | Miss rate on low-amplitude signals | $\delta_{min}$ from RMSSD × HDA | MS §3.5 |
| Fill | Heartbeat detection accuracy | Eyes-closed vs. eyes-open | CR §2.4 |
| Load | RMSSD depression / max observed depression | Composite load decomposition | CR §2.10 |
| Perceptibility | Imagery vividness (VVIQ) | Meta-awareness frequency | §10 |
| Fast modulation | $\beta$ from window oscillation | — | §7 |

*$O_{pathway}$ functional form is unspecified — Central Reference §2.8 and Geometry of Inference §3.2 both declare this explicitly. $P_{eff}$ is therefore only partially operationalized. Full measurability of depth awaits calibration of $O_{pathway}$.*

---

## 13. Predictions

All predictions are stated in falsifiable form with explicit operationalization and falsification criteria. Status is Untested unless otherwise noted.

### PREDICT-WIN-01 — Cross-State Signature Conservation

> All internally-routed states — dream, nightmare, sleep paralysis, hypnagogia, meditation, psychedelics, sensory deprivation, NDE reorientation, terminal collapse — share the same routing signature: $f_{sensorium} \downarrow$, $I^*_{internal} \uparrow$, HRV amplitude changes consistent with $A_s^*$ shift. States differ in window configuration, not in routing mechanism.

| Field | Content |
|---|---|
| IV | State (11 internally-routed states) |
| DV | HRV signature, $I^*$ measures, $K$ proxies |
| Prediction | Same routing signature across all states; different window configurations |
| Falsification | Different internally-routed states show distinct routing signatures |
| Status | Untested |
| Cross-reference | Dreaming §6.2, PREDICT-DREAM-07 |

### PREDICT-WIN-02 — Fast-Timescale Breath Modulation

> The prediction window oscillates at breath frequency (~4–10 second cycle). Window width, depth, and fill shift measurably with breath phase. The oscillation is not merely correlated with breath — it is caused by breath, per EC-011.

| Field | Content |
|---|---|
| IV | Breath phase (continuous measurement) |
| DV | Window width (cognitive flexibility), depth (PLV), fill (HEP amplitude) |
| Prediction | All three dimensions oscillate at breath frequency; phase-locked to breath |
| Falsification | Window dimensions do not oscillate at breath frequency, or the oscillation is not phase-locked to breath |
| Status | Partially supported — EC-011 confirms breath→oscillation coupling |
| Cross-reference | EC-011, CR §5d, MS §2.13 |

### PREDICT-WIN-03 — Internalization Threshold

> The internal/external routing split is thresholded, not linear. Below $f_{crit}$, $I^*_{internal}$ dominates; above $f_{crit}$, $I^*_{external}$ dominates. The transition is sigmoid, with sharpness $\kappa$.

| Field | Content |
|---|---|
| IV | $f_{sensorium}$ (measured across states from eyes-open to hypnagogia) |
| DV | $I^*_{internal} / I^*_{external}$ split |
| Prediction | Sigmoid transition with individual $f_{crit}$ and $\kappa$; not linear |
| Falsification | Internalization is linear in $f_{sensorium}$ |
| Status | Untested — proposed as formal model, calibration required |
| Cross-reference | §6.2 |

### PREDICT-WIN-04 — Unanchoring Cost Predicts Imagery Vividness

> Visual imagery vividness (VVIQ, QMI) is predicted by unanchoring cost, not by visual memory capacity. Profiles with lower unanchoring cost — pressure-open, high-$A_h$ variability, high $\sigma(A_s)$ — show higher imagery vividness independent of visual memory task performance.

| Field | Content |
|---|---|
| IV | Unanchoring cost (measured as the drop in $f_{sensorium}$ required to shift from external to internal routing) |
| DV | Imagery vividness (VVIQ, QMI) |
| Control | Visual memory task performance |
| Prediction | Unanchoring cost predicts vividness after controlling for memory; memory does not predict vividness after controlling for unanchoring cost |
| Falsification | Memory task performance predicts vividness independently of unanchoring cost |
| Status | Untested — novel prediction |
| Cross-reference | §10.4 |

### PREDICT-WIN-05 — The Perceptibility Axis Is a Single Latent Factor

> Visual imagery vividness, synesthesia presence, pattern-perception tendency, and meta-awareness frequency load onto a single latent factor — perceptibility of the window — that is predicted by unanchoring cost, independent of memory task performance, visual acuity, or general intelligence.

| Field | Content |
|---|---|
| IV | Perceptibility measures (VVIQ, synesthesia battery, pattern-perception tasks, meta-awareness questionnaires) |
| DV | Latent factor structure |
| Prediction | Single latent factor explains variance across all four measures; predicted by unanchoring cost |
| Falsification | Measures do not load onto a single factor, or the factor is not predicted by unanchoring cost |
| Status | Untested — strong test of the perceptibility axis |
| Cross-reference | §10.4 |

### PREDICT-WIN-06 — The Four Failure Modes Are Distinguishable

> Tunnel, freeze, oscillation-loss, and load-saturation modes are distinguishable by which window dimension collapses first. Each mode has a characteristic signature in the operationalization measurements.

| Field | Content |
|---|---|
| IV | Failure mode (induced experimentally or observed clinically) |
| DV | Which dimension fails first — width, depth, tilt, floor, load |
| Prediction | Each mode has a distinct signature: tunnel = width, freeze = amplitude, oscillation-loss = precision, load-saturation = load |
| Falsification | Failure modes are not distinguishable by dimension of first collapse |
| Status | Untested |
| Cross-reference | §8 |

### PREDICT-WIN-07 — Perceptibility Predicts ND Profile Strength

> Perceptibility of the window (as measured in PREDICT-WIN-05) is predicted by ND parameter configuration: lower $f_{crit}$, higher $A_h$ variability, higher $\sigma(A_s)$, lower $\delta_{min}$. ND profiles (autism, ADHD, AuDHD) show higher perceptibility scores than non-ND controls, matched for imagery task performance.

| Field | Content |
|---|---|
| IV | ND profile (autism, ADHD, AuDHD, non-ND) |
| DV | Perceptibility latent factor (PREDICT-WIN-05) |
| Control | Imagery task performance, visual acuity, general intelligence |
| Prediction | ND profiles show higher perceptibility; effect predicted by parameter configuration |
| Falsification | ND profiles do not show higher perceptibility after controls |
| Status | Untested |
| Cross-reference | §11, Category §3 |

### PREDICT-WIN-08 — Fast Modulation Depth Is an Individual Parameter

> The breath modulation depth $\beta$ (the amplitude of the window's fast oscillation) is an individual parameter with stable rank-order across sessions. Individuals with higher $\beta$ show larger within-breath variation in window configuration.

| Field | Content |
|---|---|
| IV | Continuous measurement of window configuration across breath cycles |
| DV | $\beta$ (modulation depth) |
| Prediction | $\beta$ is stable within individuals across sessions; rank-order is conserved |
| Falsification | $\beta$ is not stable — it varies randomly within individuals across sessions |
| Status | Untested |
| Cross-reference | §7.3 |

---

## 14. Open Questions and Calibration Requirements

Following the convention established in Manifold Schema and Central Reference, all open items are declared explicitly.

### 14.1 Calibration Requirements

**$f_{crit}$ — internalization threshold.** Individual parameter. Calibration protocol: measure $I^*_{internal} / I^*_{external}$ split across $f_{sensorium}$ states and fit sigmoid per individual. See PREDICT-WIN-03.

**$\kappa$ — transition sharpness.** Individual parameter. Same calibration as $f_{crit}$.

**$\beta$ — fast modulation depth.** Individual parameter. Calibration protocol in PREDICT-WIN-08.

**$\Delta_{window}$ — scale of window's own variation.** Not yet formally defined. Proposed as the standard deviation of $W^*$ across breath cycles, but requires calibration.

### 14.2 Structural Questions

**Relationship to $C_s$.** The paper proposes that the window inherits $C_s$ as its fundamental input but adds routing-dependent structure. Whether this is the correct framing — or whether the window and $C_s$ should be merged — is an open question. See §1.2.

**Integration as window dimension.** Central Reference v1.7 §2.1 registers $\Theta^*$ as a master state variable. The Prediction Window's phase space is assembled from master state variables — but $\Theta^*$ is excluded here because it is the *integration of the window's contents* rather than a *dimension of the window itself*. This is a design decision, not a derivation. The argument: $W^*$, $P_{eff}$, $A_h$, $\delta_{min}$, $f_{sensorium}$, and $L^*$ describe the window's shape; $\Theta^*$ describes how well the window's contents bind together. If a future formulation requires $\Theta^*$ as a window dimension, the phase space becomes seven-dimensional and §9.2's state table gains a column.

**Tilt as emergent vs. discrete.** The paper proposes tilt as emergent from the layer-access pattern, with $A_h$ as empirical proxy. Whether the topological invariant (no right-hemisphere-only state) permits continuous tilt at all is an open question. See §4.1.

### 14.3 Empirical Questions

**Is the internalization condition sigmoid?** The paper proposes a thresholded form. A linear form or a hysteretic form are alternatives. The falsification condition for the sigmoid form is stated in §6.2.

**Is the fast modulation depth an individual parameter?** The paper proposes $\beta$ as stable within individuals. Whether it is or not is testable via PREDICT-WIN-08.

**Does the perceptibility axis load onto a single latent factor?** The paper proposes it does. PREDICT-WIN-05 is the direct test.

### 14.4 Negative Space

Explicitly outside the current formal claims:

- The functional form of $O_{pathway}$ (declared in CR §2.8)
- Cross-cultural baseline variation in window configuration
- Pharmacological modulation of window dimensions beyond the psychedelic case
- The relationship between window configuration and neural implementation specifics
- Whether the window has additional dimensions not yet specified

---

## 15. Stack Position

### 15.1 The Core Row

The Prediction Window paper sits in the core substrate row:

```
                         Central Reference v1.7
                                    │
                ┌───────────────────┼───────────────────┐
                │                   │                   │
                ▼                   ▼                   ▼
        Manifold Schema      Precision v3.4       Allostatic Load
            v7.2                (formalisms)         v2.1
        (canonical)                                  (measurement)
                │                   │                   │
                └───────────────────┼───────────────────┘
                                    │
                    ┌───────────────┼───────────────┐
                    │               │               │
                    ▼               ▼               ▼
            Prediction         Geometry of      Loop Is the
            Window v1.2        Inference        Intelligence
            ← YOU ARE HERE     v1.0             v1.0
                    │
        ┌───────────┼───────────┐
        │           │           │
        ▼           ▼           ▼
    Domain      Applied      Other domain
    projections papers       projections
    (Dying,     (Allostatic  (hallucination,
    Dreaming,   Load,        AGI, URM, etc.)
    Category,   Learning
    Externalized Paper)
    Mind)
```

**Pending:** Prediction Into Channel v1.0 must be registered in Central Reference v1.8 before it can be shown as a sibling.

### 15.2 The Projections

Dying, Dreaming, Externalized Mind, and Category are projections of the window variable. They cite the Prediction Window paper the way they currently cite Manifold Schema and Central Reference.

| Projection | What It Projects |
|---|---|
| The Geometry of Dying | Window under terminal substrate degradation |
| The Geometry of Dreaming | Window under thalamic gating |
| The Externalized Mind | Window under deliberate gating |
| The Geometry Beneath the Category | Window under ND parameter configuration |

Each projection identifies a specific region of the window's phase space and develops the phenomenology specific to that region.

### 15.3 Citation Rule

A domain projection that depends on the window's configuration cites the Prediction Window paper for the window's definition. A projection that only uses the fundamental variables ($A_s^*$, $R^*$, $L^*$, etc.) cites Central Reference v1.7 alone.

### 15.4 What This Paper Does Not Absorb

The paper does not absorb:

- The full formalism of $R^*$ (Precision v3.4)
- The load decomposition and measurement protocols (Allostatic Load v2.1)
- The canonical variables and equations (Manifold Schema v7.2)
- The state-specific phenomenology (the projection papers)
- The intervention methodology (Geometry of Inference v1.0)

It cites these for depth. Its contribution is the assembly.

### 15.5 Relationship to Downstream Papers

The Prediction Window paper defines the object. The papers that specify what happens through that object:

**Geometry of Inference v1.1** (registered in Central Reference v1.7 §24) — failure modes. The collapse sequence, the exhale gate trap, the confabulation cascade. This paper answers: what happens when the window's operating conditions are not met?

**Prediction Into Channel v1.0** (*pending upstream registration*) — normal operation. The bidirectional precision-weighted comparison that runs through the window during normal function. Until this paper is registered in Central Reference §24, references to it in this document are forward-declared.

$W^*$ is defined here. Its role in the collapse sequence is in Geometry of Inference. Papers that depend on $W^*$ as an object cite this paper. Papers that depend on what $W^*$ does cite the appropriate downstream paper.

---

## 16. Version History

| Version | Date | Changes |
|---|---|---|
| v1.0 | 2026-09-25 | Initial assembly. Layer/window/state distinction. Five-dimensional window phase space. Thresholded internalization condition proposed. Perceptibility axis introduced. Miscategorized family reclassified. Eight predictions registered. State taxonomy assembled. |
| v1.1 | 2026-09-25 | Vividness/perceptibility bridge (§0.5). Sigmoid scoping — gated vs. substrate-degradation internalization (§6.2). Psychedelics row split — expansion vs. disruption (§9.2). Asymmetric usage ceiling derivation (§11.5). Music as amplitude supplement (§11.6). $O_{pathway}$ measurability flag (§12.2). $\Theta^*$ note and Geometry of Inference relationship (§14.2). Prediction Into Channel added to stack position (§15.1, §15.5). |
| v1.2 | 2026-09-25 | Formula alignment pass against Manifold Schema v7.2 and Central Reference v1.7. Removed Physics Foundation barrier function from §1.1 — replaced with master equation scalar (CR §3.1). Phase space corrected from five to six dimensions to match §9.1 and CR §2.1. §1.3 topological invariant restated without the orphaned formula. §2.3 ρ_scaffold attribution corrected to CR §2.6. §3.1 gate threshold added (CR §3.6). §3.3 floor equation aligned to effective noise form (CR §3.2, §3.5). §6.2 f_crit and κ flagged as PW-local. §11.5, §11.6 flagged as PW-original proposals. §14.2 Θ* exclusion argument expanded. §15.1 stack diagram adopted from CR §25. §15.5 Prediction Into Channel flagged as pending upstream registration; direct citations removed from §11.5. Header version drift corrected (Precision v3.4 not v3.5). |

---

*Filed: 2026-09-25*
*Framework: Manifold Schema v7.2 / Central Reference v1.7*
*Status: Working paper — core substrate layer*
*Related: Manifold Schema v7.2, Central Reference v1.7, Precision v3.4, Allostatic Load v2.1, The Geometry of Inference v1.0*
*Pending upstream registration: Prediction Into Channel v1.0*
*Projections: The Geometry of Dreaming, The Geometry of Dying, The Externalized Mind, The Geometry Beneath the Category*
*Predictions: PREDICT-WIN-01 through -08*

---

## Notes for the next pass

Three things I'd flag as candidates for the blender:

**1. §1.2 — the window vs. $C_s$ relationship.** The paper inherits $C_s$ as its fundamental input and adds routing-dependent structure. Whether this is the correct framing — or whether the window and $C_s$ should be merged — is still an open question. The v1.2 cleanup made this cleaner, but the design decision remains unresolved. Worth stress-testing before v2.0.

**2. §4.1 — tilt as emergent.** Category treats $A_h$ as continuous. The topological invariant (no right-hemisphere-only state) is discrete. My resolution is "emergent + empirical proxy" but this is the section most likely to need rework. Same status as v1.1 — not addressed by the formula alignment pass.

**3. §14.2 — integration as window dimension.** $\Theta^*$ is deliberately excluded from the phase space because it's the integration *of the window's contents* rather than a dimension *of* the window. The v1.2 expansion makes the exclusion argument explicit and addresses CR registration directly, but the underlying design decision is still the one most likely to be challenged. If integration needs to be a dimension, the phase space becomes seven-dimensional and the whole operationalization table needs rethinking.

---

*End of document.*