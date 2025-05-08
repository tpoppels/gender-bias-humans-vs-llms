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
   - Generates model outputs for reports, which will be parked in `models/`

## Required R Packages

```r
install.packages(c(
  "tidyverse",    # Data manipulation and visualization
  "brms",         # Bayesian modeling
))
```

## Running the Notebooks

1. Ensure all required packages are installed
2. Make sure gitignored raw data is present, or skip `data-cleaning.qmd`
3. Run notebooks in sequence