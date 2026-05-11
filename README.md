# Reykjavik Rowhouse EnergyPlus Models

## Purpose

This repository contains EnergyPlus IDF models, scenario inputs, and supporting documentation for a master's thesis on heating energy use in Icelandic row houses.

## Research Scope

The thesis investigates heating energy use across **five representative Icelandic row-house building groups** (BG1–BG5). Each building group is modeled under **eight scenarios** (S0–S7) representing different occupancy, ventilation, and heating setpoint configurations:

- **S0:** Baseline
- **S1:** Low occupancy
- **S2:** High occupancy
- **S3:** Daytime presence
- **S4:** Low ventilation
- **S5:** High ventilation
- **S6:** Low setpoint
- **S7:** High setpoint

## Repository Contents

### `energyplus_models/`
EnergyPlus IDF files organized by building group and scenario. Each scenario folder contains the complete model definition for that configuration.

### `model_assumptions/`
CSV files documenting key input assumptions:
- `scenario_matrix.csv` — Parameter variations across scenarios
- `bg_geometry_envelope_summary.csv` — Geometry and envelope properties for each building group
- `internal_gains_schedules.csv` — Occupancy, lighting, and equipment schedules
- `ventilation_parameter_sets.csv` — Ventilation rate and control parameters
- `weather_and_simulation_settings.csv` — Weather file, simulation timestep, and configuration

### `post_processing_scripts/`
Python and/or analysis scripts organized by function:
- `smart_meter_analysis/` — Scripts for processing and analyzing smart meter data
- `energyplus_results/` — Scripts for extracting and processing EnergyPlus outputs
- `figures/` — Scripts generating visualization figures
- `tables/` — Scripts generating summary tables

### `summary_outputs/`
Processed and anonymized output files:
- `annual_results/` — Annual energy consumption and performance metrics
- `monthly_results/` — Monthly aggregated results
- `scenario_results/` — Scenario-level comparisons and sensitivity analyses
- `heat_balance_results/` — Heat balance component analysis

### `documentation/`
Project documentation:
- `software_versions.md` — EnergyPlus and other software versions used
- `data_availability_note.md` — Explanation of data exclusions and privacy restrictions
- `file_naming_conventions.md` — IDF file naming standards and directory structure

## Software Environment

**EnergyPlus version:** v25.2.0-cf7368216c

For a complete list of software versions and dependencies, see `documentation/software_versions.md`.

## Data Availability and Privacy

**Excluded from this repository:**
- Raw smart meter data
- Identifiable building-level data (addresses, household identifiers)
- Private survey responses

These data are excluded due to data access restrictions and privacy/GDPR requirements. The repository is designed to provide model files, input documentation, post-processing scripts, and processed/anonymized summary outputs where appropriate.

For information on accessing restricted data, see `documentation/data_availability_note.md`.

## Citation

If you reference this repository or use the models in your own research, please cite the associated master's thesis:

[Citation information to be added]

## File Organization

For naming conventions and file organization standards, see `documentation/file_naming_conventions.md`.