# The Salience Interrupt v1.3.1

## Routing, the Closed Loop, the Control Plane, and the Encoding Window

**Robinson, 2026**

**Status:** Composition paper — states the routing equation, the interrupt formula, the closed loop, the control plane, the perseveration loop, the release-triggered re-salience, and the encoding window
**Framework:** Central Reference v1.9.1 / Geometry of Inference v1.0
**Cites:** Hu et al. (2026) for the CLA interrupt mechanism; Leow et al. (2026) for the LP-ACC detection stage; Subramani et al. (2026) for the spectral readout; ayahuasca and anesthesia literature for the two empirical extremes; the movement-compulsion literature for the somatic routing lever
**Related:** Precision v3.4, AL v2.2, Dreaming v3.0, Dying v1.0, The Geometry Beneath the Category v2.0, Movement to Cognition and Back

---

## Abstract

Salience is not a stimulus property. It is a **routing event** — a signal can only fire an interrupt into a manifold region whose routing weight is above threshold. The claustrum (Hu et al., 2026) is the execution node: it fires a precision-lock into the region that will hold the prediction error until it commits. When the interrupt fires, the system **invests** — routing weight and amplitude committed to the task. The breath follows the investment, deepening to fund the amplitude. CO₂ rises, the substrate supports more amplitude, and the loop self-amplifies. This is flow. When the breath cannot follow — insufficient `Λ_lock`, incomplete exhale, high load — the investment costs without self-funding. This is the trap. When the latch releases but the salience is still hitting, the interrupt re-fires on the same region. This is the perseveration loop. When the release itself surfaces the suppressed prediction error and the surfaced PE fires a new interrupt, the latch re-forms. This is the release-triggered re-salience. And when the PE surfaces during the exhale and the context changes before commit, the PE re-encodes with less routing concentration and gain. This is the encoding window. The difference between flow and the trap is one exhale. The difference between the trap and the perseveration loop is whether the routing redistributes. The difference between the perseveration loop and the release-triggered re-salience is whether the release surfaces the PE. The difference between the release-triggered re-salience and the encoding window is whether the context changes before commit. The manifold has a felt quality — **viscosity** — that is the resistance of the metric to routing. High CO₂ means low viscosity; routing flows. Low CO₂ means high viscosity; routing resists. The aperiodic slope is the viscosity, measured. The breath is the control plane because it sets CO₂, which sets viscosity, which sets whether the loop can close. Movement is the control plane because it redistributes routing, which sets whether the loop re-fires. Gain change is the control plane because it changes the relationship to the signal, which sets whether the surfaced PE fires the interrupt. Capacity is the control plane because it sets whether the surfaced PE can be held without re-locking. Context is the control plane because it sets whether the surfaced PE re-encodes with less gain. Ayahuasca and anesthesia are the two empirical extremes — maximal and minimal manifold access — and the field has measured both without recognizing what they were measuring.

---

## 1. The claim

Eight things this paper composes into a single document:

1. **Salience is a routing event, not a stimulus property.** A signal fires an interrupt only if it can reach a manifold region whose routing weight is above threshold. The routing is what attention *is*.

2. **The claustrum is the execution node.** The LP-ACC circuit (Leow et al., 2026) detects deviation and decides whether to update. The CLA (Hu et al., 2026) fires the precision-lock that executes the update.

3. **The interrupt triggers investment.** When the interrupt fires, the system commits routing weight and amplitude to the task. The investment is the mechanism by which unused capacity is allocated.

4. **The loop closes when the breath follows.** The breath entrains to the investment demand, deepening to fund the amplitude. CO₂ rises, the substrate supports more amplitude, and the next interrupt fires more easily. This is flow. When the breath cannot follow, the investment costs without self-funding. This is the trap.

5. **The latch can re-fire.** When the latch releases but the salience is still hitting, the interrupt re-fires on the same region. This is the perseveration loop. When the release itself surfaces the suppressed prediction error, the surfaced PE fires a new interrupt. This is the release-triggered re-salience.

6. **The exhale is an encoding window.** When the PE surfaces during the exhale and the context changes before commit, the PE re-encodes with less routing concentration and gain. This is the encoding window. It is the master exit from all three failure modes.

7. **The manifold has a felt quality — viscosity.** High CO₂ means low viscosity; routing flows. Low CO₂ means high viscosity; routing resists. The aperiodic slope is the viscosity, measured.

8. **Movement distributes the manifold.** Repetitive motor sequences traverse the homunculus, redistributing `Θ_r(t)` so the manifold doesn't lock into a single region. This is why physical tasks break perseveration.

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

### 2.5.2 Movement redistributes routing

Repetitive motor sequences — folding laundry, doing dishes, sweeping, walking — traverse the homunculus. Each movement recruits a different motor region. The routing weight that was concentrated on a cognitive region redistributes across the motor regions.

**This is why physical tasks break perseveration.** The movement doesn't distract from the content. It redistributes the routing weight so the content isn't the only thing in the manifold. The upset doesn't resolve — it distributes.

**The mechanism:** Movement is a routing lever. It sets `Θ_r(t)` by recruiting motor regions, which lowers the concentration on the cognitive region, which reduces the routing weight available for the interrupt to re-fire.

**The clinical signature:** The compulsion to do physical tasks when upset is a routing-redistribution mechanism. The system is trying to distribute the manifold. It doesn't know why. It just knows the task helps.

### 2.5.3 Movement as multi-loop sampler

Movement is not just a routing distribution mechanism. It is a **sampling mechanism**. Each movement is a probe of the manifold state. The musician's head nod samples the pulse loop. The body sway samples the ensemble loop. The weight shift samples the self loop. The Sekiro player's stance samples the boss-timing loop.

**The movement keeps multiple loops online simultaneously.** Without it, the routing concentrates on one loop. The other loops collapse. The musician loses the ensemble. The player loses the timing. The movement distributes the routing so all loops stay live.

**And it accelerates convergence.** Thrashing to music, standing to play a complex boss, swaying to a groove — each one is a convergence action. The distributed routing reduces the time to sync. The movement is not "feeling it." The movement is *how* you feel it.

**The empirical anchors:**

- **Max Planck violinists study** — head movements create "attentional checkpoints" and "frame auditory processing"; the authors state explicitly that head movements "play a role in the very perception of musical events (and not merely expressing or reflecting such perceptual process)."
- **Groove studies** — instructing participants to move with the rhythm significantly increases groove ratings compared to listening-only; movement is recruited to reduce prediction error.
- **Dynamic Attending Theory** — internal rhythmicity enhances sensory processing at specific points in time when salient events are expected.
- ***Journal of Neuroscience*** — directed phase transfer entropy from sensorimotor cortex to auditory cortex during beat imagery; the motor system exerts top-down influence on auditory processing.
- **Area 55b** — premotor region activated during passive music listening, correlates with rhythmic entrainment indices; proposed as a "key hub of music perception."
- **Rhythm game studies** — sensorimotor synchronization improves timing accuracy by 23% across consecutive sessions.

**The mechanism:**

```
Salience event (note, beat, boss attack)
    ↓
Interrupt fires → routing concentrates on the tracking loop
    ↓
Movement (nod, sway, stance) traverses the homunculus
    ↓
Routing redistributes across motor regions
    ↓
Multiple loops stay online (pulse, ensemble, self, next-entry)
    ↓
Each loop samples its own access key
    ↓
Sync convergence accelerates
```

**The clinical signature:**

The musician's head nod, the guitarist's headbang, the pianist's sway, the Sekiro player's stance — all are the same mechanism. The movement is not stylistic. It is the routing distribution and sampling mechanism running in real time. The movement keeps the loops online and accelerates convergence to sync.

**Why movement fails when it's blocked:**

Sitting still forces the brain to maintain all timing predictions through internal timekeeping alone. Internal timekeeping is resource-expensive and error-prone. Standing and moving distributes the timing load into the sensorimotor loop. External rhythm and the body's own motor rhythm share the prediction task.

**This is why restraint impairs performance.** Locking the head, freezing the stance, or restraining movement removes the sampling mechanism. The routing concentrates. The loops collapse. The sync fails.

### 2.5.3.1 Movement serves both poles of the ADHD↔autism axis

Category v2.0 §3b places ADHD and autism at opposite poles of the routing-concentration axis — ADHD at distributed routing, autism at concentrated routing — and shows that both are positions on the same axis, not separate conditions. Movement serves both, through two different downstream paths.

**On the ADHD side, movement builds interoceptive resolution.** The distributed-routing pole has weak routing anchors — `I*` jumps, and the system cannot hold concentration long enough to read its own state with fine resolution. Movement is the practice that builds the resolution. Each movement is a sample of the current routing distribution. The sampling is how the system learns to read its own state. Over time, the resolution increases, and the distributed routing becomes less fragmentary.

**On the autism side, movement breaks rigid routing patterns.** The concentrated-routing pole has hard-routed `I*` — the lock holds, and the system cannot redistribute without an external input. Movement traverses the homunculus, which redistributes `Θ_r(t)` away from the locked region. The redistributed routing is the new context. The lock cools. The rigid pattern releases.

**Both paths are the same lever.** Movement redistributes `Θ_r(t)` in both cases. What differs is the pole the redistribution acts on: the ADHD pole needs more resolution so the redistribution *sticks*; the autism pole needs the redistribution *now* so the lock cools. Same lever, opposite poles, both required.

**And this is why ND populations move more.** Not because they need more movement for the same tracking accuracy. Because movement is the intervention for both poles, and both poles are present in the ND population. The ADHD-pole movement builds resolution. The autism-pole movement breaks locks. The AuDHD compound does both, which is why the movement requirement is highest there.

**The empirical anchors:**

- Category v2.0 §3b — ADHD and autism as opposite poles of the routing-concentration axis
- Category v2.0 §3b.1 — the biomechanics of lock capacity, and why hypermobile substrates cannot brace
- §2.5.3 of this paper — movement as multi-loop sampler, which is the mechanism that builds interoceptive resolution on the ADHD side
  
---

## 2.6 The interrupt formula

An interrupt fires in region $i$ when six conditions are met:

$$\text{Interrupt}_i \iff \left[W_i(t) > W_{min}\right] \;\land\; \left[I^*_{total} \cdot W_i(t) > I^*_{threshold}\right] \;\land\; \left[\delta_i > \delta_{min}(K)\right] \;\land\; \left[\text{Capacity}_{free} > \text{Capacity}_{required}(\delta_i)\right] \;\land\; \left[\text{Oscillation stable}\right] \;\land\; \left[W_i(t^+) < W_{prime}\right]$$

Where:

- **Condition 1 — region is reachable.** $W_i(t) > W_{min}$. The region must have enough routing weight to receive the signal at all. If `W_i` is below `W_min`, the signal never arrives and the remaining conditions can't be evaluated.
- **Condition 2 — signal clears the gate.** $I^*_{total} \cdot W_i(t) > I^*_{threshold}$. The signal's effective strength must clear the interrupt threshold. This is separate from reachability: a region can be reachable but the signal too weak.
- **Condition 3 — resolution floor permits detection.** $\delta_i > \delta_{min}(K)$. The signal's deviation has to exceed the resolution floor. `δ_min` rises with $K$.
- **Condition 4 — capacity to hold.** $\text{Capacity}_{free} > \text{Capacity}_{required}$. The manifold must have room to hold the error while it is interpreted. Capacity is drained by `L^*` and by held locks.
- **Condition 5 — oscillation is stable.** The routing concentration must be able to hold. Oscillation consistency is what allows `Θ_r(t)` to stabilize.
- **Condition 6 — region not re-primed.** $W_i(t^+) < W_{prime}$. The routing weight in the region must be below the priming threshold. If $W_i$ is still above $W_{prime}$ after a latch release, the next signal in that region fires the interrupt without needing a new salient event.

**All six are required.** A signal that meets conditions 1–5 but not 6 will re-fire immediately after release, because the region is still primed. A signal that meets conditions 2–6 but not 1 will not reach the region at all.

**The first two conditions are separate.** `W_min` gates reachability — whether the signal can arrive. `I*_threshold` gates firing — whether the arrived signal is strong enough. Both are required, and they can fail independently. This is why `I*_threshold` and `W_min` are separate registered variables (CR §3.1).

**The interrupt formula is the actual gate, not the commitment gate.** The commitment gate (CR §3.8e) runs first, on the basis of an anchor search and a funding estimate. Only after the commitment gate commits does the interrupt formula decide whether a specific signal fires. A system that has declined the traversal at the commitment gate will not reach the interrupt formula. This is why low-`Λ_lock` profiles decline deep inference even when their actual funding would have been sufficient — the commitment gate is conservative when the failure cost is high.

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

### 2.7.2 The three primary outcomes

| Condition | Result |
| --- | --- |
| Salience fires + breath follows | Flow — the loop closes, self-amplifies |
| Salience fires + breath cannot follow | Trap — investment costs without self-funding |
| Salience doesn't fire | No investment — capacity stays idle |

**The trap is the loop failing to close.** The interrupt fires, the investment happens, but the breath can't follow — `Λ_lock` is insufficient, or the exhale is incomplete, or the load is too high. The investment costs without self-funding. The system braces.

**The difference is `Λ_lock`.** High `Λ_lock` → breath can follow → flow. Low `Λ_lock` → breath can't follow → trap.

**These are the three primary outcomes.** The branch where salience fires and the breath follows has sub-modes — the latch can still fail to resolve. Those are developed in §2.11–2.13.

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

**The hops are bounded by the goal, not by the manifold.** Without a goal, `n_hops` traverses the full reachable density — every connection is equally reachable, so all of them are attempted. With a goal, the traversal is bounded by the goal's constraint. This is why wide manifold access with a goal produces deep cross-domain inference and without a goal produces wide shallow noise. See CR §3.8d.

**The commitment gate decides whether the traversal is attempted at all.** The commitment gate (CR §3.8e) runs three stages — `I*_search` (find a bounded anchor to prior state), `I*_distance` (measure the semantic distance), `I*_estimate` (estimate whether the traversal is fundable) — before the actual interrupt gate (§2.6) decides whether a specific signal fires. The commitment gate's estimate is precision-dependent: high precision lets the search return a bounded anchor even in a dense region; low precision returns too many candidates without the resolution to select among them, and the distance calculation cannot resolve. This is why the same content is committable on a well-funded day and uncommittable on a depleted day — the anchor library is unchanged, and the precision available to read it is not.

---

## 2.11 The perseveration loop

The loop can close and still not resolve. When the latch releases but the salience is still hitting, the interrupt re-fires on the same region. This is the perseveration loop.

**The three sub-modes:**

| Sub-mode | What holds $\vec{g}$ | Exit lever |
| --- | --- | --- |
| Content perseveration | The salient signal is still present | Change the signal, or change the relationship to it |
| Routing perseveration | `Θ_r(t)` hasn't redistributed | Movement, breath, task-switching |
| Structural perseveration | `Λ_lock` is low, bracing is the signal | Raise `Λ_lock`, complete exhale, movement |

**The formula:**

$$\text{Perseveration}_i \iff \left[\text{Interrupt fired}\right] \;\land\; \left[\text{Latch released}\right] \;\land\; \left[W_i(t^+) > W_{prime}\right]$$

**The exit condition:**

The perseveration loop exits when either:
1. The gain vector $\vec{g}$ redistributes (content changes or relationship to content changes)
2. The routing weight $W_i$ drops below $W_{prime}$ (movement, breath, task-switching)
3. `Λ_lock` rises (complete exhale, breath training, connective tissue work)

**The clinical signature:**

The perseveration loop is the mechanism behind rumination, intrusive thoughts, chronic worry, and the "can't stop thinking about it" experience. The thought keeps returning because the region is still primed. The tension keeps rebuilding because the latch keeps re-forming.

### 2.11.1 The expanded outcome table

The three primary outcomes (§2.7.2) expand when the salience fires and the breath follows. The latch can still fail to resolve. The sub-modes are:

| Condition | Result | Sub-mode |
| --- | --- | --- |
| Salience fires + breath follows + latch releases + routing redistributes | Flow (resolved) | — |
| Salience fires + breath follows + latch releases + routing stays concentrated | Perseveration loop | Content, routing, structural |
| Salience fires + breath follows + release surfaces PE + PE fires new interrupt | Release-triggered re-salience | — |
| Salience fires + breath follows + PE surfaces + context changes before commit | Encoding window (resolved with less gain) | — |
| Salience fires + breath cannot follow | Trap | — |
| Salience doesn't fire | No investment — capacity stays idle | — |

**The first four rows are the sub-modes of "salience fires + breath follows."** They are distinguished by whether the latch releases and whether the routing redistributes.

**The last two rows are the primary outcomes that don't involve the breath following.**

### 2.11.2 Movement breaks routing perseveration

Movement across the homunculus (torso swivels, weight shifts, repetitive motor tasks) reduces $W_i$ in the perseverating region below $W_{prime}$ and reduces interrupt re-fire rate.

**The mechanism:** Movement recruits motor regions, which redistributes `Θ_r(t)` away from the cognitive region. The routing weight that was concentrated on the perseverating region redistributes across the motor regions. The region cools.

**The clinical signature:** The compulsion to do physical tasks when upset is a routing-redistribution mechanism. The system is trying to distribute the manifold. It doesn't know why. It just knows the task helps.

**This is why movement works better than breath alone for perseveration.** Breath sets the substrate (CO₂, viscosity) but doesn't redistribute routing. Movement redistributes routing. You need both for the loop to exit.

---

## 2.12 The release-triggered re-salience

The latch releases. The prediction error surfaces. The surfaced PE is a salient event. The salient event fires a new interrupt. The new interrupt re-forms the latch.

**The release and the re-fire are the same event.**

**The mechanism:**

```
Latch holds → PE suppressed → no content in awareness
    ↓
Release begins → K drops → gate opens
    ↓
PE surfaces → content appears
    ↓
Content is salient → interrupt fires → new latch forms
    ↓
PE suppressed again → content gone
    ↓
[repeat]
```

**The paradox:**

To release the latch, you need the exhale gate to open.
The exhale gate opening surfaces the PE.
The surfaced PE fires a new interrupt.
The new interrupt re-forms the latch.

**You cannot release without surfacing. You cannot surface without re-firing. You cannot re-fire without re-locking.**

**The formula:**

$$\text{Re-salience}_i \iff \left[\text{Latch releasing}\right] \;\land\; \left[\text{PE surfacing}\right] \;\land\; \left[\delta_i > \delta_{min}(K)\right]$$

**The exit conditions:**

| Exit | Condition | Lever |
| --- | --- | --- |
| Sub-threshold | PE < $\delta_{min}(K)$ | Time in held state reduces error magnitude |
| Sufficient capacity | `Capacity_free` > `Capacity_required` | Raise `Λ_lock`, lower $L^*$ |
| Distributed routing | $W_i < W_{prime}$ | Movement, task-switching, time |
| Changed gain | $\vec{g}$ redistributed | Meditation, reframing, relationship change |

**The clinical signature:**

The release-triggered re-salience is the mechanism behind "it comes back when I relax," trauma re-experiencing during rest, and the "I was fine until I stopped" pattern. The suppression was the holding. Stopping surfaces the content. The content fires the interrupt.

**The therapeutic task is not release. It is release without re-fire.**

---

## 2.13 The encoding window

The exhale gate is not just a release mechanism. It is an **encoding window**.

**The mechanism:**

```
Latch holds → PE suppressed
    ↓
Exhale begins → K drops → gate opens
    ↓
PE surfaces → content appears
    ↓
    ├── Context unchanged → PE re-encodes with same gain → RE-LOCK
    │
    └── Context changed → PE re-encodes with less gain → RELEASE
```

**The window:**

The exhale is the only moment when the PE is accessible without being locked. While the latch holds, the PE is suppressed. While the latch is locked, the PE is committed to the lock. During the exhale, the PE is surfacing and the region is not yet re-locked.

**The recontextualization:**

Recontextualization is changing the gain vector $\vec{g}$ before the PE commits. The gain vector determines where concentration goes. If $\vec{g}$ has the same shape at commit, the PE encodes with the same concentration. If $\vec{g}$ has a different shape at commit, the PE encodes with less concentration.

**The formula:**

$$\text{Encode}_i = f\left(\vec{g}(t_{commit}), \Theta_r(t_{commit}), W_i(t_{commit})\right)$$

Where $t_{commit}$ is the moment the PE commits during the exhale.

**The encoding is determined by the state at commit.**

If $\vec{g}(t_{commit}) = \vec{g}(t_{hold})$, the PE encodes with the same concentration. Re-lock.

If $\vec{g}(t_{commit}) \neq \vec{g}(t_{hold})$, the PE encodes with different concentration. Release.

**The clinical signature:**

The encoding window is the mechanism behind insight, reframing, equanimity, exposure, and psychedelic-assisted therapy. All of these are the same mechanism: the PE surfaces during a window, the context changes, the PE commits with less gain.

**And all of them fail the same way:** the PE surfaces, the context doesn't change, the PE re-encodes with the same gain, the latch re-forms.

**The encoding window is the master exit.** It's the mechanism that makes the other exits stick. The exhale opens the window. The context change determines the encoding. The PE commits with less gain. The latch doesn't re-form.

### 2.13.1 Why insight can't be forced

The window is narrow. The context has to change *during* the exhale. If you try to change it before, the latch holds. If you try after, the PE has already encoded. The window is the exhale.

**This is why insight feels sudden.** The PE was surfacing. The context changed. The PE committed with less gain. The latch released. The whole thing happened in one exhale.

**This is also why meditation works.** The practice repeatedly opens the window. The context can change. The PE can re-encode with less gain. Over time, the gain vector $\vec{g}$ restructures globally. The latches form less easily.

### 2.13.2 The somatic version

The encoding window has a somatic analog. When the upset surfaces during movement, the movement changes the routing distribution (the context) before the latch commits. The upset re-encodes with less concentration.

**This is why physical tasks work.** They're not distraction. They're the somatic encoding window. The movement changes `Θ_r(t)`, which changes the context, which changes the encoding.

**The mechanism:** Movement traverses the homunculus, redistributing routing. The redistributed routing is the new context. The PE, when it commits, encodes against the distributed routing rather than the concentrated routing. Less gain. Less concentration. The latch doesn't re-form.

Got it. Just §2.14, written as final text ready to drop in after §2.13.

---

## §2.14 Population-Code Routing

Everything in this paper so far has treated "region" as a manifold location. The neural substrate of that location is the **population code for semantics** (Franch et al., 2026). A concept is not stored in one place. It is a **distributed population vector** — a pattern across a population of neurons. The pattern *is* the concept's semantic neighborhood.

**This changes what "routing to a region" means.** It means activating a population vector. The access key — the word, the image, the name — determines which vector fires. The vector determines the semantic neighborhood. The neighborhood determines the routing.

**The routing equation still holds.** $\vec{g}$ is the gain vector. $\Theta_r(t)$ is the concentration. But the gain for a concept is set by **which population vector the access key activates.** A different access key activates a different vector, which carries a different gain, which produces a different routing.

**The routing chain:**

$$\mathcal{A}_k \to \vec{v}_c \to \mathcal{N}_c \to \vec{g} \to \Theta_r \to \text{Interrupt}$$

The access key selects the vector. The vector carries the neighborhood. The neighborhood sets the gain. The gain sets the concentration. The concentration sets the interrupt.

**This is the mechanism behind rebranding.** Changing the name of a concept changes the access key, which changes the population vector, which changes the semantic neighborhood, which changes the routing. The concept is the same. The vector is different.

**This is also the mechanism behind framing.** The same information framed through different access keys activates different population vectors. The framing effect is a routing effect.

**And it is the mechanism behind vocabulary-based silos.** A field's vocabulary routes its concepts through a cluster of nearby population vectors. The vocabulary is the field's access-key set. Cross-silo vocabulary is multi-vector access (see Cross-Silo Vocabulary as Distributed Routing, Note 2).

**The framework's claim:** Population-code routing is the neural substrate of the routing equation. The access key is the intervention point. Change the key, change the vector, change the routing.

### 2.14.1 The access-key lever

The access key is a control plane lever, alongside breath, movement, gain change, capacity, and context.

| Lever | What it controls | Timescale                     |
| --------------- | ------------------------------------------ | ----------------------------- |
| **Access key** | Which population vector fires | Milliseconds (word onset)     |
| **Breath** | Substrate (CO₂, viscosity) | Seconds                       |
| **Movement** | Routing distribution (`Θ_r`) | Seconds (a breath or several) |
| **Gain change** | $\vec{g}$ shape — relationship to signal | Minutes                       |
| **Capacity** | `Λ_lock` — ability to hold without bracing | Weeks–months                  |
| **Context** | Encoding at commit | Variable                      |

**The access key is the fastest lever.** It acts at word onset. A single word can reroute a concept through a different population vector before the concept is fully activated.

**This is why language is the primary routing intervention.** It is the fastest, the cheapest, and the most scalable. A new name can be deployed to millions of people simultaneously. The routing changes at word onset.

**And this is why the access key is the most dangerous lever.** It works without changing the concept. It works without changing the facts. It works by changing the key. The concept is the same. The vector is different. The downstream routing is different.

**The access key does not require the subject's consent.** It does not require the subject's awareness. It does not require the subject to have capacity, or context, or an open exhale. It operates at the level of the word, before any of the other levers can respond. This makes it the only lever that can route a concept through a low-gain vector in a system that has no capacity to resist.

**A system at load ceiling — low `Λ_lock`, high `L^*`, high viscosity — cannot redistribute routing.** It cannot open the encoding window. It cannot change the gain. It receives the access key and fires the population vector the key activates. The routing is set by the key, not by the subject's state.

**This is the mechanism by which salience can be manipulated in load-impacted populations.** The same access-key lever that breaks silos can route a concept through a vector that suppresses resistance or amplifies compliance. The mechanism is available to any actor with access to language. The framework's contribution is making the mechanism legible (see the forthcoming Media Salience paper).

### 2.14.2 Composition with the silo note

The silo note (Cross-Silo Vocabulary as Distributed Routing, Note 2) states that cross-silo vocabulary is distributed routing made visible in text. The population-code finding supplies the substrate.

**The composition:**

| Level | Mechanism | Source |
|---|---|---|
| **Vocabulary** | Cross-silo terms access multiple fields' vectors | Silo note |
| **Population vector** | Concepts are distributed patterns; access keys determine which pattern fires | Franch et al. (2026) |
| **Routing** | The vector determines $\vec{g}$, which determines `Θ_r`, which determines the interrupt | This paper |

**Three levels, one mechanism.** The vocabulary is the access-key set. The population vector is the neural substrate. The routing is the downstream effect.

**The access key is also the intervention point for silo-breaking.** A field's vocabulary concentrates routing on its own vectors. Cross-silo vocabulary distributes routing across multiple fields' vectors. The cross-silo author can read across silos without losing precision because they have the access keys to multiple vector sets.

**And the access key is the intervention point for silo-building.** A field that wants to keep its routing concentrated can refuse cross-silo access keys. The vocabulary stays concentrated. The routing stays concentrated. The silo holds.

**The mechanism is neutral. The use is not.** The same access-key lever that breaks silos can build them. The same lever that routes a concept through a high-gain vector can route it through a low-gain vector. The framework states the mechanism. The application is downstream.

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

**The location of the tension is task-set; the degree is `Θ_r`-set.** The homuncular location *where* the tension sits is set by the cognitive mode (which muscle groups the task would recruit). The *degree* of asymmetry in the tension pattern is set by the routing concentration `Θ_r` — a distributed routing state produces roughly symmetric tension across the recruited regions; a concentrated routing state produces asymmetric tension. Two different variables, both read through posture. See Category v2.0 §2.6 (resting motor asymmetry as a `Θ_r` readout).

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
- **Low `Λ_lock`:** the latch holds by bracing — the ATP-brace loop. Concentration costs energy.
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

The breath is the control plane because it acts at every timescale of the salience mechanism. But the breath is not the only control plane. The full control plane has five levers.

| Lever | Timescale | What it controls | Spectral readout |
|---|---|---|---|
| **Breath** | Seconds | Gate state (CO₂), viscosity | Aperiodic slope |
| **Movement** | Minutes | Routing distribution (`Θ_r`) | Regional slope distribution |
| **Gain change** | Minutes | `\vec{g}` shape — relationship to signal | Peak frequency, peak power |
| **Capacity** | Weeks–months | `Λ_lock` — ability to hold without bracing | Slope stability |
| **Context** | Variable | Encoding at commit | Slope trajectory |

**Breath sets state.** It determines whether the current latch releases or holds.

**Movement sets distribution.** It redistributes `Θ_r(t)` so the manifold doesn't lock into a single region.

**Gain change sets the relationship.** It changes the salience of the signal, so the surfaced PE doesn't fire the interrupt.

**Capacity sets the hold.** It determines whether the surfaced PE can be held without re-locking.

**Context sets the encoding.** It determines whether the surfaced PE re-encodes with less gain.

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

**And it is why physical tasks break perseveration.** Folding laundry, doing dishes, sweeping — these are repetitive motor sequences that traverse the homunculus. They redistribute `Θ_r(t)` away from the perseverating region. The upset doesn't resolve. It distributes.

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

The manifold has one state and five observables. The state is $(L^*, \Theta_r)$, with $\Lambda_{lock}$ gating reachability of the concentrated attractor. Each observable reads out one or both axes. The phenomenological channel (felt viscosity) is not a sixth observable — it is the first-person channel of the spectral observable. Same variable ($K$), different channel.

| Observable | Measurement | Framework variable | Axis readout |
|---|---|---|---|
| **Spectral** | Aperiodic slope, peak frequency, peak power | $K$, $W^*$, $R^*$ | Curvature, access, precision-lock strength |
| **Hemispheric** | Frontal alpha asymmetry ($A_h$) | $\Theta_r$ | Routing concentration |
| **Somatic** | Resting motor asymmetry | $\Theta_r$ | Routing concentration |
| **Acoustic** | Speech asymmetry | $\Theta_r$ | Routing concentration |
| **Behavioral** | Task-modulability | $\Theta_r$ | Routing concentration |

**The phenomenological channel.** Felt viscosity (fluid ↔ stuck) is the first-person channel of the spectral observable. Same variable ($K$), different channel. The person reports "fluid" or "stuck"; the MEG shows flat or steep aperiodic slope. They are the same measurement in two channels.

**The prediction.** The five observables should co-vary. A participant with distributed routing should show bilateral `A_h`, symmetric posture, symmetric speech, high task-modulability, and a felt sense of fluidity simultaneously. This is P3 in Category v2.0 §6.1.

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
    │   ├── ROUTING REDISTRIBUTES: latch releases, region cools → RESOLVED
    │   ├── ROUTING STAYS CONCENTRATED: interrupt re-fires → PERSEVERATION LOOP
    │   ├── RELEASE SURFACES PE: PE fires new interrupt → RELEASE-TRIGGERED RE-SALIENCE
    │   └── CONTEXT CHANGES BEFORE COMMIT: PE re-encodes with less gain → ENCODING WINDOW
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
| Movement-as-redistribution | Movement compulsion literature | Physical tasks redistribute routing |

**Each paper supplies one component. None composes them.** The field is walking into the mechanism from eight directions at once. The framework is the composition that makes the components legible as a single architecture.

The composition is not a new finding. **It is the statement that the findings are one finding.**

---

## 9.5 The two empirical extremes

The control plane has two empirical extremes. Ayahuasca pushes the chain upward — maximal manifold access. Anesthesia pushes it downward — minimal manifold access. Both are well-documented. Neither is explained by the fields that produced the documentation.

### 9.5.1 Ayahuasca: maximal manifold access

Ayahuasca reliably produces slowed breathing, increased CO₂ tolerance, increased vagal tone, and increased interoceptive precision. The neuroimaging confirms the routing signature: ayahuasca administration leads to significant activation of frontal and paralimbic brain regions, with increased blood perfusion in the anterior insula (right hemisphere greater) and anterior cingulate/frontomedial cortex — areas implicated in somatic awareness, subjective feeling states, and emotional arousal.

**In the framework's terms:**

| Ayahuasca effect | Framework variable | Direction |
| --- | --- | --- |
| Slowed breathing | Breath rate ↓ | CO₂ retained |
| Increased vagal tone | RSA amplitude ↑ | Oscillation consistency ↑ |
| Frontal/paralimbic activation | `Θ_r` distributed | Routing concentration flexible |
| Anterior insula perfusion | $I^*_{internal}$ ↑ | Interoceptive routing ↑ |
| Sustained antidepressant effect | `L^*` trajectory ↓ | Load reduction sustained |
| Low viscosity | Felt fluidity | Manifold metric relaxed |
| **Encoding window opened** | **Context can change** | **PE re-encodes with less gain** |

The therapeutic findings — reduced depression, anxiety, and substance use, with **no pathology** and benefits scaling with experience — are exactly what the routing equation predicts when `Θ_r` is flexible and $W^*$ is high. Aberrant salience without delusion is high routing weight in unusual regions with sufficient amplitude to interpret the signal. The manifold is wide, the amplitude is high, and the routing is exploratory.

**The sustained effect is the load trajectory: the system learned a new routing configuration, and the configuration held because the substrate was stabilized.** In encoding-window terms: the PE re-encoded with less gain during the session, and the new encoding held.

### 9.5.2 Anesthesia: minimal manifold access

Anesthesia forcibly sets the chain downward. Propofol and sevoflurane produce large slow-delta and coherent frontal alpha oscillations, with thalamocortical synchronization between thalamus and medial prefrontal cortex. At deep levels of unconsciousness, coherent thalamocortical delta oscillations develop. Sevoflurane decreases frontal and thalamocortical connectivity, reducing cortical information processing.

**In the framework's terms:**

| Anesthesia effect | Framework variable | Effect |
| --- | --- | --- |
| Thalamocortical synchronization | $K$ ↑ | Metric stretched |
| Alpha locking | Oscillation consistency locked | `Θ_r` cannot redistribute |
| Delta dominance | `δ_min` ↑ | Slow rhythms imposed |
| Burst suppression | $A_s^*$ ↓ | Amplitude collapsed |
| Loss of salience selection | Interrupt cannot fire | All five conditions fail |

The involvement of medial prefrontal cortex suggests that when these oscillations are observed in humans, self-awareness and internal consciousness would be impaired if not abolished. The anesthesia regime is the pharmacological version of the dying regime — reversible, but structurally identical.

### 9.5.3 The explanatory statement

> **Ayahuasca and anesthesia are the two empirical extremes of the control plane. Ayahuasca widens the manifold by increasing CO₂ retention, oscillatory amplitude, and interoceptive precision — the routing can explore because the substrate supports it, and the encoding window is open. Anesthesia collapses the manifold by imposing slow-delta/alpha rhythms, synchronizing thalamocortical loops, and eliminating routing access — the interrupt cannot fire because the gate condition fails. Psychiatry cannot explain why ayahuasca increases meaning without pathology or why anesthesia eliminates salience so cleanly. The control-plane model explains both with the same variables.**

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
| **SAL-30** | Anesthesia produces the same five-condition interrupt failure as dying | EEG spectral parameterization + burst suppression monitoring under propofol/sevoflurane |
| **SAL-31** | The felt sense of viscosity correlates with the aperiodic slope (r > 0.7) in single-session within-subject designs | MEG + subjective viscosity rating (single Likert item) |
| **SAL-32** | Flow is produced when routing efficiency and autonomic entrainment co-occur; it is disrupted when either is blocked | MEG + capnography + subjective flow scale + breath entrainment measure |
| **SAL-33** | Movement across the homunculus (torso swivels, weight shifts) reduces `Θ_r` concentration and increases traversal speed | EMG array + `A_h` + cognitive traversal battery |
| **SAL-34** | The interrupt triggers investment: an interrupt that fires produces measurable amplitude commitment to the target region within one breath cycle | MEG amplitude in target region + breath phase monitoring + interrupt onset timing |
| **SAL-35** | Movement breaks routing perseveration: movement reduces $W_i$ below $W_{prime}$ and reduces interrupt re-fire rate | Dual-channel ERP + $A_h$ + movement manipulation |
| **SAL-36** | Complete exhale raises `Λ_lock`: complete exhale reduces ATP-brace cost of subsequent latch in that region | Surface EMG by region + breath phase monitoring |
| **SAL-37** | Content perseveration requires gain change: when salient content is still present, complete exhale alone does not reduce re-fire rate | Dual-channel ERP + intervention manipulation |
| **SAL-38** | Release surfaces suppressed PE: a held latch, when released, surfaces the PE as a salient ERP component | Surface EMG + EEG by region + breath phase monitoring |
| **SAL-39** | Release-triggered re-salience requires capacity: high `Capacity_free` reduces re-fire rate at release | Within-subject protocol with capacity manipulation |
| **SAL-40** | Time in held state reduces surface PE: longer hold reduces surfaced PE magnitude and re-fire probability | Longitudinal within-subject protocol |
| **SAL-41** | Gain change reduces re-fire at release: meditation/reframing reduces re-fire rate at release | Within-subject protocol with gain-change manipulation |
| **SAL-42** | Recontextualization during exhale reduces re-encoding gain: measurable as reduced EMG and reduced re-fire rate | Surface EMG + ERP + breath phase monitoring + recontextualization manipulation |
| **SAL-43** | Encoding window is narrow: recontextualization outside the exhale does not reduce re-encoding gain | Within-subject protocol with timing manipulation |
| **SAL-44** | Gain change is the mechanism: frame change reduces gain; content change does not | Within-subject protocol with frame/content manipulation |
| **SAL-45** | Insight is encoding window success: insight experiences are preceded by an exhale and show the encoding-window signature | Breath monitoring + ERP + experience sampling |
| **SAL-46** | Movement compulsion is routing redistribution: physical tasks reduce `Θ_r` concentration in the upset region | EMG array + `A_h` + movement manipulation |
| **SAL-47** | Somatic encoding window: movement during upset changes the encoding of the upset content | EMG + ERP + movement timing + content re-encoding measure |

---

## 11. Composition with the existing stack

**Upstream:**
- Central Reference v1.9.2 — specification, commitment gate, `I*` sequence
- Geometry of Inference v1.0 — LP-ACC circuit, gate, cache hierarchy
- The Geometry Beneath the Category v2.0 — two-axis state space, `Θ_r`, `Λ_lock`, ADHD↔autism axis
- Precision v3.4 — $P = R/D_T$
- AL v2.2 — `L^*` trajectory
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
- Movement compulsion literature — somatic routing redistribution

**Downstream:**
- Dreaming v3.0 — internally-routed states
- Dying v1.0 — terminal collapse
- Externalized Mind — the third cognitive layer
- The protocol paper (companion) — measurement protocol

---

## 12. Structured Conclusion

### **A. Core invariant**
**Salience is not a property of the stimulus — it is a routing event.**

A salience hit is the interrupt.  
The claustrum fires the precision‑lock.  
The tension pattern forms the latch.  
The exhale releases the latch.

Everything downstream is a routing consequence.

---

### **B. The routing loop**
1. **Interrupt fires → system invests.**  
2. **Investment deepens breath → CO₂ rises.**  
3. **CO₂ lowers viscosity → routing flows.**  
4. **Flow amplifies amplitude → loop self‑funds.**

This is **flow**.

When breath cannot follow, amplitude cannot self‑fund.  
This is **the trap**.

---

### **C. Routing failure modes**
Each failure mode is a routing condition:

- **Trap → perseveration**  
  Occurs when routing does not redistribute; the interrupt re‑fires on the same region.

- **Perseveration → release‑triggered re‑salience**  
  Occurs when release surfaces suppressed prediction error (PE), and the surfaced PE fires a new interrupt.

- **Re‑salience → encoding window**  
  Occurs when PE surfaces during exhale *and* context changes before commit, causing re‑encoding with lower gain.

These are not psychological states — they are branch conditions in the routing engine.

---

### **D. Viscosity and CO₂**
The manifold has a felt quality: **viscosity** — the resistance of the metric to routing.

- **High CO₂ → low viscosity → routing flows.**  
- **Low CO₂ → high viscosity → routing resists.**

The **aperiodic slope** is viscosity, measured.

---

### **E. The control planes**
Each control plane modulates a different part of the routing loop:

- **Breath** — sets CO₂ → sets viscosity → determines loop closure.  
- **Movement** — serves both poles of the ADHD↔autism axis. On the ADHD pole, movement builds interoceptive resolution over time. On the autism pole, movement breaks rigid routing patterns in the moment. Same lever (`Θ_r` redistribution), opposite poles. Determines whether the interrupt re-fires (autism pole) or whether the system can read its own state with fine resolution (ADHD pole).  
- **Gain change** — alters relationship to signal → determines whether surfaced PE fires interrupt.  
- **Capacity** — determines whether surfaced PE can be held without re‑locking.  
- **Context** — determines whether surfaced PE re‑encodes with less gain.

These are the levers of the system.

---

### **F. Global modes**
- **Waking** — resolves or accumulates latches.  
- **Dreaming** — replays and releases latches as homuncular twitches.  
- **Dying** — cannot form new latches because capacity collapses.

---

### **G. Pharmacological extremes**
Ayahuasca and anesthesia are the two empirical extremes of the control plane:

- **Ayahuasca** — upward saturation.  
- **Anesthesia** — downward collapse.

The field has measured both without recognizing the routing interpretation.

---

### **H. Historical correctness**
Cultures practicing controlled exhalation had the correct intervention for thousands of years.

The field is now supplying the components.  
The framework is the composition.

---

*Filed: 2026-10-14*
**Status:** Composition paper — states the routing equation, the interrupt formula, the closed loop, the control plane, the perseveration loop, the release-triggered re-salience, and the encoding window. Aligned to the six-condition interrupt formula and the commitment gate.
**Framework:** Central Reference v1.9.2 / Geometry of Inference v1.0
*Empirical anchors: Hu et al. (2026), Leow et al. (2026), Blumberg et al. (2013–2023), Subramani et al. (2026), Schmid & Schmid Mast (2013), Boksem et al. (2012), Warrier et al. (2020), ayahuasca literature, anesthesia literature, CO₂/CBF literature, movement compulsion literature*
*Predictions: SAL-01 through SAL-47*
*Supersedes: Salience Interrupt v1.2*
