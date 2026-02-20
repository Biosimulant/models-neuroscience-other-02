# COMBO_0062 - Neuroscience Cortical Circuits

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
- `neuroscience-other-56012-56012-model`: Neuroscience: Model5601256012Model
- `neuroscience-other-57905-57905-model`: Neuroscience: Model5790557905Model
- `neuroscience-other-57910-57910-model`: Neuroscience: Model5791057910Model
- `neuroscience-other-58172-58172-model`: Neuroscience: Model5817258172Model

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
- neuroscience-other-56012-56012-model :: opensourcebrain:56012 :: https://github.com/OpenSourceBrain/56012
- neuroscience-other-57905-57905-model :: opensourcebrain:57905 :: https://github.com/OpenSourceBrain/57905
- neuroscience-other-57910-57910-model :: opensourcebrain:57910 :: https://github.com/OpenSourceBrain/57910
- neuroscience-other-58172-58172-model :: opensourcebrain:58172 :: https://github.com/OpenSourceBrain/58172

## How to Run
```bash
python run_local.py --duration auto --tick-dt auto
```

## How to Interpret Outputs
Use output trajectories and summary metrics to compare mechanistic consistency across constituent models.
Interpret comparative spaces as non-causal side-by-side simulation views.
