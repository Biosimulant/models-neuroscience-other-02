# COMBO_0073 - Neuroscience Cortical Circuits

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
- `neuroscience-other-a-sensorimotor-spinal-cord-model-hoshino-et-al-2-267395-model`: Neuroscience: ASensorimotorSpinalCordModelHoshinoEtAl2267395Model
- `neuroscience-other-a-set-of-reduced-models-of-layer-5-pyramidal-neu-146026-model`: Neuroscience: ASetOfReducedModelsOfLayer5PyramidalNeu146026Model
- `neuroscience-other-a-simple-model-of-neuromodulatory-state-dependen-222932-model`: Neuroscience: ASimpleModelOfNeuromodulatoryStateDependen222932Model
- `neuroscience-other-a-single-kinetic-model-for-all-human-voltage-gat-230137-model`: Neuroscience: ASingleKineticModelForAllHumanVoltageGat230137Model

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
- neuroscience-other-a-sensorimotor-spinal-cord-model-hoshino-et-al-2-267395-model :: modeldb:267395 :: https://modeldb.science/267395
- neuroscience-other-a-set-of-reduced-models-of-layer-5-pyramidal-neu-146026-model :: modeldb:146026 :: https://modeldb.science/146026
- neuroscience-other-a-simple-model-of-neuromodulatory-state-dependen-222932-model :: modeldb:222932 :: https://modeldb.science/222932
- neuroscience-other-a-single-kinetic-model-for-all-human-voltage-gat-230137-model :: modeldb:230137 :: https://modeldb.science/230137

## How to Run
```bash
python run_local.py --duration auto --tick-dt auto
```

## How to Interpret Outputs
Use output trajectories and summary metrics to compare mechanistic consistency across constituent models.
Interpret comparative spaces as non-causal side-by-side simulation views.
