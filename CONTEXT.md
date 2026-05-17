# repo-template — Context Document

## What it is
A general-purpose repository template for data engineering, data science, and machine learning projects. Clone or use as a GitHub template to start new projects with a clean, consistent structure.

## Who it's for
Anyone starting a new DE/DS/ML project who wants a battle-tested folder structure without building it from scratch.

## Structure
```
project/
├── data/
│   ├── 0-raw        ← Original, immutable source data
│   ├── 1-bronze     ← Ingested, schema-enforced
│   ├── 2-silver     ← Cleansed, deduplicated, merged
│   ├── 3-gold       ← Aggregated, analytics-ready
│   ├── 4-features   ← ML feature sets
│   └── 5-processed  ← Final data for modeling or analysis
├── docs/            ← Project documentation
├── models/          ← Trained models and predictions
├── notebooks/       ← Jupyter notebooks for exploration
├── references/      ← Data dictionaries and reference materials
├── reports/figures/ ← Generated graphics and figures
├── src/             ← Source code
├── CONTEXT.md       ← This file
├── environment.yml  ← Conda environment definition
├── README.md        ← Project README
└── requirements.txt ← Python dependencies
```

## How to use
1. Click **Use this template** on GitHub to create a new repo
2. Clone locally
3. Update `README.md` with project details
4. Update `CONTEXT.md` with architectural decisions
5. Add dependencies to `requirements.txt` and `environment.yml`
6. Delete folders that don't apply to your project type
7. Start building

## Standards
- Keep `data/0-raw/` immutable — never modify original source data
- Document architectural decisions in `CONTEXT.md` as they are made
- Name notebooks with a number prefix: `01-exploration.ipynb`
- No credentials, API keys, or secrets in the repo
- All source code lives in `src/` — notebooks are for exploration only

## Part of
TDBI platform — Think, Debate, Build, Iterate
