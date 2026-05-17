# EnergyPlus IDF Files for Residential Heating Energy Use Analysis in Reykjavík

## Purpose

This repository contains EnergyPlus Input Data Files (IDF) used for building energy simulations developed as part of a master's thesis on residential heating energy use in Icelandic row houses.

The thesis investigates variation in heating energy use among selected representative row-house building groups in Reykjavík, with a focus on physical building characteristics, occupant behavior, and operational assumptions.

Thesis link: [Skemman link to be added]

## Repository Contents

The EnergyPlus input files are organized in the `InputDataFiles/` directory by building group and simulation scenario.

## Building Groups

The models represent five representative row-house building groups:

- **BG1**: Building Group 1
- **BG2**: Building Group 2
- **BG3**: Building Group 3
- **BG4**: Building Group 4
- **BG5**: Building Group 5

## Simulation Scenarios

Each building group includes eight simulation scenarios:

- **S0: Baseline**: Reference scenario with baseline assumptions
- **S1: Low occupancy**: Reduced number of occupants
- **S2: High occupancy**: Increased number of occupants
- **S3: Daytime presence**: Modified occupancy schedule with weekday daytime presence
- **S4: Low ventilation**: Reduced manual ventilation assumptions
- **S5: High ventilation**: Increased manual ventilation assumptions
- **S6: Low setpoint**: Lower indoor heating setpoint
- **S7: High setpoint**: Higher indoor heating setpoint

## File Naming Convention

IDF files follow the naming convention:

```text
BG{number}_S{scenario_number}_{scenario_name}.idf
```

Example file names:

```text
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

The files were prepared for use with:

```text
EnergyPlus v25.2.0-cf7368216c
```

Compatibility with other EnergyPlus versions has not been tested.

## Notes on Use

These files are provided to support transparency and reproducibility of the simulation setup used in the associated thesis. They are intended as EnergyPlus model input files and may require the same EnergyPlus version, weather file, and supporting assumptions described in the thesis to reproduce the reported simulation results.

## Exclusions

This repository contains only EnergyPlus IDF model files. The following materials are not included:

- Raw smart-meter data
- Address-level or identifiable building information
- Survey responses or household-level occupant data
- Simulation output files
- Post-processing scripts
- Full documentation of all modeling assumptions

For the complete methodology, assumptions, and interpretation of results, please refer to the associated master's thesis.

## Citation

If you reference or use these IDF files, please cite the archived repository and the associated master's thesis.

Repository citation:

```text
Speakman, M. J. (2026). EnergyPlus IDF files for residential heating energy use analysis in Reykjavík (Version 1.0.0) [Computer software]. Zenodo. https://doi.org/[DOI to be added]
```

Associated thesis:

```text
Speakman, M. J. (2026). [Thesis title to be added] [Master's thesis, Reykjavík University]. Skemman. [URL to be added]
```

## License

License information to be added.
