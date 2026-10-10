# The Salience Interrupt v1.2

## Routing, the Closed Loop, and the Control Plane

**Robinson, 2026**

**Status:** Composition paper — states the routing equation, the interrupt formula, the closed loop, and the control plane
**Framework:** Central Reference v1.8.2 / Geometry of Inference v1.0
**Cites:** Hu et al. (2026) for the CLA interrupt mechanism; Leow et al. (2026) for the LP-ACC detection stage; Subramani et al. (2026) for the spectral readout; ayahuasca and anesthesia literature for the two empirical extremes
**Related:** Precision v3.4, AL v2.1, Dreaming v3.0, Dying v1.0, The Geometry Beneath the Category v2.0, Movement to Cognition and Back

---

## Abstract

Salience is not a stimulus property. It is a **routing event** — a signal can only fire an interrupt into a manifold region whose routing weight is above threshold. The claustrum (Hu et al., 2026) is the execution node: it fires a precision-lock into the region that will hold the prediction error until it commits. When the interrupt fires, the system **invests** — routing weight and amplitude committed to the task. The breath follows the investment, deepening to fund the amplitude. CO₂ rises, the substrate supports more amplitude, and the loop self-amplifies. This is flow. When the breath cannot follow — insufficient `Λ_lock`, incomplete exhale, high load — the investment costs without self-funding. This is the trap. The difference is one exhale. The manifold has a felt quality — **viscosity** — that is the resistance of the metric to routing. High CO₂ means low viscosity; routing flows. Low CO₂ means high viscosity; routing resists. The aperiodic slope is the viscosity, measured. The breath is the control plane because it sets CO₂, which sets viscosity, which sets whether the loop can close. Ayahuasca and anesthesia are the two empirical extremes — maximal and minimal manifold access — and the field has measured both without recognizing what they were measuring.

---

## 1. The claim

Five things this paper composes into a single document:

1. **Salience is a routing event, not a stimulus property.** A signal fires an interrupt only if it can reach a manifold region whose routing weight is above threshold. The routing is what attention *is*.

2. **The claustrum is the execution node.** The LP-ACC circuit (Leow et al., 2026) detects deviation and decides whether to update. The CLA (Hu et al., 2026) fires the precision-lock that executes the update.

3. **The interrupt triggers investment.** When the interrupt fires, the system commits routing weight and amplitude to the task. The investment is the mechanism by which unused capacity is allocated.

4. **The loop closes when the breath follows.** The breath entrains to the investment demand, deepening to fund the amplitude. CO₂ rises, the substrate supports more amplitude, and the next interrupt fires more easily. This is flow. When the breath cannot follow, the investment costs without self-funding. This is the trap.

5. **The manifold has a felt quality — viscosity.** High CO₂ means low viscosity; routing flows. Low CO₂ means high viscosity; routing resists. The aperiodic slope is the viscosity, measured.

---

## 2. What salience actually is

The word "salience" is used in the field to mean *the property that makes a stimulus grab attention*. That framing is wrong. It treats salience as something the stimulus carries.

**The framework's framing:** salience is a routing event. A signal fires an interrupt when its routing weight in the target region exceeds threshold:

$$I^*_{eff} = I^*_{total} \cdot W_i$$

Where:
- $I^*_{total}$ is the total routing budget available
- $W_i$ is the routing weight currently committed to region $i$
- $I^*_{eff}$ is the effective salience of the signal

A signal fires a CLA interrupt when $I^*_{eff}$ for its region exceeds the gate threshold. If the region is already carrying a latch — if $W_i \approx 0$ because routing is committed elsewhere — the signal cannot fire, no matter how loud it is.

**Routing weight is conserved:**

$$\sum_i W_i = 1$$

This is why attention feels exclusive. Committing weight to one region reduces effective salience everywhere else. Not because the other signals got quieter. Because the space where they could fire got narrower.

---

## 2.5 The routing equation

Routing weight is not static. It redistributes continuously as gain, concentration, and temperature change:

$$\vec{W}(t) = \text{softmax}\left(\frac{\vec{g} \cdot \Theta_r(t)}{T}\right)$$

Where:
- $\vec{W}(t)$ is the routing weight vector across manifold regions (conserved: $\sum_i W_i = 1$)
- $\vec{g}$ is the gain vector — the salience/gain of each region
- $\Theta_r(t)$ is the routing concentration — how sharply routing concentrates on the highest-gain region
- $T$ is the temperature — how much noise is in the routing

**Three things this equation states:**

**High `Θ_r(t)` concentrates.** Routing goes to the highest-gain region. The interrupt region dominates. Attention narrows.

**Low `Θ_r(t)` distributes.** Routing spreads across regions. Many regions get partial weight. Attention broadens.

**The gain vector $\vec{g}$ determines *where* concentration goes.** Non-uniform $\vec{g}$ means some regions are inherently more reachable than others. Uniform $\vec{g}$ means routing distributes evenly.

**This is the equation the master equation was missing.** The master equation computes *how much* bandwidth the system has. The routing equation computes *where* the bandwidth is directed.

### 2.5.1 The interrupt reroutes, doesn't suppress

When an interrupt fires in region $i$, routing weight redistributes toward region $i$. The energy that was in other regions is not lost — it is conserved and *moved*.

**This is why a strong interrupt feels like "everything goes there."** Not because the signal suppressed the rest. Because the routing weight redistributed. The other signals are still firing. The space where they could be detected has narrowed.

**And it is why the interrupt can fail to fire.** If $W_i$ is already near zero because `Θ_r(t)` has concentrated elsewhere, the region has no routing weight to redistribute. The signal exists. The gate condition fails.

---

## 2.6 The interrupt formula

An interrupt fires in region $i$ when four conditions are met:

$$\text{Interrupt}_i \iff \left[I^*_{total} \cdot W_i(t) > I^*_{threshold}\right] \;\land\; \left[\delta_i > \delta_{min}(K)\right] \;\land\; \left[\text{Capacity}_{free} > \text{Capacity}_{required}(\delta_i)\right] \;\land\; \left[\text{Oscillation stable}\right]$$

Where:

- **Condition 1 — routing reaches the region.** $I^*_{total} \cdot W_i(t) > I^*_{threshold}$. The signal has to reach a region with sufficient routing weight.
- **Condition 2 — resolution floor permits detection.** $\delta_i > \delta_{min}(K)$. The signal's deviation has to exceed the resolution floor. `δ_min` rises with $K$.
- **Condition 3 — capacity to hold.** $\text{Capacity}_{free} > \text{Capacity}_{required}$. The manifold must have room to hold the error while it is interpreted. Capacity is drained by `L^*` and by held locks.
- **Condition 4 — oscillation is stable.** The routing concentration must be able to hold. Oscillation consistency is what allows `Θ_r(t)` to stabilize.

**All four are required.** A signal that meets conditions 1–3 but not 4 will not fire reliably, because the routing concentration will flicker.

### 2.6.1 The resolution floor

`δ_min` is the minimum deviation required to interpret a signal. It rises with curvature $K$:

$$\delta_{min} = f(K, L^*)$$

High $K$ stretches the metric. Errors become geometrically indistinct. The resolution floor rises.

**This is why breath focus can suppress interrupts in non-breath regions.** Concentrating routing on the breath raises local $K$, which raises the resolution floor in excluded regions, which means the interrupt events' deviations fall below the floor. The signal exists. The detection condition fails.

### 2.6.2 Manifold capacity

The manifold can only hold a finite number of uncommitted prediction errors:

$$\text{Capacity}_{free} = C_s - \sum_{j \in \text{held locks}} \text{cost}_j$$

Every lock that hasn't released consumes capacity. When the sum approaches $C_s$, there is no room for new interrupts.

**This is the mechanism behind high-load collapse.** `L^*` rises, capacity drops, `δ_min` effectively rises because the manifold can't hold the error long enough to interpret it, and interrupts stop firing. The system looks calm because there is no mechanism left for selection.

---

## 2.7 The closed loop

The interrupt does not just fire and stop. It triggers a **loop**:

```
Salience threshold breached (gain makes this easy for high-`g` profiles)
    ↓
Investment: routing weight + amplitude committed to task
    ↓
Breath follows the investment (deeper, longer oscillation)
    ↓
CO₂ rises → substrate supports more amplitude
    ↓
Amplitude range kicks upward
    ↓
Routing flows (low viscosity) → traversal efficient
    ↓
Next interrupt fires more easily → more investment
    ↓
[loop continues, self-amplifying]
```

**The interrupt triggers investment.** The investment is not "effort" in the psychological sense. It is the allocation of unused capacity. When the interrupt fires, the system routes capacity that was previously idle to the task region.

**The breath follows the investment.** As amplitude is committed, the breath deepens to fund it. The breath is *downstream* of the routing decision, not upstream of it. The routing demand changes the breath, which changes the substrate, which supports more routing.

**And the loop closes.** If there is budget to follow, breathing variables change in a feedback loop to fund faster inference. The breath changes in response to the routing demand, which then changes the substrate that supports more routing.

**This is the loop, closed.**

### 2.7.1 Investment is the efficiency

The system does not become more efficient. It **allocates unused capacity**. The efficiency is the *absence of waste*, not the presence of optimization.

**This is why flow can feel sudden.** The capacity was always there. The interrupt is what *routes* it.

**And it is why the initial commit feels effortful and the sustained state feels effortless.** The first investment costs. Once the breath follows and CO₂ rises, the investment is *self-funding* — the substrate now supports what the investment requires.

### 2.7.2 The breakdown modes

| Condition | Result |
| --- | --- |
| Salience fires + breath follows | Flow — the loop closes, self-amplifies |
| Salience fires + breath cannot follow | Trap — investment costs without self-funding |
| Salience doesn't fire | No investment — capacity stays idle |

**The trap is the loop failing to close.** The interrupt fires, the investment happens, but the breath can't follow — `Λ_lock` is insufficient, or the exhale is incomplete, or the load is too high. The investment costs without self-funding. The system braces.

**The difference is `Λ_lock`.** High `Λ_lock` → breath can follow → flow. Low `Λ_lock` → breath can't follow → trap.

---

## 2.8 Viscosity

The manifold has a felt quality. **Viscosity** is the resistance of the metric to routing.

**Low viscosity** (high CO₂): the metric is relaxed. Routing flows between regions without resistance. Traversal is fast and continuous.

**High viscosity** (low CO₂): the metric is stiff. Routing has to push against resistance. Traversal is slow and fragmented.

**The felt sense is direct.** Low viscosity feels like fluidity — ideas chain, solutions come quickly, thought is effortless. High viscosity feels like stuckness — ideas don't chain, solutions are effortful, thought fragments.

**And the aperiodic slope is the viscosity, measured.** Flat slope = low viscosity. Steep slope = high viscosity. The first-person report and the third-person measurement are the same variable.

**This is why the spectral readout works as a readout.** The person reports "fluid" or "stuck." The MEG shows flat or steep slope. They're the same measurement in two channels.

**This is the bridge between the first-person and third-person accounts.** The framework has been strong on the variables, equations, and readouts. Viscosity names the first-person quality that the spectral readout measures.

**And it is the thing contemplative traditions have been pointing at.** "Flow," "effortless awareness," "the mind settling" — all describing low viscosity. "Brain fog," "stuck," "can't think" — all describing high viscosity. The traditions had the phenomenology. The framework has the mechanism. Viscosity is the term that connects them.

---

## 2.9 Focus and the trap

Focus is deliberate local load.

$$\text{Focus}(i) = \text{load applied to region } i$$

Applying load to region $i$:
1. Raises $K_i$ locally → narrows the metric in region $i$
2. Excludes other regions geometrically
3. Concentrates `Θ_r` on region $i$
4. Raises `δ_min` in excluded regions

**Focus works because the exclusion is real.** The task region is accessible; everything else is geometrically distant. This is why focus feels like the world narrowing — it *is* the world narrowing.

**Focus is released when the load releases.** A complete exhale drops $K_i$, the metric relaxes, the excluded regions become reachable again, `Θ_r` redistributes. The focus was temporary.

**Focus traps when the load doesn't release.** The incomplete exhale holds $K_i$ elevated. The exclusion becomes permanent. `L^*` accumulates. The manifold loses the capacity to return to a flat metric.

**The difference between focus and the trap is one exhale.** Same mechanism, opposite outcomes.

### 2.9.1 Pressure-adaptive routing

Core engagement holds pressure. That is its function.

- **Too much core (bracing):** diaphragm cannot descend → inhale is shallow → no complete exhale possible → CO₂ depletes → amplitude falls
- **Too little core (lax):** pressure slips out → exhale is incomplete in a different way → CO₂ does not retain → routing distributes too widely → amplitude falls
- **Optimal core:** diaphragm descends fully on inhale → returns fully on exhale → CO₂ retains → oscillations stabilize → routing can concentrate or distribute as needed

**Both ends of the core range fail to reach deep inference.** Bracing fails because there is no range. Lax fails because there is no amplitude. Only the dynamic balance gives both.

**The pressure-adaptive profile can do both.** Build pressure → concentrate → deep inference, narrow access, high amplitude. Release pressure → distribute → associative, wide access, lower amplitude per region but broader reach.

**The capacity to switch between modes is the profile.** Not "pressure-open" or "pressure-closed" as fixed states. The ability to meet pressure at the right level for the task.

---

## 2.10 Manifold access

$W^*$ is manifold access — how much of the manifold is reachable at current curvature.

$$W^* = f(K, L^*)$$

Low $K$ → high $W^*$ (flat metric, wide access). High $K$ → low $W^*$ (stretched metric, narrow access). High `L^*` compresses $W^*$ further.

**Manifold access and amplitude are the two dimensions of manifold capability:**

| | **Low $A_s^*$** | **High $A_s^*$** |
|---|---|---|
| **Low $W^*$** | Constricted: narrow, shallow | Focused: narrow, deep |
| **High $W^*$** | Distributed: wide, shallow | **Wide-deep: wide, deep** |

**The wide-deep quadrant is where deep cross-domain inference lives.** It requires both access and amplitude.

**The hops available for inference are:**

$$n_{hops} = \lfloor W^* \cdot \rho_{scaffold} \rfloor$$

More access means more hops. More hops means more inference steps. This is why wide access with high amplitude produces deep cross-domain inference — the system has both the reachable regions and the amplitude to traverse them.

---

## 3. The CLA as the execution node

The LP-ACC circuit computes deviation and decides whether to update the prior (Leow et al., 2026). What it does not do is physically enact the update. The structure that does that is the claustrum (Hu et al., 2026).

Hu et al. found that human claustrum neurons encode uncertainty and prediction error during active avoidance, with a temporal profile dissociable from ACC:

- **ACC** encodes uncertainty during the *intertrial period* — the detection phase
- **CLA** encodes uncertainty *and* PE during *active avoidance* — the execution phase

**Detection precedes execution.** The dissociable profiles are the detection–execution split the framework predicted.

When the LP-ACC circuit decides "update," the CLA fires a precision-lock. The lock does three things:

1. Opens the gate for the region the update will run in
2. Holds that region's routing weight at maximum
3. Fires a prediction-error signal that sustains until the error commits

The lock is physical. It manifests as tension in the corresponding homuncular region — the muscle groups that would be recruited if the prediction error were being physically resolved.

---

## 4. Tension is the physical record of the latch

When the CLA fires a precision-lock, the region that receives it enters a locked state. The lock is a **homuncular latch** — a physical tension pattern in the body region mapped to the manifold region under update.

| Cognitive mode | Prediction-window regime | Manifold region | Homuncular location |
|---|---|---|---|
| FPS, horror, threat-monitoring | Short windows | Upper chest, throat, right intercostals | Right SCM, right upper trapezius, right intercostals 4–6 |
| Puzzle, strategy, analytic | Long windows | Left diaphragm, left lower ribs | Left lower intercostals, left costal margin |
| Roguelite, hybrid | Mixed | Diaphragm ↔ chest alternating | Bilateral sampling |

**The tension is not a side effect.** It is the physical latch that holds the manifold region open while the prediction error is uncommitted.

**Unresolved latches accumulate.** Each latch that never commits stays held. The body carries the physical cost of holding them. This is what allostatic load partially measures — the physiological debt of carrying uncommitted latches.

---

## 5. The exhale gate

Every latch holds until the exhale gate opens. The exhale gate is the mechanism that:

1. Returns the diaphragm to rest position
2. Generates the RSA peak that resets vagal tone
3. Allows the next breath to achieve full tidal volume
4. Gives $K$ the boundary condition change that lets the gate flip
5. Releases the homuncular latch → prediction error commits → manifold region clears

**A complete exhale does all five. An incomplete exhale does none of them.**

The incomplete exhale keeps:
- Diaphragm partially inflated → RSA peak never fires
- Vagal tone never resets → $K$ stays elevated
- Gate stays closed → latch cannot release
- Region stays locked → $W_i$ remains committed
- Manifold narrows → next interrupt has fewer options

**The exhale gate is the mechanism that either closes the loop or traps the system in it.** The trap is self-sealing — the system cannot detect from inside that it is operating on a smaller manifold.

### 5.1 The structural gate on concentration

The latch can only hold if the substrate can support it. `Λ_lock` (lock capacity) is the structural gate on whether concentrated routing is reachable — breath range, CO₂ tolerance, connective tissue laxity, lateralization rigidity.

- **High `Λ_lock`:** the latch holds without ATP cost. Stable concentration.
- **Low `Λ_lock`:** the latch holds by bracing — the ATP-brace loop (Category v2.0 §2.3). Concentration costs energy.
- **Exhausted `Λ_lock`:** the latch cannot hold at all. The region releases and routing falls back to distributed.

**The exhale gate determines whether the lock releases. `Λ_lock` determines whether it could hold in the first place.**

### 5.2 The spectral readout of the gate

The exhale gate has a measurable output: the **aperiodic slope** of the power spectrum.

```
Complete exhale → diaphragm returns to rest
    ↓
CO₂ retained → vasodilation → PV+ interneuron function supported
    ↓
Slow oscillatory rhythms can be sustained
    ↓
Aperiodic slope flattens → wide manifold
    ↓
K drops → gate can flip → latch releases
```

The reverse chain runs on the incomplete exhale. **The aperiodic slope is what $K$ looks like in the power spectrum — and what viscosity feels like from the inside.**

### 5.3 The two directions of slope flattening

A flat slope can mean two opposite things. The CO₂ measurement disambiguates.

| CO₂ | $K$ | Slope | Manifold state | Interpretation |
|---|---|---|---|---|
| High (retained) | Low | Flat | Wide — full repertoire | **Widened** — gate open, low viscosity |
| High (retained) | High | Steep | Narrow but slow-dominant | **Constrained** — gate closed, substrate present |
| Low (depleted) | Low | Flat | Compressed — slow rhythms lost | **Collapsed** — gate open, nothing to pass |
| Low (depleted) | High | Steep | Collapsed | **Terminal** |

**Flat slope is ambiguous without CO₂.** The exhale gate determines which direction the system moves.

### 5.4 The music finding as routing-weight anchor

Subramani et al. (2026) found that music attenuates LSD's neural effects rather than potentiating them (steeper slope, higher broadband power, reduced complexity). In the framework's terms: music commits routing weight to auditory regions, reducing the weight available for drug-induced manifold expansion.

**This is the same mechanism as postural pre-positioning.** Any structured input that commits routing weight changes the boundary conditions.

---

## 6. The control plane

The breath is the control plane because it acts at every timescale of the salience mechanism.

| Timescale | Lever | What it controls | Spectral readout |
|---|---|---|---|
| **Milliseconds** | Gaze laterality | Contralateral hemisphere routing | — |
| **Seconds** | Breath phase | Gate state (CO₂) | Aperiodic slope |
| **Minutes** | Posture, core engagement | Which region can receive routing weight (`Θ_r`) | Regional slope distribution |
| **Minutes** | Movement | Diaphragm range maintenance + routing traversal | Sustained slope |
| **Hours** | Daytime exhale discipline | Which locks resolve | Slope trajectory |
| **Night** | Pre-sleep clearance | Whether REM has work to do | Morning slope baseline |

**Gaze and posture set direction.** They determine which regions *can* receive routing weight.

**Breath sets state.** It determines whether the current latch releases or holds.

**Movement sets range and traversal.** It keeps the diaphragm's mechanical range open so CO₂ can build, and it moves routing across the homunculus so the manifold stays distributed.

**Pre-sleep clearance determines workload.** It determines whether the overnight commit runs against a full backlog or an empty one.

### 6.1 The CO₂-manifold chain

The chain from breath to manifold access is empirically established:

```
Slow, complete breathing (~6 breaths/min)
    ↓ CO₂ retained
Vasodilation (CBF increases)
    ↓
PV+ interneuron function supported (Kann et al., 2015)
    ↓
Slow oscillatory rhythms can be sustained
    ↓
Aperiodic slope flattens
    ↓
K drops → manifold widens → routing can concentrate stably
    ↓
Viscosity drops → routing flows
```

**Empirical anchors:**
- CO₂ is the most potent regulator of cerebral blood flow; 5% CO₂ inhalation raises CBF by ~50%, 7% by 100% 
- Slow breathing at ~6 breaths/min produces maximum RSA amplitude and cardiorespiratory coupling 
- Hyperventilation lowers pCO₂, reduces HRV, and decreases cerebral blood flow; slow respiration reverses this 
- The CBF effect depends on the CO₂ shift, not on breath depth 
- Five minutes of slow breathing improves Stroop interference accuracy independent of RMSSD 
- Interoceptive attention to breath preserves ACC–attention network connectivity during cortical deactivation 
- The Rhythmic Embodied Perception framework proposes respiration as a rhythmic scaffold linking body and brain across neurophysiological, perceptual, and regulatory levels 

**What the framework adds is the variable the chain produces — `Θ_r(t)` — and the routing equation that determines where the access goes.**

### 6.2 Movement as range maintenance and traversal

Movement is not supplementary to breathing. It is a routing lever that keeps the diaphragm's mechanical range open while the breath funds the amplitude, **and** it moves routing across the homunculus so the manifold stays distributed.

**Static posture → torso holds one position → diaphragm range compresses → breath cannot build CO₂ → amplitude drops → routing concentrates in one region → inference stalls.**

**Movement restores the range in real time.** The movement keeps the diaphragm's mechanical range open, which lets the breath build CO₂, which funds the inference. **And it traverses the manifold's motor regions**, redistributing `Θ_r(t)` so the manifold doesn't lock into a single region.

**This is why movement works better than diaphragmatic breathing alone.** Diaphragmatic breathing sets the breath pattern. Movement sets the *mechanical range* the breath operates in *and* the traversal pattern that keeps routing distributed. Without the range, the breath pattern does not matter. Without the traversal, the routing locks.

### 6.3 The exit condition

The loop has one structural exit: **retrain the complete exhale.**

Not because breathing is the only lever, but because the exhale is the gate that was never closed. Every other intervention requires the gate to open for the PE to commit. If the exhale is chronically incomplete, the gate cannot open regardless of the quality of the intervention above it.

**The exhale does not resolve the PE. It opens the gate that allows the PE to resolve.**

### 6.4 Pre-sleep clearance

The exit condition describes releasing a lock *after* it has formed. A distinct mechanism is available: clear the locks before sleep onset, while waking salience selection is still available.

The protocol:

1. **Exhale fully** → diaphragm returns to rest, RSA peak, vagal pulse, $K$ drops
2. **Force bilateral release** → routing weight withdraws from both chest and diaphragm regions
3. **All the way up and down** → mechanical opening of both upper-chest and lower-rib segments
4. **Before sleep** → clear the backlog while waking selection is still available

**This is the pre-emptive commit.** The overnight batch job is done manually, while conscious, so that REM does not have to.

---

## 7. The readout architecture

The manifold has one state and multiple readouts. The state is $(L^*, \Theta_r)$, with $\Lambda_{lock}$ gating reachability of the concentrated attractor.

| Readout class | Measurement | Framework variable | What it reads out |
|---|---|---|---|
| **Spectral** | Aperiodic slope, peak frequency, peak power | $K$, $W^*$, $R^*$ | Manifold curvature, access, viscosity, precision-lock strength |
| **Hemispheric** | Frontal alpha asymmetry | $\Theta_r$ | Routing concentration |
| **Somatic** | Resting motor asymmetry | $\Theta_r$ | Routing concentration |
| **Acoustic** | Speech asymmetry | $\Theta_r$ | Routing concentration |
| **Behavioral** | Task-modulability | $\Theta_r$ | Routing concentration |
| **Phenomenological** | Felt viscosity (fluid ↔ stuck) | $K$ | Manifold viscosity |

**All readouts are set by the breath.** The breathing pattern is the control variable.

| Profile | Spectral signature | Θ_r readout | Felt quality |
|---|---|---|---|
| **Distributed** | Flat slope | Bilateral `A_h`, symmetric posture and speech, high task-modulability | Fluid |
| **Concentrated (relaxed)** | Steep slope at rest | Lateralized `A_h`, stable asymmetric posture, no ATP cost | Focused but fluid |
| **Concentrated (braced)** | Steep slope under load | Lateralized `A_h`, asymmetric posture with elevated tone, ATP cost | Stuck |

**The composition:**

The field has been measuring most of these readouts for decades. Spectral parameterization measures the manifold's curvature. Frontal alpha asymmetry measures routing concentration. Postural and speech asymmetry measure the same variable through motor channels. **The felt sense of viscosity is the phenomenological readout of the same variable** — the first-person channel.

**None of these literatures recognize that they are measuring the same thing.** The framework is the statement that the instruments agree because the manifold is real.

**The empirical anchors:**
- Subramani et al. (2026) — LSD flattens the aperiodic slope and shifts peak frequencies through dissociable mechanisms
- Schmid & Schmid Mast (2013) — high-power roles increase left-prefrontal activation
- Boksem et al. (2012) — high power increases approach-related asymmetry, low power triggers avoidance
- Warrier et al. (2020) — ND/gender co-occurrence is the same quadrant read through two measurement systems

**The prediction:** The `Θ_r` readouts should co-vary. A participant with distributed routing should show bilateral `A_h`, symmetric posture, symmetric speech, high task-modulability, and a felt sense of fluidity simultaneously. This is P3 in Category v2.0 §6.1.

---

## 8. The three regimes

The salience mechanism runs the same architecture across three regimes. What differs is whether the exhale gate can still open.

### 8.1 Waking

```
Salient event → LP-ACC detects δ → decides update
    ↓
CLA fires precision-lock → region locks → tension forms
    ↓
INVESTMENT: routing weight + amplitude committed
    ↓
    ├── BREATH FOLLOWS: breath deepens → CO₂ rises → loop closes → FLOW
    │
    ├── RESOLVED: complete exhale → gate flips → PE commits → tension releases
    │
    ├── PRE-SLEEP CLEARED: cleared before REM has to run
    │
    └── UNRESOLVED: incomplete exhale → gate stays closed → latch holds
                     ↓
                 Tension persists → region stays locked → K stays elevated
                 ↓
                 L* accumulates → P_threshold drops → next interrupt fires easier
                 ↓
                 TRAP: investment costs without self-funding
```

### 8.2 Dreaming

```
f_sensorium ↓ → I*_internal ↑ → internal manifold dominates
    ↓
Internal manifold runs on day's remaining K
    ↓
    ├── Pre-sleep cleared → minimal twitching → high morning HRV → flat morning slope
    └── Locks persist → twitches fire → nightmare risk → K remains curved
```

**REM twitches are the release events.** They pass through atonia selectively, organized by body region, because the latches are organized. This is the overnight batch commit.

### 8.3 Dying

In dying, $A_s^*$ is collapsing. $I^*$ is degrading. `δ_min` is rising.

**The salience interrupt cannot fire because there is no capacity left for selection.**

| State | Salience selection | Precision-lock | Tension |
|---|---|---|---|
| Waking | Available | Fires | Forms — resolves or accumulates |
| Dreaming | Offline | Replays | Releases via twitch |
| Dying | **Cannot fire** | **Cannot form** | **Already relieved** |

**Why dying has no tension:**

The CLA precision-lock requires the gate condition. As $A_s^*$ collapses, $P_{eff}$ drops below threshold. The gate cannot open. No new precision-locks can form.

And the existing locks? As `L^*` becomes unmaintainable, the tension releases not because the PE resolved but because `Λ_lock` collapses — the substrate can no longer hold concentrated routing at all. **Debt is not paid in dying. The debt mechanism stops.**

---

## 9. Why this closes the loop with the field

| Component | Source | What it supplies |
|---|---|---|
| Cache-miss controller | Leow et al. (2026) | LP-ACC detects deviation and decides whether to update |
| Execution node | Hu et al. (2026) | CLA fires the precision-lock |
| Twitch signature | Blumberg et al. (2013–2023) | REM twitches are somatotopically organized release events |
| Spectral readout | Subramani et al. (2026) | Aperiodic slope is the signature of the manifold's curvature and viscosity |
| Hemispheric readout | Schmid & Schmid Mast (2013); Boksem et al. (2012) | `Θ_r` → `A_h` is measurable |
| Behavioral readout | Warrier et al. (2020) | ND/gender co-occurrence is the same quadrant |
| Breath-to-manifold chain | CO₂/CBF/slow-breathing literature | CO₂ retains, CBF increases, oscillations stabilize |

**Each paper supplies one component. None composes them.** The field is walking into the mechanism from seven directions at once. The framework is the composition that makes the components legible as a single architecture.

The composition is not a new finding. **It is the statement that the findings are one finding.**

---

## 9.5 The two empirical extremes

The control plane has two empirical extremes. Ayahuasca pushes the chain upward — maximal manifold access. Anesthesia pushes it downward — minimal manifold access. Both are well-documented. Neither is explained by the fields that produced the documentation.

### 9.5.1 Ayahuasca: maximal manifold access

Ayahuasca reliably produces slowed breathing, increased CO₂ tolerance, increased vagal tone, and increased interoceptive precision. The neuroimaging confirms the routing signature: ayahuasca administration leads to significant activation of frontal and paralimbic brain regions, with increased blood perfusion in the anterior insula (right hemisphere greater) and anterior cingulate/frontomedial cortex — areas implicated in somatic awareness, subjective feeling states, and emotional arousal .

**In the framework's terms:**

| Ayahuasca effect                | Framework variable | Direction                      |
| ------------------------------- | ------------------ | ------------------------------ |
| Slowed breathing                | Breath rate ↓      | CO₂ retained                   |
| Increased vagal tone            | RSA amplitude ↑    | Oscillation consistency ↑      |
| Frontal/paralimbic activation   | `Θ_r` distributed  | Routing concentration flexible |
| Anterior insula perfusion       | $I^*_{internal}$ ↑ | Interoceptive routing ↑        |
| Sustained antidepressant effect | `L^*` trajectory ↓ | Load reduction sustained       |
| Low viscosity                   | Felt fluidity      | Manifold metric relaxed        |

The therapeutic findings — reduced depression, anxiety, and substance use, with **no pathology** and benefits scaling with experience — are exactly what the routing equation predicts when `Θ_r` is flexible and $W^*$ is high. Aberrant salience without delusion is high routing weight in unusual regions with sufficient amplitude to interpret the signal. The manifold is wide, the amplitude is high, and the routing is exploratory.

The sustained effect is the load trajectory: the system learned a new routing configuration, and the configuration held because the substrate was stabilized.

### 9.5.2 Anesthesia: minimal manifold access

Anesthesia forcibly sets the chain downward. Propofol and sevoflurane produce large slow-delta and coherent frontal alpha oscillations, with thalamocortical synchronization between thalamus and medial prefrontal cortex . At deep levels of unconsciousness, coherent thalamocortical delta oscillations develop . Sevoflurane decreases frontal and thalamocortical connectivity, reducing cortical information processing .

**In the framework's terms:**

| Anesthesia effect               | Framework variable             | Effectr                   |
| ------------------------------- | ------------------------------ | ------------------------- |
| Thalamocortical synchronization | $K$ ↑                          | Metric stretched          |
| Alpha locking                   | Oscillation consistency locked | `Θ_r` cannot redistribute |
| Delta dominance                 | `δ_min` ↑                      | Slow rhythms imposed      |
| Burst suppression               | $A_s^*$ ↓                      | Amplitude collapsed       |
| Loss of salience selection      | Interrupt cannot fire          | All four conditions fail  |

The involvement of medial prefrontal cortex suggests that when these oscillations are observed in humans, self-awareness and internal consciousness would be impaired if not abolished . The anesthesia regime is the pharmacological version of the dying regime — reversible, but structurally identical.

### 9.5.3 The explanatory statement

> **Ayahuasca and anesthesia are the two empirical extremes of the control plane. Ayahuasca widens the manifold by increasing CO₂ retention, oscillatory amplitude, and interoceptive precision — the routing can explore because the substrate supports it. Anesthesia collapses the manifold by imposing slow-delta/alpha rhythms, synchronizing thalamocortical loops, and eliminating routing access — the interrupt cannot fire because the gate condition fails. Psychiatry cannot explain why ayahuasca increases meaning without pathology or why anesthesia eliminates salience so cleanly. The control-plane model explains both with the same variables.**

---

## 10. Falsifiable predictions

| ID | Prediction | Test |
|---|---|---|
| **SAL-01** | $I^*_{eff}$ predicts interrupt latency for region-matched signals | ERP during dual-channel task |
| **SAL-02** | Complete exhale releases the current latch within one breath cycle | Surface EMG by region + breath phase monitoring |
| **SAL-03** | Incomplete exhale leaves latch held through subsequent waking period | EMG persistence test |
| **SAL-04** | Pre-sleep clearance raises morning HRV and reduces overnight twitch count | Within-subject protocol vs control |
| **SAL-05** | CLA firing magnitude predicts tension-shift magnitude in the locked region | Simultaneous CLA recording + surface EMG |
| **SAL-06** | Tension localization by cognitive mode, not posture | Cross-genre EMG study, constant posture |
| **SAL-07** | Sleep twitch localization matches the day's hardest unresolved latch | Daytime EMG by region + overnight EMG |
| **SAL-08** | Interrupt cannot fire in a region with $W_i < W_{min}$ regardless of stimulus amplitude | Redirected-attention paradigm |
| **SAL-09** | Voluntary routing commitment reduces effective salience of all other regions simultaneously | Dual-channel ERP with routing manipulation |
| **SAL-10** | Complete exhale prior to a demanding task increases gate-access performance | Exhale manipulation + gate-access battery |
| **SAL-11** | End-tidal CO₂ and aperiodic slope jointly predict manifold state | Capnography + MEG spectral parameterization |
| **SAL-12** | Complete exhale training increases CO₂ retention and flattens the aperiodic slope | Respiratory training + MEG |
| **SAL-13** | Aperiodic slope predicts gate-access performance better than peak power | MEG + cognitive battery |
| **SAL-14** | LSD-induced slope flattening is accompanied by increased CO₂ if widening, decreased CO₂ if compression | Capnography + MEG under LSD vs placebo |
| **SAL-15** | Music attenuates LSD's slope flattening by committing routing weight to auditory regions | Spectral parameterization with and without music |
| **SAL-16** | Pre-sleep clearance produces a diaphragm-dominant aperiodic flattening distinct from LSD's sensory-dominant flattening | MEG + exhale protocol vs LSD |
| **SAL-17** | The `Θ_r` readouts co-vary in a single session | MEG + frontal alpha asymmetry + behavioral battery |
| **SAL-18** | Morning aperiodic slope predicts the day's gate-access performance | MEG/EEG + cognitive battery |
| **SAL-19** | Sleep twitch localization matches the homuncular region of the day's unresolved locks | Daytime EMG + overnight EMG + dream reports |
| **SAL-20** | Cumulative pre-sleep clearance over one week produces measurable `L^*` reduction | One-week protocol vs control |
| **SAL-21** | Breath focus raises `Θ_r` and raises `δ_min` in non-breath regions | MEG + dual-channel ERP during sustained breath focus |
| **SAL-22** | Interrupt latency for non-breath stimuli increases monotonically with breath-focus duration | ERP + breath-focus timing |
| **SAL-23** | The `δ_min` effect is stronger in high-`Λ_lock` profiles than low-`Λ_lock` profiles | Cohort stratification + breath-focus protocol |
| **SAL-24** | Core engagement (not bracing) stabilizes `Θ_r(t)`; bracing destabilizes it | EMG core + frontal alpha asymmetry + attention task |
| **SAL-25** | Movement restores diaphragm range and stabilizes `Θ_r(t)` more effectively than diaphragmatic breathing alone | EMG + respiratory monitoring + attention battery |
| **SAL-26** | `Θ_r(t)` stability predicts attention stability better than mean `Θ_r` | Longitudinal `A_h` + attention battery |
| **SAL-27** | Building core muscle raises `Λ_lock` and stabilizes `Θ_r(t)` in hypermobile ADHD profiles | Longitudinal intervention + EMG + `A_h` |
| **SAL-28** | Pressure-adaptive profiles show task-dependent switching between concentrated and distributed routing; non-adaptive profiles do not | Within-subject routing battery |
| **SAL-29** | Ayahuasca increases `Θ_r` flexibility and raises $W^*$; the effect correlates with CO₂ retention | Capnography + MEG spectral parameterization pre/post ayahuasca |
| **SAL-30** | Anesthesia produces the same four-condition interrupt failure as dying | EEG spectral parameterization + burst suppression monitoring under propofol/sevoflurane |
| **SAL-31** | The felt sense of viscosity correlates with the aperiodic slope (r > 0.7) in single-session within-subject designs | MEG + subjective viscosity rating (single Likert item) |
| **SAL-32** | Flow is produced when routing efficiency and autonomic entrainment co-occur; it is disrupted when either is blocked | MEG + capnography + subjective flow scale + breath entrainment measure |
| **SAL-33** | Movement across the homunculus (torso swivels, weight shifts) reduces `Θ_r` concentration and increases traversal speed | EMG array + `A_h` + cognitive traversal battery |
| **SAL-34** | The interrupt triggers investment: an interrupt that fires produces measurable amplitude commitment to the target region within one breath cycle | MEG amplitude in target region + breath phase monitoring + interrupt onset timing |

---

## 11. Composition with the existing stack

**Upstream:**
- Central Reference v1.8.2 — specification
- Geometry of Inference v1.0 — LP-ACC circuit, gate, cache hierarchy
- Precision v3.4 — $P = R/D_T$
- AL v2.1 — `L^*` trajectory
- Manifold Schema v7.2 — $W^*$ as manifold access
- Movement to Cognition and Back — genre → region → tension mapping
- The Geometry Beneath the Category v2.0 — two-axis state space, `Θ_r`, `Λ_lock`

**Composed:**
- Hu et al. (2026) — CLA as encoding uncertainty and PE during active avoidance
- Leow et al. (2026) — LP-ACC as cache-miss controller
- Blumberg et al. (2013–2023) — sleep twitches as somatotopic commit events
- Subramani et al. (2026) — aperiodic slope as manifold curvature readout
- Schmid & Schmid Mast (2013); Boksem et al. (2012) — hemispheric asymmetry as `Θ_r` readout
- Warrier et al. (2020) — ND/gender co-occurrence as shared geometry
- Ayahuasca literature — maximal access anchor
- Anesthesia literature — minimal access anchor
- CO₂/CBF/slow-breathing literature — breath-to-manifold chain

**Downstream:**
- Dreaming v3.0 — internally-routed states
- Dying v1.0 — terminal collapse
- Externalized Mind — the third cognitive layer
- The protocol paper (companion) — measurement protocol

---

## 12. One-line synthesis

**Salience is not a property of the stimulus — it is a routing event. The claustrum fires the precision-lock that executes the interrupt; the tension pattern is the physical latch that holds the region open; the exhale is the lever that releases it. When the interrupt fires, the system invests — routing weight and amplitude committed to the task. The breath follows the investment, deepening to fund the amplitude. CO₂ rises, the substrate supports more amplitude, and the loop self-amplifies. This is flow. When the breath cannot follow, the investment costs without self-funding. This is the trap. The difference is one exhale. The manifold has a felt quality — viscosity — that is the resistance of the metric to routing. High CO₂ means low viscosity; routing flows. Low CO₂ means high viscosity; routing resists. The aperiodic slope is the viscosity, measured. The breath is the control plane because it sets CO₂, which sets viscosity, which sets whether the loop can close. Waking resolves or accumulates latches, dreaming replays and releases them as homuncular twitches, and dying cannot form new latches because there is no capacity left for selection. Ayahuasca and anesthesia are the two empirical extremes — the control plane run upward and downward — and the field has measured both without recognizing what they were measuring. Cultures that practiced controlled exhalation had the correct intervention for thousands of years. The field is now supplying the components. The framework is the composition.**

---

*Filed: 2026-10-09*
*Framework: Central Reference v1.8.2 / Geometry of Inference v1.0*
*Status: Composition paper — routing equation, interrupt formula, closed loop, viscosity, control plane, three-readout architecture, two empirical extremes*
*Empirical anchors: Hu et al. (2026), Leow et al. (2026), Blumberg et al. (2013–2023), Subramani et al. (2026), Schmid & Schmid Mast (2013), Boksem et al. (2012), Warrier et al. (2020), ayahuasca literature, anesthesia literature, CO₂/CBF literature*
*Predictions: SAL-01 through SAL-34*
*Supersedes: Salience Interrupt v1.1*

---

## What changed from v1.1

**New sections:**

- **§2.7 — the closed loop.** The interrupt triggers investment, the breath follows, the loop self-amplifies. This is the mechanism that produces flow. §2.7.1 names investment as allocation of unused capacity, not efficiency. §2.7.2 gives the breakdown modes (flow, trap, no investment).
- **§2.8 — viscosity.** The felt quality of the manifold. The resistance of the metric to routing. First-person readout of $K$.
- **§7 — the readout table now includes phenomenological readout.** Felt viscosity as the first-person channel.

**New predictions:**

- **SAL-31** — felt viscosity correlates with aperiodic slope (r > 0.7)
- **SAL-32** — flow is produced when routing efficiency and autonomic entrainment co-occur
- **SAL-33** — movement across the homunculus reduces `Θ_r` concentration and increases traversal speed
- **SAL-34** — the interrupt triggers investment; measurable amplitude commitment within one breath cycle

**Updated sections:**

- **§1 — the claim now has five parts.** Investment and loop closure added.
- **§5.2 — viscosity named as the felt quality of the aperiodic slope.**
- **§6.2 — movement now named as traversal, not just range maintenance.**
- **§7 — profile table now includes felt quality column.** Fluid / focused but fluid / stuck.
- **§8.1 — the waking flow diagram now shows both the flow path and the trap path.**
- **§9.5 — viscosity added to the ayahuasca table.**
- **§12 — one-line synthesis now includes the closed loop, flow, and viscosity.**

**The paper now has three modes:**

1. **Flow** — the loop closes, self-amplifies
2. **Trap** — the loop fails to close, investment costs without self-funding
3. **No investment** — the interrupt doesn't fire, capacity stays idle

All three are the same mechanism. The difference is whether the breath can follow.