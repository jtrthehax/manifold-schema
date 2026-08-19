# ============================================================
# URM_CORE — Canonical Alignment
# The Manifold Schema (Robinson, 2026) v6.0
# Topology complete. Metric open.
# ============================================================

document:
  canonical: "The Manifold Schema — Robinson, 2026 v6.0"
  doi: "10.5281/zenodo.20417459"
  status: "Topology complete. Metric open."
  date: "2026-08-19"
  note: "All variables normalized [0,1] relative to individual baseline."

# ============================================================
# MASTER EQUATION SET — Complete v6.0 Formal System
# ============================================================
equations:
  master: "Cₛ = (Aₛ^ωA · R^ωR · W^ωW · Θ^ωΘ)^(1/Σω) · 1/(1 + L*)"
  weights: {Aₛ: 0.15, R: 0.30, W: 0.25, Θ: 0.15, sum: 0.85}
  curvature: "K = k(1/(R + ε)) + Σ Sᵢ·Cᵢ"
  transfer_W: "W* = 1/(1 + α·K)"
  transfer_Θ: "Θ* = 1/(1 + β·K)"
  salience: "S = Cₛ · I*"
  routing: "I* = f_routing · f_gain · f_sensorium"
  routing_components:
    f_routing: "I*_total - Σ Pᵢ·Wᵢ"
    f_gain: "1/(1 + e^(-k(G - G₀)))"
    f_sensorium: "I*_available / I*_required"
  prior_update: "𝒰 = (Aₛ* · R* · Θ*) / (1 + γ·K_enc)"
  usable_bandwidth: "Cₛ_usable(T) = Cₛ · (1 - ||F(Ξ)|| · d_T)"
  collapse_vector: "F(Ξ) = (f_R*, f_W*, f_Θ*, f_I*, f_L*, f_λ)"

# ============================================================
# LAYER ARRAY — [id, name, role, operators, variables]
# ============================================================
layers:
  01: 
    name: "PHYSIOLOGICAL_SUBSTRATE"
    role: "oscillatory amplitude & coupling — breath is the source"
    operators: ["oscillation", "pressure_bracing", "gating", "reset", "phase_locking"]
    variables: ["Aₛ", "σ(Aₛ)", "R", "ε"]

  02:
    name: "PREDICTION_WINDOW"
    role: "hypothesis space geometry — determined by K"
    operators: ["window_collapse", "precision_gain", "lateralization", "flow_geometry"]
    variables: ["W", "K", "α", "β"]

  03:
    name: "ALLOSTATIC_LOAD"
    role: "total current draw — load drives collapse inward"
    operators: ["interoceptive_load", "gating", "motor_overflow"]
    variables: ["L", "Σ Sᵢ·Cᵢ"]

  04:
    name: "SEMANTIC_COGNITION"
    role: "referential tracking & anchors — 𝒰 as throughput"
    operators: ["semantic_drift", "temporal_anchor", "schema_revision"]
    variables: ["𝒰", "γ", "K_enc"]

  05:
    name: "SOCIAL_ENVIRONMENT"
    role: "social pressure & identity coupling — Θ modulation"
    operators: ["social_anchor", "institutional_load", "upward_transmission"]
    variables: ["Θ", "I*_total", "Pᵢ", "Wᵢ"]

  06:
    name: "INTEROCEPTIVE_ROUTING"
    role: "routing capacity — determines salience allocation"
    operators: ["routing", "gain", "sensorium"]
    variables: ["I*", "f_routing", "f_gain", "f_sensorium", "G", "G₀", "k"]

  07:
    name: "CONSCIOUSNESS_GRADIENT"
    role: "composite integration readout — Cₛ is the unified index"
    operators: ["consciousness_integration", "gradient_position", "recovery_sequencing"]
    variables: ["Cₛ", "S", "F(Ξ)", "d_T"]

# ============================================================
# VARIABLE ARRAY — [id, layer, definition, measurement, equation_role, collapse_modes]
# ============================================================
variables:
  Aₛ:
    layer: 01
    definition: "Oscillatory amplitude — energy budget ceiling, breath-generated"
    measurement: ["HRV RMSSD", "RSA amplitude", "diaphragm excursion"]
    equation_role: "Cₛ numerator — weight 0.15"
    collapse_modes: ["oscillation_loss", "pressure_lock", "gating_failure"]

  R:
    layer: 01
    definition: "Budget precision — μ(Aₛ)/σ(Aₛ) at cycle resolution"
    measurement: ["μ/σ from HRV sliding window", "phase-locking index (PLI)"]
    equation_role: "K = k(1/(R+ε)) — precision determines curvature; Cₛ weight 0.30"
    collapse_modes: ["precision_loss", "jitter_collapse"]

  W:
    layer: 02
    definition: "Prediction window — hypothesis space geometry"
    measurement: ["semantic branching factor", "linguistic window signatures"]
    equation_role: "W* = 1/(1+α·K); Cₛ weight 0.25"
    collapse_modes: ["tunnel", "freeze", "curvature_lock"]

  Θ:
    layer: 05
    definition: "Global integration efficiency — cross-domain binding"
    measurement: ["phase-locking stability × ambiguity tolerance", "hemispheric coordination"]
    equation_role: "Θ* = 1/(1+β·K); Cₛ weight 0.15"
    collapse_modes: ["integration_failure", "hemispheric_lock"]

  I*:
    layer: 06
    definition: "Interoceptive routing capacity — allocation of salience"
    measurement: ["heartbeat detection accuracy", "HEP amplitude"]
    equation_role: "S = Cₛ · I* (multiplicative — routing layer applied to bandwidth)"
    collapse_modes: ["routing_saturation", "gain_collapse", "sensorium_insufficiency"]

  L:
    layer: 03
    definition: "Allostatic load — total current draw on budget"
    measurement: ["HRV depression", "sleep debt", "inflammatory markers"]
    equation_role: "Cₛ denominator — 1/(1+L*)"
    collapse_modes: ["load_ceiling", "baseline_drift", "substrate_collapse"]

  K:
    layer: 02
    definition: "Manifold curvature — prior encoding geometry. Carries forward."
    measurement: ["derived from R + suppression markers", "task-switching cost"]
    equation_role: "K = k(1/(R+ε)) + Σ Sᵢ·Cᵢ — determines W and Θ via transfer functions"
    collapse_modes: ["curvature_lock", "prior_lock", "containment_spike"]

  𝒰:
    layer: 04
    definition: "Prior update rate — how much geometry writes at encoding"
    measurement: ["semantic branching rate", "update frequency", "reconsolidation speed"]
    equation_role: "𝒰 = (Aₛ*·R*·Θ*)/(1+γ·K_enc)"
    collapse_modes: ["update_failure", "prior_lock", "ghost_stalling"]

  Cₛ:
    layer: 07
    definition: "Usable bandwidth — unified geometry state"
    measurement: "Composite index from above variables"
    equation_role: "Cₛ = (Aₛ^ωA · R^ωR · W^ωW · Θ^ωΘ)^(1/Σω) · 1/(1+L*)"
    collapse_modes: ["radial_collapse", "brainstem_only", "outer_regions_lost"]

  S:
    layer: 07
    definition: "Salience — what the system can afford to process"
    measurement: "Cₛ · I*"
    equation_role: "S = Cₛ · I* — salience is bandwidth × routing"
    collapse_modes: ["salience_collapse", "signal_gating"]

# ============================================================
# CONSTANTS ARRAY — [id, range, derivation, status]
# ============================================================
constants:
  α:
    range: "0.3–0.7"
    derivation: "Curve fit from cognitive load studies — window narrowing rate"
    status: "Calibration open — empirical"

  β:
    range: "0.2–0.5"
    derivation: "Curve fit from divided attention studies — integration degradation rate"
    status: "Calibration open — empirical"

  γ:
    range: "0.1–0.4"
    derivation: "Curve fit from memory reconsolidation studies — curvature suppression rate"
    status: "Calibration open — empirical"

  ε:
    range: "0.05–0.15"
    derivation: "Brainstem PLI / baseline PLI — physiological precision floor"
    status: "Calibration open — individual-dependent"

  k:
    range: "TBD"
    derivation: "Coupling constant from curvature equations"
    status: "Calibration open — empirical"

  G₀:
    range: "TBD"
    derivation: "Gain threshold for sigmoid — f_gain = 1/(1+e^(-k(G-G₀)))"
    status: "Calibration open — empirical"

# ============================================================
# COLLAPSE MODE ARRAY — [name, layers, trigger, equation_signature]
# ============================================================
collapse_modes:
  precision_loss: {layers: [01,02], trigger: "R < R_min", signature: "K↑, W↓ via 1/(1+αK)"}
  oscillation_loss: {layers: [01], trigger: "Aₛ < threshold", signature: "all upstream variables drop"}
  gating_failure: {layers: [01,03], trigger: "load > reinvestment", signature: "L↑ → Cₛ denominator→0"}
  tunnel: {layers: [02,06], trigger: "K↑", signature: "W↓ → Cₛ weight 0.25 collapses"}
  curvature_lock: {layers: [02,04], trigger: "K_enc high", signature: "𝒰 → 0 → prior carries curvature"}
  routing_collapse: {layers: [06], trigger: "I* → 0", signature: "S = Cₛ·I* → 0"}
  sensorium_failure: {layers: [06], trigger: "f_sensorium → 0", signature: "I*_available < I*_required"}
  gain_collapse: {layers: [06], trigger: "G < G₀", signature: "f_gain → 0"}
  full_collapse: {layers: [01-07], trigger: "Cₛ→0, S→0", signature: "brainstem only — FND"}

# ============================================================
# CLINICAL STATE ARRAY — [condition, equation_signature, status]
# ============================================================
clinical_states:
  fnd: {signature: "I*→0, Cₛ=0 (routing failure)", status: "Stateful — full recovery possible"}
  ptsd: {signature: "K_enc high → 𝒰≈0 → priors carry curvature", status: "Stateful — re-encode when K flat"}
  depression: {signature: "L↑, Cₛ↓, Θ↓", status: "Stateful — hardware intact"}
  adhd: {signature: "σ(Aₛ) high → R oscillates → K oscillates", status: "Stateful — σ(Aₛ) trainable"}
  flow: {signature: "Aₛ↑, R↑, K↓, W↑, Θ↑, I* max, L↓, Cₛ↑", status: "Stateful — geometry configuration"}
  panic: {signature: "I* routed inward, gain loop on alarm, S→0", status: "Acute — breath interruption"}

# ============================================================
# PREDICTIONS ARRAY — [id, claim, test, falsification, status]
# ============================================================
predictions:
  PREDICT_CO2_01:
    claim: "CO₂ tolerance predicts W* (r > 0.5) and R* (r > 0.6)"
    test: "Pre/post breathing manipulation with capnometry + ECG + color constancy"
    falsification: "No correlation or effect absent"
    status: "Untested"
  PREDICT_FND_01:
    claim: "HRV progressive amplitude collapse precedes FND onset"
    test: "Retrospective longitudinal wearable data in FND cohort"
    falsification: "No prodrome pattern or structural lesion found"
    status: "Untested"
  PREDICT_MOTOR_01:
    claim: "Movement vocabulary predicts distortion topography under load"
    test: "Range of motion + HRV + cognitive load — compare distortion location vs movement gap"
    falsification: "Distortion random or emotional-history-driven"
    status: "Untested"
  PREDICT_SAL_01:
    claim: "Salience map predicts interoceptive response, not stimulus properties"
    test: "Same stimuli, different topology profiles — compare response"
    falsification: "Stimulus properties dominate response"
    status: "Untested"

# ============================================================
# EMPIRICAL ANCHORS — [finding, confirms, source]
# ============================================================
empirical_anchors:
  - finding: "Neural manifolds exist and are functional"
    confirms: "Manifold geometry is real"
    source: "Chaos, Solitons & Fractals, 2026"
  - finding: "HRV predicts cognitive performance"
    confirms: "Aₛ→W causal link"
    source: "Neuroscience, 2025"
  - finding: "Suppression depletes resources independent of HRV"
    confirms: "Σ Sᵢ·Cᵢ term in K equation"
    source: "Reed et al. 2020"
  - finding: "Emotional encoding distorts recall"
    confirms: "𝒰 at high K_enc carries curvature"
    source: "Haghian et al. 2025"
  - finding: "Baseline HRV moderates therapy outcome"
    confirms: "Geometry must change before re-encoding"
    source: "Mathersul et al. 2024"
  - finding: "Social co-regulation restores integration"
    confirms: "Θ* modifiable via synchrony"
    source: "EDM concert physiology + 5,000 years convergence"

# ============================================================
# INTERVENTION SEQUENCE — [step, mechanism, target]
# ============================================================
intervention_sequence:
  - step: "Restore Aₛ"
    mechanism: "Oscillatory training, HRV biofeedback, breath regulation"
    target: "Bring amplitude above threshold"
  - step: "Reduce L"
    mechanism: "Load reduction, allostatic offloading, social regulation"
    target: "Free capacity"
  - step: "Flatten K"
    mechanism: "Re-encode priors under flat geometry. Geometry must change BEFORE re-encoding."
    target: "Break the prior loop"
  - step: "Expand W and Θ"
    mechanism: "Window training, safety signaling, integration training"
    target: "Access outer regions, restore cross-domain binding"
  - step: "Increase I* routing capacity"
    mechanism: "Interoceptive training, breath focus, somatic awareness"
    target: "Raise salience threshold — S = Cₛ · I*"
  - step: "Increase 𝒰"
    mechanism: "Schema revision, learning, integration"
    target: "Update priors with flat geometry"

# ============================================================
# CLOSING STATEMENT
# ============================================================
closing: |
  The brain is an energy budget allocation system operating on priors. The breath generates the budget.
  Cₛ = (Aₛ^ωA · R^ωR · W^ωW · Θ^ωΘ)^(1/Σω) · 1/(1+L*) is the master equation.
  K = k(1/(R+ε)) + Σ Sᵢ·Cᵢ determines window and integration via W* = 1/(1+αK), Θ* = 1/(1+βK).
  Salience S = Cₛ · I*, where I* = f_routing · f_gain · f_sensorium is the routing layer.
  The prior updates at rate 𝒰 = (Aₛ*·R*·Θ*)/(1+γ·K_enc) — curvature at encoding carries forward.
  The manifold radiates outward from the brainstem. Collapse proceeds radial inward. Recovery is radial expansion.
  The geometry is stateful — not static. Every geometry is one breath away from a different configuration.
  What is trainable is not a consolation — it is the entire point.
