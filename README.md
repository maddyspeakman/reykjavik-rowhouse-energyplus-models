# EnergyPlus Simulation Files for Residential Heating Energy Use Analysis in Reykjavík

## Purpose

This repository contains EnergyPlus Input Data (IDF) files used in simulations for a master's thesis investigating heating energy use in representative Icelandic row houses. The IDF files are provided here because their length makes them impractical to include directly in thesis appendices.

## Repository Contents

All EnergyPlus IDF files are organized in the `InputDataFiles/` directory by building group and scenario.

### Building Groups

The models represent **five representative Icelandic row-house building groups:**

- **BG1** – Building Group 1
- **BG2** – Building Group 2
- **BG3** – Building Group 3
- **BG4** – Building Group 4
- **BG5** – Building Group 5

### Scenarios

Each building group includes **eight scenarios** representing different occupant behavior and building operational parameters:

- **S0: Baseline** – Reference scenario with standard assumptions
- **S1: Low occupancy** – Reduced occupancy levels
- **S2: High occupancy** – Increased occupancy levels
- **S3: Daytime presence** – Modified occupancy patterns with daytime presence
- **S4: Low ventilation** – Reduced ventilation rates
- **S5: High ventilation** – Increased ventilation rates
- **S6: Low setpoint** – Lower indoor temperature setpoint
- **S7: High setpoint** – Higher indoor temperature setpoint

## File Naming Convention

EnergyPlus IDF files follow the naming convention:

```
BG{number}_S{scenario_number}_{scenario_name}.idf
```

### Examples

```
BG1_S0_baseline.idf
BG1_S1_low_occupancy.idf
BG1_S2_high_occupancy.idf
BG1_S3_daytime_presence.idf
BG1_S4_low_ventilation.idf
BG1_S5_high_ventilation.idf
BG1_S6_low_setpoint.idf
BG1_S7_high_setpoint.idf
```

## Software Environment

**EnergyPlus version:** v25.2.0-cf7368216c

## Exclusions

This repository contains **only** EnergyPlus IDF model files. The following are **not** included:

- Raw smart meter data
- Identifiable building-level information (addresses, household identifiers)
- Survey responses and occupant behavior data
- Simulation output files and results
- Post-processing scripts and analysis code
- Model input assumptions documentation

For information on the complete thesis project, including post-processing scripts, results analysis, and detailed model assumptions, please refer to the primary thesis documentation.

## Citation

If you reference these IDF files or use them in your own research, please cite the associated master's thesis:

[Citation information to be added]

## License

[License information to be added]
