# Space Plan - neuroscience-hippocampal-circuits-combo-0079

## Scientific Scope
- Domain: neuroscience
- Theme: hippocampal_circuits
- Base models: neuroscience-other-a-general-model-of-hippocampal-and-dorsal-striat-266836-model, neuroscience-other-a-model-for-how-correlation-depends-on-the-neuro-153452-model, neuroscience-other-a-model-of-unitary-responses-from-a-c-and-pp-syn-137259-model, neuroscience-other-a-model-of-ventral-hippocampal-ca1-pyramidal-neu-267066-model

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
