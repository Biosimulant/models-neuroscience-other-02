# COMBO_0072 - Neuroscience Cortical Circuits

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
- `neuroscience-other-a-multilayer-cortical-model-to-study-seizure-pro-206238-model`: Neuroscience: AMultilayerCorticalModelToStudySeizurePro206238Model
- `neuroscience-other-a-neural-mass-computational-model-of-the-thalamo-138970-model`: Neuroscience: ANeuralMassComputationalModelOfTheThalamo138970Model
- `neuroscience-other-a-neural-mass-model-of-cross-frequency-coupling-227677-model`: Neuroscience: ANeuralMassModelOfCrossFrequencyCoupling227677Model
- `neuroscience-other-a-novel-mechanism-for-ramping-bursts-based-on-sl-2016216-model`: Neuroscience: ANovelMechanismForRampingBurstsBasedOnSl2016216Model

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
- neuroscience-other-a-multilayer-cortical-model-to-study-seizure-pro-206238-model :: modeldb:206238 :: https://modeldb.science/206238
- neuroscience-other-a-neural-mass-computational-model-of-the-thalamo-138970-model :: modeldb:138970 :: https://modeldb.science/138970
- neuroscience-other-a-neural-mass-model-of-cross-frequency-coupling-227677-model :: modeldb:227677 :: https://modeldb.science/227677
- neuroscience-other-a-novel-mechanism-for-ramping-bursts-based-on-sl-2016216-model :: modeldb:2016216 :: https://modeldb.science/2016216

## How to Run
```bash
python run_local.py --duration auto --tick-dt auto
```

## How to Interpret Outputs
Use output trajectories and summary metrics to compare mechanistic consistency across constituent models.
Interpret comparative spaces as non-causal side-by-side simulation views.
