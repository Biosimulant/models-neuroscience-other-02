# Space Plan - neuroscience-cortical-circuits-combo-0071

## Scientific Scope
- Domain: neuroscience
- Theme: cortical_circuits
- Base models: neuroscience-other-a-model-for-focal-seizure-onset-propagation-evol-266524-model, neuroscience-other-a-model-for-recurrent-spreading-depolarizations-235377-model, neuroscience-other-a-model-of-antennal-lobe-of-bee-chen-jy-et-al-20-226471-model, neuroscience-other-a-model-of-slow-motor-unit-kim-2017-235769-model

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
