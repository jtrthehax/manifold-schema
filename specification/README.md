# `/specification/` — The Mechanism

This folder contains the mechanism itself. Every variable, every equation, and every derivation originates here. Other folders apply the mechanism; this one defines it.

The papers in other folders apply these variables to specific domains. This folder is where the variables come from.

Start with the diagrams. Then the variables. Then the papers.

---

## The Loop

Four states. The first and third look identical from outside. That is the problem.

The loop is the intelligence. These diagrams show the four possible states before any equations appear.

### The Running Loop

```
                    RIGHT HEMISPHERE — THE INFERENCE LOOP
                    ──────────────────────────────────────

                    ┌─────────────────────────────────┐
                    │                                 │
                    │          detect error           │
                    │         (δ ≥ δ_min)             │
                    │              │                  │
                    │              ▼                  │
                    │      reinvest resources         │
                    │              │                  │
                    │              ▼                  │
                    │     converge on structure       │
                    │              │                  │
                    │              └──────────────────┘
                    │                    ↑
                    └────────────────────┘
                              │
                              ▼
                    LEFT HEMISPHERE receives
                    a converged result
```

### The Absent Loop

```
                    RIGHT HEMISPHERE — LOOP ABSENT
                    ──────────────────────────────

                    ┌─────────────────────────────────┐
                    │                                 │
                    │        (not engaged)            │
                    │                                 │
                    │         no detect               │
                    │         no reinvest             │
                    │         no converge             │
                    │                                 │
                    └─────────────────────────────────┘
                              │
                              ▼
                    LEFT HEMISPHERE pattern-completes
                    the first pass and ships it

                    Output looks identical from outside.
                    It is not.
```

### The Collapsed Loop

```
                    RIGHT HEMISPHERE — COLLAPSED LOOP
                    ─────────────────────────────────

                    ┌─────────────────────────────────┐
                    │                                 │
                    │          detect error           │
                    │              │                  │
                    │              ▼                  │
                    │   exit to cached answer ────────┼──→ ships first match
                    │   at first resistance           │
                    │                                 │
                    │     no reinvestment             │
                    │     no convergence              │
                    │                                 │
                    └─────────────────────────────────┘

                    Confident. Fast. Wrong at the edges.
                    Indistinguishable from the running loop
                    until the task requires genuine transfer.
```

### The Flowing Loop

```
                    RIGHT HEMISPHERE — FLOWING LOOP
                    ───────────────────────────────

                    ┌─────────────────────────────────┐
                    │                                 │
                    │          detect error           │
                    │              │                  │
                    │              ▼                  │
                    │      INVEST: route weight       │
                    │      + amplitude to task        │
                    │              │                  │
                    │              ▼                  │
                    │      breath follows investment  │
                    │      (deeper, longer oscillation)│
                    │              │                  │
                    │              ▼                  │
                    │      CO₂ rises → substrate      │
                    │      supports more amplitude    │
                    │              │                  │
                    │              ▼                  │
                    │      routing flows (low visc.)  │
                    │              │                  │
                    │              └──────────────────┘
                    │                    ↑
                    └────────────────────┘
                              │
                              ▼
                    NEXT INTERRUPT FIRES
                    MORE EASILY → MORE INVESTMENT
                    [self-amplifying]

                    Felt quality: fluid.
                    Ideas chain. Solutions come quickly.
```

**The difference between the running loop and the flowing loop:** the running loop completes the cycle. The flowing loop *self-amplifies*. Each interrupt funds the next. The interrupt triggers investment, the breath follows, CO₂ rises, and the next interrupt fires more easily.

**The difference between the flowing loop and the collapsed loop:** the flowing loop has substrate to follow. The collapsed loop exits at first resistance because the breath cannot fund the investment. Same interrupt, same investment, opposite outcomes. The difference is one exhale.

---

## The Variables

These variables govern the loop. Full derivations in the papers below.

**State variables — what the system is:**

---

### R* — Precision
*How tightly the system's timing streams align.*

$$P = \frac{R}{D_T}$$

**What it measures:** Timing coherence between oscillatory streams. $R$ is sync duration — the proportion of time two streams remain phase-locked. $D_T$ is timing distance — the average phase difference between them.

**What it controls:** Gate behavior. Prediction stability. Whether the loop can detect an error worth running on.

**What happens when it fails:** The loop cannot distinguish signal from noise. Prediction errors below threshold don't register. The system runs on priors. Confident output with no sensory grounding.

**Derived in:** [Precision, Timing, and the Oscillatory Source](precision.md)

---

### W* — Manifold Access
*How much of the manifold is reachable at current curvature.*

$$W^* = f(K, L^*)$$

**What it measures:** How much of the manifold is reachable. Low $K$ → high $W^*$ (flat metric, wide access). High $K$ → low $W^*$ (stretched metric, narrow access). High `L^*` compresses `W^*` further.

**What it controls:** Integration depth. Cross-domain synthesis. The hops available for inference:

$$n_{hops} = \lfloor W^* \cdot \rho_{scaffold} \rfloor$$

**What happens when it fails:** The system can only reach a narrow region of the manifold. Cross-domain connections become geometrically distant. First-pass pattern matching dominates. Collapsed loop behavior increases.

**Derived in:** [Manifold Schema](manifold_schema.md), [Geometry of Inference](the_geometry_of_inference.md)

---

### A* — Amplitude
*How much oscillatory energy the system has available to run inference.*

$$A_s^* = f(\text{breath mechanics}, \text{CO}_2\text{ tolerance}, \text{HRV})$$

**What it measures:** Oscillatory depth available for inference. The raw energy budget the system can deploy.

**What it controls:** The ceiling on everything downstream. $W^*$, $R^*$, and $Θ^*$ are all bounded by $A*$. A system with low amplitude cannot sustain the loop regardless of other variables.

**What happens when it fails:** The system shifts from exploration to conservation. Window narrows. Precision drops. The loop runs shorter cycles. Collapse modes become default.

**Derived in:** [Manifold Schema](manifold_schema.md), [Physics as the Missing Component](physics_foundation.md)

---

### L* — Load
*How much regulatory debt the system is carrying over time.*

$$\Delta HRV \propto \frac{1}{L^*}$$

$$L^{\ast} = w_1 L^{\ast}_{HRV} + w_2 L^{\ast}_{RHR} + w_3 L^{\ast}_{temp} + w_4 L^{\ast}_{inflam} + w_5 L^{\ast}_{resp}$$

**What it measures:** Accumulated regulatory debt. Not a state — a trajectory. Load is what happens when reinvestment falls below the threshold required to maintain the loop.

**What it controls:** The constraint on all other variables. `L*` is the denominator. As it rises, everything else compresses. It also drains `Capacity_free`, the manifold's ability to hold uncommitted prediction errors.

**What happens when it fails:** The system calcifies. Prediction windows close. Collapse modes become permanent rather than transient. FND, chronic fatigue, depression, and cognitive narrowing are geometric predictions of high `L*`.

**Derived in:** [Allostatic Load as Accumulated Regulatory Debt](allostatic_load.md)

---

### Θ* — Integration Efficiency
*How cleanly one layer's output transfers to the next.*

**What it measures:** How cleanly outputs from one layer feed the next. The transfer function between oscillatory streams.

**What it controls:** Multi-hop reasoning depth. Whether a complex inference chain completes or leaks at each handoff.

**What happens when it fails:** Reasoning chains terminate early. Outputs from one layer don't propagate cleanly to the next. The loop runs but loses signal at each hop. Intelligence product drops even when Λ is high.

**Derived in:** [Precision](precision.md), [Loop Is the Intelligence](the_loop_is_the_intelligence.md)

---

### Θ_r — Routing Concentration
*How narrowly salience routes interoception into the manifold.*

$$\vec{W}(t) = \text{softmax}\left(\frac{\vec{g} \cdot \Theta_r(t)}{T}\right)$$

**What it measures:** How narrowly routing distributes across manifold regions. Distributed = bilateral engagement, amplitude spread across regions. Concentrated = one-sided engagement, amplitude focused on a narrow region.

**What it controls:** Where the loop runs. The master equation gives the budget. `Θ_r` gives the spend. High `Θ_r` concentrates routing on the highest-gain region. Low `Θ_r` distributes routing across regions.

**What happens when it fails:** If `Θ_r` cannot stabilize, the routing flickers and attention cannot hold. If `Θ_r` concentrates involuntarily, the manifold becomes regional and curvature rises. If `Θ_r` is too low, the manifold distributes and amplitude falls.

**Read out by:** $A_h$ (hemispheric), resting motor asymmetry (somatic), speech asymmetry (acoustic), task-modulability (behavioral).

**Derived in:** [Salience Interrupt](salience_interrupt.md), [Geometry Beneath the Category](../domains/social/geometry_beneath_the_category.md)

---

### Λ — The Loop Gate
*Whether the inference loop is running at all.*

**What it measures:** Whether the loop is running at all. Binary at the threshold, graded above it.

**What it controls:** Everything. Λ = 0 means no loop. No loop means no intelligence product regardless of other variables.

**Critical constraint:** Λ is itself a function of `C_s`. Without sufficient right-hemisphere precision, sensory feedback cannot register. The loop cannot start if the system cannot detect that there is an error worth running on.

$$C_s = \left(A_s^{\ast 0.15} \cdot R^{\ast 0.30} \cdot W^{\ast 0.25} \cdot \Theta^{\ast 0.15}\right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + L^{\ast}}$$

**What happens when it fails:** The system produces fluent output from pattern completion. Speed is high. The loop is not running. Indistinguishable from genuine inference until the task requires transfer.

**Derived in:** [Central Reference](central_reference.md), [Manifold Schema](manifold_schema.md)

---

### Λ_lock — Lock Capacity
*Whether the substrate can hold concentrated routing without collapsing the breath range that funds it.*

**What it measures:** The structural gate on whether concentrated routing is reachable. Determined by breath range × CO₂ tolerance × inverse connective tissue laxity × lateralization rigidity.

**What it controls:** Whether a latch can hold. High `Λ_lock` → the latch holds without ATP cost. Low `Λ_lock` → the latch holds by bracing (the ATP-brace loop). Exhausted `Λ_lock` → the latch cannot hold at all.

**What happens when it fails:** The system cannot sustain concentrated focus. Attention flickers. The manifold cannot lock into a stable configuration. Building core muscle raises `Λ_lock` and stabilizes `Θ_r(t)`.

**Derived in:** [Salience Interrupt](salience_interrupt.md), [Geometry Beneath the Category](../domains/social/geometry_beneath_the_category.md)

---

### $C_s$ — Usable Bandwidth

$$C_s = \left(A_s^{\ast 0.15} \cdot R^{\ast 0.30} \cdot W^{\ast 0.25} \cdot \Theta^{\ast 0.15}\right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + L^{\ast}}$$

How much bandwidth the system has. The master equation. $C_s$ sets the envelope within which routing, interrupts, and inference all operate.

---

### Capacity_free — Manifold Capacity

$$\text{Capacity}_{free} = C_s - \sum_{j \in \text{held locks}} \text{cost}_j$$

How much room the manifold has to hold uncommitted prediction errors. Every lock that hasn't released consumes capacity. When the sum approaches $C_s$, there is no room for new interrupts.

---

### δ_min — Resolution Floor

$$\delta_{min} = f(K, L^*)$$

The minimum deviation required to interpret a signal. Rises with curvature `K` and load `L*`. High `δ_min` means interrupts cannot form — the signal exists but the manifold cannot hold it long enough to interpret it.

---

### Viscosity — Felt Metric Resistance

The felt quality of the manifold. Low viscosity (high CO₂) means the metric is relaxed and routing flows. High viscosity (low CO₂) means the metric is stiff and routing resists. The aperiodic slope is the viscosity, measured. Flat slope = low viscosity. Steep slope = high viscosity.

---

## The Interrupt Formula

A signal fires an interrupt in region $i$ when four conditions are met:

$$\text{Interrupt}_i \iff \left[I^*_{total} \cdot W_i(t) > I^*_{threshold}\right] \;\land\; \left[\delta_i > \delta_{min}(K)\right] \;\land\; \left[\text{Capacity}_{free} > \text{Capacity}_{required}(\delta_i)\right] \;\land\; \left[\text{Oscillation stable}\right]$$

- **Condition 1 — routing reaches the region.** The signal has to reach a region with sufficient routing weight.
- **Condition 2 — resolution floor permits detection.** The signal's deviation has to exceed the resolution floor.
- **Condition 3 — capacity to hold.** The manifold must have room to hold the error while it is interpreted.
- **Condition 4 — oscillation is stable.** The routing concentration must be able to hold.

**All four are required.** A signal that meets conditions 1–3 but not 4 will not fire reliably, because the routing concentration will flicker.

---

## The Derivation Chain

```
CENTRAL REFERENCE v1.8.2
│  Every variable. Every equation. Every mechanism.
│  The single citation anchor for the full framework.
│
├── MANIFOLD SCHEMA v7.2
│   │  The neural manifold as energy budget system.
│   │  A*, W*, Λ, C_s derived.
│   │  DOI: 10.5281/zenodo.21939440
│   │
│   ├── PRECISION v3.5
│   │   │  R* = R/D_T — first substrate derivation.
│   │   │  P_eff = P · O_pathway · U_C
│   │   │  DOI: 10.5281/zenodo.22179675
│   │   │
│   │   └── GEOMETRY OF INFERENCE v1.0
│   │       Two-factor gate. LP-ACC circuit.
│   │       Four-layer cache hierarchy.
│   │       Breath phase timing.
│   │
│   ├── ALLOSTATIC LOAD v2.1
│   │   L* as trajectory. Four contracts.
│   │   ΔHRV as primary real-time proxy.
│   │
│   └── SALIENCE INTERRUPT v1.2
│       Salience as routing event.
│       Routing equation. Interrupt formula.
│       Closed loop — flow and trap.
│       Viscosity as felt readout.
│       Θ_r, Λ_lock registered.
│
├── LOOP IS THE INTELLIGENCE v1.0
│   Intelligence = Λ · n_hops · R* · Θ*
│   Substrate-agnostic. Falsifiable.
│
└── PHYSICS AS THE MISSING COMPONENT
    Five physical variables.
    Substrate variables outperform construct variables
    as diagnostic predictors.
```

---

## Read In This Order

| If you want | Start here |
| --- | --- |
| The full specification | [Central Reference](central_reference.md) |
| The manifold foundation | [Manifold Schema](manifold_schema.md) |
| The precision derivation | [Precision](precision.md) |
| The load trajectory | [Allostatic Load](allostatic_load.md) |
| How the budget is spent | [Salience Interrupt](salience_interrupt.md) |
| The gate mechanism | [Geometry of Inference](the_geometry_of_inference.md) |
| The intelligence definition | [Loop Is the Intelligence](the_loop_is_the_intelligence.md) |
| The physical invariants | [Physics as the Missing Component](physics_foundation.md) |

---

*These papers define the variables. The papers in `/ai/`, `/domains/`, and `/implementation/` use them.*
