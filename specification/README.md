# `/specification/` — The Mechanism

This folder contains the mechanism itself. Every variable, every equation, and every derivation originates here. Other folders apply the mechanism; this one defines it.

The papers in other folders apply these variables to specific domains. This folder is where the variables come from.

Start with the diagrams. Then the variables. Then the papers.

---

## The Loop

Three states. The output of the first two looks identical from outside. That is the problem.

The loop is the intelligence. These diagrams show the three possible states before any equations appear.

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

---

## The Variables

These six variables govern the loop. Full derivations in the papers below.

---

### R* — Precision
*How tightly the system’s timing streams align.*

$$P = \frac{R}{D_T}$$

**What it measures:** Timing coherence between oscillatory streams. $R$ is sync duration — the proportion of time two streams remain phase-locked. $D_T$ is timing distance — the average phase difference between them.

**What it controls:** Gate behavior. Prediction stability. Whether the loop can detect an error worth running on.

**What happens when it fails:** The loop cannot distinguish signal from noise. Prediction errors below threshold don't register. The system runs on priors. Confident output with no sensory grounding.

**Derived in:** [Precision, Timing, and the Oscillatory Source v3.5]

---

### W* — Window Width
*How many nodes the system can hold at once.*

**What it measures:** How many nodes the system holds simultaneously during inference. The prediction window — how far ahead and how many threads remain active.

**What it controls:** Integration depth. Cross-domain synthesis. The ability to hold a complex structure long enough to find errors in it.

**What happens when it fails:** The system can only process what fits in a narrow window. Cross-domain connections become invisible. First-pass pattern matching dominates. Collapsed loop behavior increases.

**Derived in:** [Manifold Schema v7.2], [Geometry of Inference v1.0]

---

### A* — Amplitude
*How much oscillatory energy the system has available to run inference.*

$$A_s^* = f(\text{breath mechanics}, \text{CO}_2\text{ tolerance}, \text{HRV})$$

**What it measures:** Oscillatory depth available for inference. The raw energy budget the system can deploy.

**What it controls:** The ceiling on everything downstream. W*, R*, and Θ* are all bounded by A*. A system with low amplitude cannot sustain the loop regardless of other variables.

**What happens when it fails:** The system shifts from exploration to conservation. Window narrows. Precision drops. The loop runs shorter cycles. Collapse modes become default.

**Derived in:** [Manifold Schema v7.2], [Physics as the Missing Component]

---

### L* — Load
*How much regulatory debt the system is carrying over time.*

$$\Delta HRV \propto \frac{1}{L^*}$$

$$L^{\ast} = w_1 L^{\ast}_{HRV} + w_2 L^{\ast}_{RHR} + w_3 L^{\ast}_{temp} + w_4 L^{\ast}_{inflam} + w_5 L^{\ast}_{resp}$$


**What it measures:** Accumulated regulatory debt. Not a state — a trajectory. Load is what happens when reinvestment falls below the threshold required to maintain the loop.

**What it controls:** The constraint on all other variables. L* is the denominator. As it rises, everything else compresses.

**What happens when it fails:** The system calcifies. Prediction windows close. Collapse modes become permanent rather than transient. FND, chronic fatigue, depression, and cognitive narrowing are geometric predictions of high L*.

**Derived in:** [Allostatic Load as Accumulated Regulatory Debt v2.1]

---

### Θ* — Integration Efficiency
*How cleanly one layer’s output transfers to the next.*

**What it measures:** How cleanly outputs from one layer feed the next. The transfer function between oscillatory streams.

**What it controls:** Multi-hop reasoning depth. Whether a complex inference chain completes or leaks at each handoff.

**What happens when it fails:** Reasoning chains terminate early. Outputs from one layer don't propagate cleanly to the next. The loop runs but loses signal at each hop. Intelligence product drops even when Λ is high.

**Derived in:** [Precision v3.5], [Loop Is the Intelligence v1.0]

---

### Λ — The Gate
*Whether the inference loop is running at all.*

**What it measures:** Whether the loop is running at all. Binary at the threshold, graded above it.

**What it controls:** Everything. Λ = 0 means no loop. No loop means no intelligence product regardless of other variables.

**Critical constraint:** Λ is itself a function of C_s. Without sufficient right-hemisphere precision, sensory feedback cannot register. The loop cannot start if the system cannot detect that there is an error worth running on.

$$C_s = \left(A_s^{\ast 0.15} \cdot R^{\ast 0.30} \cdot W^{\ast 0.25} \cdot \Theta^{\ast 0.15}\right)^{\frac{1}{0.85}} \cdot \frac{1}{1 + L^{\ast}}$$

**What happens when it fails:** The system produces fluent output from pattern completion. Speed is high. The loop is not running. Indistinguishable from genuine inference until the task requires transfer.

**Derived in:** [Central Reference v1.6], [Manifold Schema v7.2]

---

## The Derivation Chain

```
CENTRAL REFERENCE v1.6
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
│   └── ALLOSTATIC LOAD v2.1
│       L* as trajectory. Four contracts.
│       ΔHRV as primary real-time proxy.
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

| If you want                 | Start here                         |
| --------------------------- | ---------------------------------- |
| The full specification      | [Central Reference v1.6]           |
| The manifold foundation     | [Manifold Schema v7.2]             |
| The precision derivation    | [Precision v3.5]                   |
| The load trajectory         | [Allostatic Load v2.1]             |
| The gate mechanism          | [Geometry of Inference v1.0]       |
| The intelligence definition | [Loop Is the Intelligence v1.0]    |
| The physical invariants     | [Physics as the Missing Component] |

---

*These papers define the variables. The papers in `/ai/`, `/domains/`, and `/implementation/` use them.*
