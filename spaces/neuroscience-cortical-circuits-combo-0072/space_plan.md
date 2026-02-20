# Space Plan - neuroscience-cortical-circuits-combo-0072

## Scientific Scope
- Domain: neuroscience
- Theme: cortical_circuits
- Base models: neuroscience-other-a-multilayer-cortical-model-to-study-seizure-pro-206238-model, neuroscience-other-a-neural-mass-computational-model-of-the-thalamo-138970-model, neuroscience-other-a-neural-mass-model-of-cross-frequency-coupling-227677-model, neuroscience-other-a-novel-mechanism-for-ramping-bursts-based-on-sl-2016216-model

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
