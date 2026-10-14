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
- Density and flow monitoring.
- Activation and updating of local guidance.
- Repeated simulation runs and output calculation.

The complete AnyLogic model is not currently provided. Repository contents and file-specific instructions will be updated as materials are uploaded.

## Reproducibility

The 1 s intervals specified above apply to the emotion and guidance procedures and should not be interpreted as a fixed numerical integration step for all pedestrian movement calculations.

The random seeds used in the reported experiments were not retained. Consequently, the individual simulation runs cannot be reproduced exactly from the documented settings alone. Future runs should record their seeds alongside scenario settings and outputs.

This repository is currently under preparation and does not yet provide a complete executable reproduction package.

## Scope

The simulations examine evacuation efficiency and local congestion under the modelled conditions. They use a static ship environment and assume effective guidance communication and passenger compliance.

The results do not establish safety or system reliability under evolving hazards, communication failures, or seafarer unavailability.

## Citation

If you use this work in your research, please cite the associated manuscript. Full bibliographic details and the DOI will be added when available.

## Questions and Feedback

Please open an Issue in this repository for questions about the implementation, parameter settings, or documentation.
