# 2026-seasonal-soil-memory

Reproducible analysis code for “Seasonal Memory in Soils”: soil-moisture time series, SOM fraction chemistry (FT-ICR-MS), vegetation, and soil properties across contrasting hillslope storage.

## Associated manuscript
- **Title:** Seasonal Memory in Soils: Hydrologic History Drives Divergent Soil Organic Matter Trajectories Across Hillslopes  
- **Journal:** JGR Biogeosciences (in prep)  
- **Authors:** X. Takver et al.

## Data availability
- **Environmental Data Initiative (EDI):** DOI pending  
- **EMSL Science Central:** DOI pending  
- **Long-term data (EDI):** https://doi.org/10.6073/pasta/065e8bdaf36478d8e85ab0837d76bbe5  

**Note:** This repository contains analysis code. Data are archived at EDI and EMSL Science Central.

## Code archive (DOI)
- **Zenodo:** DOI pending  
- **Recommended citation:** cite the Zenodo **version DOI** corresponding to the release used for the paper.

## Repository organization
- `data/`
  - `<dataset>/raw/` – raw data inputs (not tracked in git; obtain from EDI and place in the appropriate data stream folder)
- `output/` (not tracked in git; created by the provided scripts)
  - `figures/` – generated figures, organized by data stream
  - `statistics/` – generated statistical tables, organized by data stream
- `scripts/` – analysis scripts organized by data stream
  - `functions/` – shared helper functions sourced by analysis scripts

## How to run
### Quick start
1. Clone the repo
2. Restore dependencies (see below)
3. Run the workflow scripts for the desired data stream in numeric order (01 → 03)

Example:
- `scripts/<data_stream>/01_processing.R`
- `scripts/<data_stream>/02_statistics.R`
- `scripts/<data_stream>/03_figure_X.R`

### Reproducibility
- **R:** tested with R 4.5.1  
- Package versions are pinned with `renv` (see `renv.lock`). Run:
  - `renv::restore()`

## Outputs
- Figures: `output/figures/`
- Statistical tables: `output/statistics/`

## Contact
Xander Takver  
xander.takver@oregonstate.edu  
GitHub: XTakver