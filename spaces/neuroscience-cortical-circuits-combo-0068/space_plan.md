# Space Plan - neuroscience-cortical-circuits-combo-0068

## Scientific Scope
- Domain: neuroscience
- Theme: cortical_circuits
- Base models: neuroscience-other-87278-87278-model, neuroscience-other-97747-97747-model, neuroscience-other-a-biophysical-model-of-thalamocortical-network-s-2015422-model, neuroscience-other-a-cortical-sheet-mesoscopic-model-for-investigat-155565-model

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
