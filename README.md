# carbon-credit-4-adapt
Analysis repository for assessing technical potential and net economic benefit (NEB) of adaptation-linked carbon crediting in agriculture. Includes spatial workflows, country-level modelling (Kenya, Ethiopia, Nigeria), and reproducible outputs for evidence-based decision-making.

## Purpose

The analysis supports the development of country-specific evidence on where agricultural practices may generate:

- mitigation benefits
- productivity benefits
- adaptation benefits
- positive net economic benefit
- plausible opportunities for scaling

The initial country focus is:

- Ethiopia
- Kenya
- Nigeria

The analytical framework is designed to support country profiling and related spatial outputs, including maps, tables, and summary datasets.

## Scope of this repository

This repository is used to:

- prepare and harmonize spatial input layers
- generate technical potential surfaces
- estimate NEB inputs and outputs
- run sensitivity and uncertainty analyses
- produce intermediate and final analytical outputs
- document methods, assumptions, and data dependencies

This repository does **not** contain:

- project management materials
- meeting administration
- donor reporting files
- communications assets
- production deployment code for a tool or web platform

If a deployable tool is developed, that should be maintained in a separate repository.

## Analytical components

The analysis is expected to cover five broad components:

1. **Setup and harmonization**
   - common grid
   - practice-by-data matrix
   - baseline layers
   - country-level analytical specifications

2. **Technical potential**
   - mitigation surfaces
   - productivity benefit estimation
   - adaptation benefit estimation
   - spatial integration and opportunity zoning
   - uncertainty analysis

3. **Net Economic Benefit (NEB)**
   - framework definition
   - cost estimation
   - adoption assumptions
   - spatial NEB calculation
   - sensitivity analysis

4. **Scaling and interpretation**
   - alignment with feasibility and scaling considerations
   - scenario exploration
   - country-level synthesis

5. **Outputs**
   - maps
   - summary tables
   - country-level analytical datasets
   - documented assumptions and metadata

## Repository structure

├── README.md
├── data/
│   ├── raw/
│   ├── interim/
│   ├── processed/
│   └── metadata/
├── scripts/
│   ├── 01_setup/
│   ├── 02_technical_potential/
│   ├── 03_neb/
│   ├── 04_scaling/
│   ├── 05_outputs/
│   └── utils/
├── config/
│   ├── countries/
│   ├── practices/
│   ├── scenarios/
│   └── paths/
├── outputs/
│   ├── figures/
│   ├── tables/
│   ├── rasters/
│   └── summaries/
├── docs/
│   ├── methods/
│   ├── data_sources/
│   └── schemas/
└── tests/

## Working principles

- Reproducibility first: all core outputs must be generated from code and configuration  
- No large raw data in the repository  
- Modular workflows across technical potential, NEB, and outputs  
- Centralised configuration (avoid hard-coded parameters and paths)  
- All key assumptions must be documented  

---

## Data handling

- Large spatial and raw datasets are not stored in this repository  
- External storage should be used for heavy data assets  
- This repository maintains:
  - metadata  
  - data inventories  
  - access instructions  
  - processing scripts  
- All data sources must be documented in `docs/data_sources/`  

---

## Branching model

- `main` – stable, reviewed code  
- Feature branches for development (e.g. `feature/neb`, `feature/ethiopia`)  
- Pull requests required before merging into `main`  
- Keep branches short-lived and focused  

---

## Environment

- The computational environment must be defined using one approach:
  - `renv.lock` (R)  
  - `environment.yml` (conda)  
  - `requirements.txt` (Python)  
- All contributors should use the same environment specification  

---

## Outputs

Typical outputs include:

- Spatial layers (e.g. mitigation, adaptation, NEB)  
- Maps and visualisations  
- Summary tables  
- Country-level datasets  
- Intermediate analytical products  

All outputs should have:
- Clear structure  
- Consistent naming  
- Version or date reference  

---

## Status and ownership

- This repository is under active development  
- Methods and structure may evolve during early phases  
- Maintainers:  
  - Pete Steward
  - Ani Ghosh
  - Chun Song