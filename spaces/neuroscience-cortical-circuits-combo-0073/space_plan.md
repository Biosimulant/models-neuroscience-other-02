# Space Plan - neuroscience-cortical-circuits-combo-0073

## Scientific Scope
- Domain: neuroscience
- Theme: cortical_circuits
- Base models: neuroscience-other-a-sensorimotor-spinal-cord-model-hoshino-et-al-2-267395-model, neuroscience-other-a-set-of-reduced-models-of-layer-5-pyramidal-neu-146026-model, neuroscience-other-a-simple-model-of-neuromodulatory-state-dependen-222932-model, neuroscience-other-a-single-kinetic-model-for-all-human-voltage-gat-230137-model

## Wiring Plan
- Comparative mode with monitor-only routing.
- Each base model state-like output connects to monitor ports `state_a..state_d`.
- No direct causal links among base models unless explicitly upgraded later.

## Visualization Plan
- Include `StateComparisonMonitor` and `StateMetricsMonitor`.
- Require at least:
  - one timeseries visual,
  - one summary table visual.

## Validation Gates
- space schema validity
- wiring endpoint validity
- smoke run success
- repo manifest/entrypoint validators pass
