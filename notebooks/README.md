# Analysis Notebooks

This directory will contain the Quarto notebooks used for data cleaning and model fitting.

## Notebooks

1. `01_data-cleaning.qmd`
   - Data preprocessing and anonymization
   - Quality checks and data validation
   - Outputs cleaned data to `data/processed/`

2. `02_model-fitting.qmd`
   - Statistical model specification using brms
   - Model diagnostics and validation
   - Generates model outputs for reports

## Required R Packages

```r
install.packages(c(
  "tidyverse",    # Data manipulation and visualization
  "brms",         # Bayesian modeling
  "quarto",       # Notebook rendering
  "here",         # Project-relative paths
  "janitor",      # Data cleaning
  "skimr",        # Data summaries
  "patchwork",    # Plot arrangement
  "bayesplot",    # MCMC diagnostics
  "tidybayes"     # Bayesian model visualization
))
```

## Running the Notebooks

1. Ensure all required packages are installed
2. Run notebooks in sequence (01 → 02)
3. Check the output in `data/processed/` after running 01
4. Model outputs will be saved for use in reports 