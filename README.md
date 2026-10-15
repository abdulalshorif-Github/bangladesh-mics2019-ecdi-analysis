# Bangladesh MICS 2019: Child Development Analysis
R code examining associations between drinking-water contamination, nutritional status and early childhood development.
Author: Abdul Al Shorif
Status: Draft

**PROJECT OVERVIEW**
This project examines associations between drinking-water contamination, nutritional status and early childhood development using a prepared dataset from the Bangladesh Multiple Indicator Cluster Survey (MICS) 2019.
The project organizes existing R analysis code into separate scripts for overall Early Childhood Development Index (ECDI) outcomes, ECDI subdomains and exploratory mediation analyses.
The code has been reorganized for reproducibility and further development. 

# ANALYSES INCLUDED
1. Survey-weighted models of overall ECDI status.
2. Interaction and joint exposure analyses for E. coli and arsenic.
3. Survey-weighted models of ECDI subdomains.
4. Exploratory mediation analyses involving nutritional indicators.

# Requirements
R, RStudio and the prepared dataset, mics_ecdi_dataset_v4.xlsx.

# Run the analysis
1. Open mics2019-ecdi.Rproj in RStudio.
2. Place the dataset in data/private/.
3. Run source("setup_packages.R") to install dependencies.
4. Edit config.R to select analyses. For a first run, use analyses = c("overall").
5. Run source("run_analysis.R").

# Project structure
- R/: Analysis scripts.
- config.R: Data and analysis settings.
- outputs/: Generated results.
- docs/REVIEW_NOTES.md: Issues requiring review.
Each run saves results in a separate folder inside outputs/.
