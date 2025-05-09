# Gender Bias in Human Sentence Processing vs. Large Language Models

This repository contains a modular, multi-part portfolio project exploring how predictive biases in human language processing compare to those exhibited by large language models (LLMs).

The project is designed to demonstrate data science competencies across experimental design, statistical modeling, natural language processing, and reproducible reporting.

## Repository Structure

```
gender-bias-humans-vs-llms/
├── data/          # Raw and processed datasets (anonymized)
├── models/        # Fitted brms model objects (gitignored)
├── notebooks/     # Preprocessing and modeling scripts (.qmd)
├── reports/       # Quarto reports for each project part
├── shiny-app/     # Shiny dashboard for Part 1 (human data)
├── streamlit-app/ # Streamlit dashboard for Part 2 (LLMs)
├── docs/          # GitHub Pages output (rendered HTML reports)
├── index.qmd      # Project landing page (rendered to docs/index.html)
├── .gitignore
└── README.md      # You are here
```


## Project Overview

This project builds on a psycholinguistic research study involving 2,196 participants and multiple experimental designs. It investigates how people interpret gendered pronouns in political contexts—and compares these human behavioral patterns to those learned by LLMs.

The idea behind this portfolio project is to build a bridge between my past academic research in psycholinguistics on one side, and the kind of data science work I want to do going forward on the other side. 

### Project Parts

| Part | Focus | Tools & Skills |
|------|-------|----------------|
| **Part 1** | Analysis of human behavioral data | R, `brms`, `tidyverse`, Shiny |
| **Part 2** | LLM surprisal analysis on same stimuli | Python, HuggingFace, Streamlit |
| **Part 3** | Low-shot fine-tuning of LLMs | Python, PEFT/fine-tuning pipelines |

For a full narrative overview and interactive reports, visit the [project site](https://tpoppels.github.io/gender-bias-humans-vs-llms/).

## Reproducibility Notes

- **Raw data** are excluded from the repo due to privacy considerations.
- **Cleaned, anonymized data** are available in `/data/processed/`.
- **Large model files** (`.rds`) are stored in `/models/` and are gitignored.
- All reports are generated with [Quarto](https://quarto.org/), rendered to `/docs`, and made available via Github Pages.

### Reproducing the R environment with verified package versions etc.

To restore the R environment:

```r
install.packages("renv")
renv::restore()
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
