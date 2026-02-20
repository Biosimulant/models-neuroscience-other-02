# Space Plan - neuroscience-cortical-circuits-combo-0070

## Scientific Scope
- Domain: neuroscience
- Theme: cortical_circuits
- Base models: neuroscience-other-a-full-scale-cortical-microcircuit-spiking-netwo-244261-model, neuroscience-other-a-gap-junction-network-of-amacrine-cells-control-262452-model, neuroscience-other-a-layer-v-ccs-type-pyramidal-cell-inhibitory-syn-183424-model, neuroscience-other-a-model-circuit-of-thalamocortical-convergence-b-150240-model

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
