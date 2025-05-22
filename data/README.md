# Data Directory

This directory will contain both raw and processed data for the gender bias analysis project.

## Directory Structure

- `raw/`: Contains original, non-anonymized data
  - This directory is gitignored to protect participant privacy
  - Place original data files here before running the cleaning pipeline
- `processed/`: Contains cleaned, anonymized data
  - These files are used in the analysis notebooks and reports
  - All personally identifiable information has been removed

## Data Pipeline

1. Raw data is collected and placed in `raw/`
2. The cleaning pipeline in `notebooks/01_data-cleaning.qmd` processes the data
3. Processed data is saved to `processed/` for use in analysis

## Data Formats

- Raw data for Part 1 consists of Ibex results file (.txt format); see https://github.com/addrummond/ibex/blob/master/docs/manual.md#basic-concepts.
- Cleaned data is stored in .rds format