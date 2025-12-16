# cpb-neuropeptide

This repository contains the analysis code and data used to evaluate neuropeptide
function in the Colorado potato beetle (*Leptinotarsa decemlineata*), with a focus on
GPA2 and GPCR LGR1. The analyses support feeding and injection
experiments assessing development, feeding behavior, and survival following
dsRNA-based knockdown experiments.

This repository is intended to accompany a peer-reviewed manuscript and provides
the complete, reproducible analysis workflow used in that study.

## Scientific scope

The analyses in this repository address the following experimental components:

- **Feeding assays**: larval growth, defoliation, developmental progression, and
  survival following oral dsRNA exposure
- **Injection assays**: developmental timing and survival following dsRNA injection
- **Developmental transition modeling**: life stage progression analyzed using
  survival and semi-Markov approaches

The repository focuses on phenotypic outcomes and statistical modeling rather than
molecular validation (e.g., qPCR), which are described separately in the manuscript.

## Repository structure

- `analysis/` contains fully reproducible R Markdown analysis scripts
- `data/inputs/` contains small, analysis-ready experimental datasets
- `data/derived/` contains curated or corrected datasets required for analysis
- `results/` is populated when analyses are run locally and is excluded from version control

## Relationship to the manuscript

- `analysis/feeding/feeding_analyses.Rmd` corresponds to feeding assay results and
  developmental transition analyses
- `analysis/injection/injection_analyses.Rmd` corresponds to injection assay survival
  and developmental analyses

All statistical models, transformations, and figures reported in the manuscript are
generated from the code in this repository.

## Data inclusion and exclusions

- All datasets required to reproduce the analyses are included in `data/inputs/`
  and `data/derived/`
- Large raw data files and generated outputs (e.g., intermediate CSVs, figures) are
  intentionally excluded and regenerated from source data and code
- No external file paths or proprietary data locations are required to run the analyses

## Reproducibility

Analyses use relative file paths via the `here` R package and can be run on any system
with R and the required packages installed.

To reproduce the analyses:

1. Clone or download this repository
2. Open the repository root in RStudio
3. Install required R packages as prompted
4. Knit the desired R Markdown file in `analysis/feeding/` or `analysis/injection/`

All outputs will be written to the appropriate subdirectory of `results/`.

## Citation

If you use or adapt this code, please cite the associated manuscript:

> Terris, E. et al. (YEAR). *Title*. Journal. DOI

A repository DOI may be added upon archival (e.g., Zenodo) following manuscript
acceptance.

## Repository status

This repository reflects the analysis code used for the manuscript:
- Status: **Manuscript preparation / submission**
- Updates following peer review will be versioned and documented

## Contact

For questions regarding analysis details or repository use, please contact the author at eterris@wisc.edu.

