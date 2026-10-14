# AdvMarTech-Eva_Guidance_ABM
Simulation code, parameter settings, and documentation for an emotion-coupled agent-based model of human evacuation from passenger ship with seafarer guidance.
# Seafarer-Guided Evacuation from Passenger Ships

Supporting materials for the manuscript:

**“Seafarer guided crowd evacuation from passenger ships: An emotion-coupled agent-based model.”**

This repository is being prepared to share selected implementation code, parameter settings, and documentation for the evacuation model presented in the manuscript.

## Methodology

The study develops an agent-based framework for examining how seafarer guidance influences passenger evacuation through emotional regulation and congestion-responsive route guidance.

The framework comprises three components:

1. **Seafarer deployment:** Placement of seafarers near assembly-station entrances and critical corridor and stairway junctions.
2. **Emotion regulation:** Representation of passenger heterogeneity using OCEAN personality traits and an adapted SEIRS emotional-contagion model.
3. **Local route guidance:** Density- and flow-triggered directional guidance that adjusts passenger approaches while preserving assigned assembly stations.

The model uses the SGVDS1 passenger-ship scenario as its reference environment. Simulation outputs include evacuation times, emotional-state evolution, and passenger density patterns.

## Simulation Settings

| Item | Setting |
|---|---|
| Simulation platform | AnyLogic 8.9.8 |
| Implementation | Agent-based modelling with the Pedestrian Library and Java-based model logic |
| Execution | Event-driven simulation with periodic emotion and guidance updates |
| Emotional update interval | 1 s |
| Guidance update interval | 1 s |
| Passenger populations | 400–900 passengers |
| Monte Carlo replications | 50 runs per scenario |
| Random-number generation | AnyLogic default pseudorandom-number generator with the “Random seed” option selected |
| Initial passenger allocation | Allocation among functional areas according to SGVDS1 population proportions, with random positions within each area |
| Assembly-station assignments | Fixed throughout each simulation |

All experiments reported in the revised manuscript were rerun using AnyLogic 8.9.8.

## AnyLogic Java Code and Documentation

The planned release includes selected Java code from the AnyLogic implementation, parameter and input descriptions, and instructions covering:

- Passenger initialisation and attribute assignment.
- Emotional-intensity and desired-speed updates.
- Activation and updating of local guidance.
- Repeated simulation runs and output calculation.

The complete AnyLogic model is not currently provided. Repository contents and file-specific instructions will be updated as materials are uploaded.

## Reproducibility

The 1 s intervals specified above apply to the emotion and guidance procedures and should not be interpreted as a fixed numerical integration step for all pedestrian movement calculations.

This repository is currently under preparation and does not yet provide a complete executable reproduction package.


## Citation

If you use this work in your research, please cite the associated manuscript. Full bibliographic details and the DOI will be added when available.

## Questions and Feedback

Please open an Issue in this repository for questions about the implementation, parameter settings, or documentation.

## Model Implementation Screenshots

The following screenshots show selected parts of the model
implementation in AnyLogic, including the main modelling workspace,
agent statecharts, and evacuation process logic.

### Main Model Workspace

![Main model workspace](<img width="1596" height="799" alt="cfdb86a6-181c-4915-8e17-d7f8f610930c" src="https://github.com/user-attachments/assets/fca18e8b-9016-4b3d-84de-1063def20b79" />
)


### Passenger Agent and Statechart

![Passenger agent and statechart](<img width="849" height="635" alt="4b2c65f1-6ac5-49a5-812b-635d052065af" src="https://github.com/user-attachments/assets/073e8a4d-fff9-4652-98df-ec3c9c3d4bb2" />
)

### Evacuation Process Logic

![Evacuation process flowchart](<img width="771" height="1126" alt="643f275f-608f-4dc9-9392-77566d6c98e7" src="https://github.com/user-attachments/assets/5c179822-074b-4b1e-bf8b-72791b35e9a4" />
)
