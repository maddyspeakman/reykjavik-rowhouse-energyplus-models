# EnergyPlus Simulation Files for Residential Heating Energy Use Analysis in Reykjavík

## Purpose

This repository contains EnergyPlus Input Data Files (IDF) and construction assembly files used for building energy simulations developed as part of a master's thesis on residential heating energy use in Icelandic row houses.

The thesis investigates variation in heating energy use among selected representative row-house building groups in Reykjavík, with a focus on physical building characteristics, occupant behavior, and operational assumptions. These files are provided to support transparency and reproducibility of the simulation setup used in the thesis.

## Repository Contents

The repository contains two main folders:

```text
InputDataFiles/
construction_assemblies/
```

### InputDataFiles/

The `InputDataFiles/` folder contains the EnergyPlus IDF files used for the simulation scenarios. The files are organized by building group and scenario.

Each IDF file represents one building group and one simulation scenario. The repository includes five building groups and eight simulation scenarios per building group.

### construction_assemblies/

The `construction_assemblies/` folder contains the construction assembly files used to define the envelope construction sets for each building group.

The construction assembly files are named by building group:

```text
BG1_constructions
BG2_constructions
BG3_constructions
BG4_constructions
BG5_constructions
```

These files document the construction assemblies assigned to each building group, including envelope components such as walls, roofs, floors, windows, and doors where applicable. The construction assemblies should be interpreted together with the IDF files and the methodology described in the associated master's thesis.

## Building Groups

The models represent five representative Icelandic row-house building groups:

- **BG1**: Building Group 1
- **BG2**: Building Group 2
- **BG3**: Building Group 3
- **BG4**: Building Group 4
- **BG5**: Building Group 5

The building groups differ in geometry, construction period, envelope characteristics, and exposure conditions. Full descriptions of the building groups and modeling assumptions are provided in the associated master's thesis.

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

## IDF File Naming Convention

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

## Construction Assembly File Naming Convention

Construction assembly files follow the naming convention:

```text
BG{number}_constructions
```

Example file names:

```text
BG1_constructions
BG2_constructions
BG3_constructions
BG4_constructions
BG5_constructions
```

## Software Environment

The IDF files were prepared for use with:

```text
EnergyPlus v25.2.0-cf7368216c
```

Compatibility with other EnergyPlus versions has not been tested.

## Notes on Use

These files are intended as EnergyPlus model input files and supporting construction assembly documentation. Reproducing the simulation results reported in the associated thesis may require the same EnergyPlus version, weather file, simulation settings, and modeling assumptions described in the thesis.

The IDF files include the modeled building geometry, construction definitions, internal gains, schedules, heating setpoint assumptions, AirflowNetwork inputs, and scenario-specific occupant behavior assumptions used in the simulations. The construction assembly files provide additional documentation of the envelope construction sets used for each building group.

These files should be interpreted together with the thesis methodology, since not all assumptions can be fully documented within the IDF files or construction assembly files alone.

## Exclusions

This repository does not include:

- Raw smart-meter data
- Address-level or identifiable building information
- Survey responses or household-level occupant data
- Simulation output files
- Post-processing scripts
- Weather files
- Full written documentation of all modeling assumptions

For the complete methodology, assumptions, and interpretation of results, please refer to the associated master's thesis.

## License

This repository is licensed under the MIT License. See the `LICENSE` file for details.

## Citation

If you reference or use these simulation files, please cite the archived repository and the associated master's thesis.

Repository citation:

```text
Speakman, M. J. (2026). EnergyPlus simulation files for residential heating energy use analysis in Reykjavík (Version 1.0.0) [Computer software]. Zenodo. https://doi.org/[DOI to be added]
```

Associated thesis:

```text
Speakman, M. J. (2026). Explaining variation in residential heating energy use in Reykjavík row houses: Using smart meter data and building energy simulations to assess building characteristics, heat balance drivers, and occupant behavior impacts [Master's thesis, Reykjavík University]. Skemman. [URL to be added]
```
