# COMBO_0063 - Neuroscience Cortical Circuits

## Scientific Question
How do cortical circuit motifs transform and propagate activity?

## Biological Context
Neuronal dynamics, network signaling, and emergent circuit behavior.

## Mechanistic Assumptions
- Model implementations are used as published in their curated manifests without biological reinterpretation.
- Time integration uses a shared global tick compatible with model min_dt constraints.
- Comparative (non-causal) mode is used because full deterministic IO coverage for causal coupling was not satisfied.

## Why These Models Belong Together
The combination was selected from a shared domain/theme bucket with deterministic compatibility checks.
- `neuroscience-other-58195-58195-model`: Neuroscience: Model5819558195Model
- `neuroscience-other-58199-58199-model`: Neuroscience: Model5819958199Model
- `neuroscience-other-58581-58581-model`: Neuroscience: Model5858158581Model
- `neuroscience-other-58582-58582-model`: Neuroscience: Model5858258582Model

## Wiring Rationale
- Comparative (non-causal) mode: no direct causal links were created.

## Visualization Strategy
- Monitor-driven visualization is required for this space.
- State streams are routed into explicit monitor ports (`state_a..state_d`) to avoid signal overwrite.
- At minimum, monitor visuals include one timeseries panel and one summary table.
- Rationale: A dedicated monitor model receives all participating model state streams (`state_a..state_d`) so trajectories can be compared in one place without claiming causal coupling when IO semantics are incomplete.

## Expected Behaviors
- Model output trajectories under shared runtime settings.
- Cross-model agreement/divergence in key state or metric signals.
- Relative behavior comparison without causal linkage claims.

## Known Limitations
- No new biology is introduced beyond what upstream models encode.
- Cross-model semantic matching is rule-based and may under-connect uncertain routes.

## Source Provenance
- neuroscience-other-58195-58195-model :: opensourcebrain:58195 :: https://github.com/OpenSourceBrain/58195
- neuroscience-other-58199-58199-model :: opensourcebrain:58199 :: https://github.com/OpenSourceBrain/58199
- neuroscience-other-58581-58581-model :: opensourcebrain:58581 :: https://github.com/OpenSourceBrain/58581
- neuroscience-other-58582-58582-model :: opensourcebrain:58582 :: https://github.com/OpenSourceBrain/58582

## How to Run
```bash
python run_local.py --duration auto --tick-dt auto
```

## How to Interpret Outputs
Use output trajectories and summary metrics to compare mechanistic consistency across constituent models.
Interpret comparative spaces as non-causal side-by-side simulation views.
