# COMBO_0069 - Neuroscience Cortical Circuits

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
- `neuroscience-other-a-cortico-cerebello-thalamo-cortical-loop-model-257028-model`: Neuroscience: ACorticoCerebelloThalamoCorticalLoopModel257028Model
- `neuroscience-other-a-detailed-data-driven-network-model-of-prefront-189160-model`: Neuroscience: ADetailedDataDrivenNetworkModelOfPrefront189160Model
- `neuroscience-other-a-detailed-purkinje-cell-model-masoli-et-al-2015-229585-model`: Neuroscience: ADetailedPurkinjeCellModelMasoliEtAl2015229585Model
- `neuroscience-other-a-fast-rhythmic-bursting-cell-in-vivo-cell-model-125857-model`: Neuroscience: AFastRhythmicBurstingCellInVivoCellModel125857Model

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
- neuroscience-other-a-cortico-cerebello-thalamo-cortical-loop-model-257028-model :: modeldb:257028 :: https://modeldb.science/257028
- neuroscience-other-a-detailed-data-driven-network-model-of-prefront-189160-model :: modeldb:189160 :: https://modeldb.science/189160
- neuroscience-other-a-detailed-purkinje-cell-model-masoli-et-al-2015-229585-model :: modeldb:229585 :: https://modeldb.science/229585
- neuroscience-other-a-fast-rhythmic-bursting-cell-in-vivo-cell-model-125857-model :: modeldb:125857 :: https://modeldb.science/125857

## How to Run
```bash
python run_local.py --duration auto --tick-dt auto
```

## How to Interpret Outputs
Use output trajectories and summary metrics to compare mechanistic consistency across constituent models.
Interpret comparative spaces as non-causal side-by-side simulation views.
