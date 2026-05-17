# Project Template

A general-purpose project template for data engineering, data science, and 
machine learning projects. Clone this repo to start a new project with a 
clean, consistent structure.

## How to Use

1. Click **Use this template** in GitHub to create a new repo from this template
2. Clone your new repo locally
3. Update `README.md` with your project details
4. Update `CONTEXT.md` with internal context and architectural decisions
5. Add your dependencies to `requirements.txt` and `environment.yml`
6. Delete folders that don't apply to your project type
7. Start building

## Repository Structure

```
project/
├── data
│   ├── 0-raw              <- Original, immutable source data
│   ├── 1-bronze           <- Ingested, schema-enforced
│   ├── 2-silver           <- Cleansed, deduplicated, merged
│   ├── 3-gold             <- Aggregated, analytics-ready
│   ├── 4-features         <- ML feature sets
│   └── 5-processed        <- Final data for modeling or analysis
├── docs/               # Project documentation
├── models/             # Trained models and predictions
├── notebooks/          # Jupyter notebooks for exploration and development
├── references/         # Data dictionaries, manuals, and reference materials
├── reports/
│   └── figures/        # Generated graphics and figures
├── src/                # Source code
├── .gitignore
├── CONTEXT.md          # Internal project context and architectural decisions
├── environment.yml     # Conda environment definition
├── README.md           # This file
└── requirements.txt    # Python dependencies
```

## Template Notes

This template uses a merged DE/DS structure suitable for single-team or 
early-stage projects. For larger projects with separate engineering and data 
science teams, consider splitting into dedicated DE and DS repositories with 
the Gold layer as the handoff point.

## Standards

- Keep `data/raw/` immutable — never modify original source data
- Document architectural decisions in `CONTEXT.md` as they are made
- Name notebooks with a number prefix for ordering: `01-exploration.ipynb`
- No credentials, API keys, or secrets in the repo — use environment variables
- All source code lives in `src/`, notebooks are for exploration only
- Delete data folders that don't apply to your project type