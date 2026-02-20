# Space Plan - neuroscience-hippocampal-circuits-combo-0080

## Scientific Scope
- Domain: neuroscience
- Theme: hippocampal_circuits
- Base models: neuroscience-other-a-neurocomputational-model-of-classical-conditio-138634-model, neuroscience-other-a-two-stage-model-of-dendritic-integration-in-ca-127351-model, neuroscience-other-acetylcholine-boosts-dendritic-nmda-spikes-ca3-pyramidal-neuron-osb267298-model, neuroscience-other-acetylcholine-boosts-dendritic-nmda-spikes-in-a-267298-model

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
