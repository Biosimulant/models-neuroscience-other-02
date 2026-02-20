# Space Plan - neuroscience-cortical-circuits-combo-0069

## Scientific Scope
- Domain: neuroscience
- Theme: cortical_circuits
- Base models: neuroscience-other-a-cortico-cerebello-thalamo-cortical-loop-model-257028-model, neuroscience-other-a-detailed-data-driven-network-model-of-prefront-189160-model, neuroscience-other-a-detailed-purkinje-cell-model-masoli-et-al-2015-229585-model, neuroscience-other-a-fast-rhythmic-bursting-cell-in-vivo-cell-model-125857-model

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
