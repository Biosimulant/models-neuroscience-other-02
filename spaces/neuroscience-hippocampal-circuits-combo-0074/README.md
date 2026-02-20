# COMBO_0074 - Neuroscience Hippocampal Circuits

## Scientific Question
How do recurrent hippocampal motifs shape network dynamics over time?

## Biological Context
Neuronal dynamics, network signaling, and emergent circuit behavior.

## Mechanistic Assumptions
- Model implementations are used as published in their curated manifests without biological reinterpretation.
- Time integration uses a shared global tick compatible with model min_dt constraints.
- Comparative (non-causal) mode is used because full deterministic IO coverage for causal coupling was not satisfied.

## Why These Models Belong Together
The combination was selected from a shared domain/theme bucket with deterministic compatibility checks.
- `neuroscience-other-51196-51196-model`: Neuroscience: Model5119651196Model
- `neuroscience-other-51781-51781-model`: Neuroscience: Model5178151781Model
- `neuroscience-other-55035-55035-model`: Neuroscience: Model5503555035Model
- `neuroscience-other-64167-64167-model`: Neuroscience: Model6416764167Model

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
- neuroscience-other-51196-51196-model :: opensourcebrain:51196 :: https://github.com/OpenSourceBrain/51196
- neuroscience-other-51781-51781-model :: opensourcebrain:51781 :: https://github.com/OpenSourceBrain/51781
- neuroscience-other-55035-55035-model :: opensourcebrain:55035 :: https://github.com/OpenSourceBrain/55035
- neuroscience-other-64167-64167-model :: opensourcebrain:64167 :: https://github.com/OpenSourceBrain/64167

## How to Run
```bash
python run_local.py --duration auto --tick-dt auto
```

## How to Interpret Outputs
Use output trajectories and summary metrics to compare mechanistic consistency across constituent models.
Interpret comparative spaces as non-causal side-by-side simulation views.
