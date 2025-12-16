# cpb-neuropeptide

This repository contains analysis code and data for RNAi knockdown phenotypic assay results
in the Colorado potato beetle (*Leptinotarsa decemlineata*). The project focuses on
feeding and injection experiments targeting neuropeptide GPA2 / GPCR LGR1 pathways and associated
developmental, feeding, and survival phenotypes.

## Repository structure

- `analysis/` contains R Markdown files for each experiment type
- `data/inputs/` contains input datasets
- `data/derived/` contains externally curated or intermediate datasets
- `results/` is where figures and tables are written when analyses are run

## Data availability

All input datasets required to run the analyses are included in this repository
under `data/inputs/` and `data/derived/`.

Generated outputs (intermediate CSVs) are written to the `results/`
directory and are not tracked in GitHub.

## How to run the analyses

1. Clone or download this repository
2. Open the repository in RStudio
3. Install required R packages as needed
4. Open either:
   - `analysis/feeding/feeding_analyses.Rmd`, or
   - `analysis/injection/injection_analyses.Rmd`
5. Knit the R Markdown file or run chunks interactively

All file paths are relative and use the `here` package, so the analyses should run
without modification on any system.

## Outputs

Running the analyses will generate:
- cleaned and transformed datasets
- summary tables
- figures
- model-ready datasets

These outputs are written to subdirectories of `results/`.

## Notes

This repository is intended to support reproducible analysis and manuscript
preparation. Derived outputs are regenerated from source data and code rather than
stored in version control.

## Contact

For questions about this repository, please contact:

Emma Terris, eterris@wisc.edu  
University of Wisconsin–Madison
