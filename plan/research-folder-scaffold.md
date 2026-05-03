# Set Up a Research Project Folder Scaffold

Use this guide to create a standard folder scaffold for a research project.

The goal is to organize data, code, documentation, reports, and outputs in a clear structure that supports reproducible research, collaboration, and version control.

## Instructions

Create the folder structure below in the current project directory.

Do not delete or overwrite existing files.

If a folder already exists, keep it.

If a placeholder file already exists, leave it unchanged.

Create placeholder `.gitkeep` files in empty folders so Git can track the folder structure.

Create starter documentation files where specified.

## Folder Structure

``` text
project-name/
|-- data/
|   |-- raw/              # Original data; do not edit directly
|   |-- interim/          # Intermediate files created during cleaning
|   `-- processed/        # Cleaned or analysis-ready datasets
|-- code/
|   |-- notebooks/        # Exploratory analysis and prototyping
|   |-- scripts/          # Reusable scripts for cleaning and analysis
|   |-- src/              # Project functions or reusable code
|   `-- tests/            # Validation checks
|-- output/
|   |-- figures/          # Generated plots and charts
|   |-- tables/           # Generated tables and summaries
|   `-- models/           # Model outputs, if needed
|-- reports/
|   |-- drafts/           # Working versions of papers or reports
|   |-- final/            # Finalized reports
|   `-- presentations/    # Slides and presentation files
|-- docs/
|   |-- plan.md           # Project goals, milestones, and tasks
|   |-- context.md        # Background, assumptions, and scope
|   `-- references.md     # Key references and notes
|-- README.md             # Project overview and instructions
|-- .gitignore            # Files Git should ignore
`-- LICENSE               # Licensing terms, if applicable
```

## Files to Create

Create these folders:

``` text
data/raw
data/interim
data/processed
code/notebooks
code/scripts
code/src
code/tests
output/figures
output/tables
output/models
reports/drafts
reports/final
reports/presentations
docs
```

Create these files if they do not already exist:

``` text
README.md
.gitignore
docs/plan.md
docs/context.md
docs/references.md
```

Add `.gitkeep` files to empty folders so the folder scaffold is tracked by Git.

## Suggested README.md Content

``` markdown
# Project Name

Briefly describe the project here.

## Project Structure

- `data/raw/`: Original data. Do not edit directly.
- `data/interim/`: Intermediate data files created during cleaning.
- `data/processed/`: Cleaned or analysis-ready datasets.
- `code/notebooks/`: Exploratory analysis and prototyping.
- `code/scripts/`: Reusable scripts for data cleaning and analysis.
- `code/src/`: Project functions or reusable code.
- `code/tests/`: Validation checks.
- `output/figures/`: Generated plots and charts.
- `output/tables/`: Generated tables and summaries.
- `output/models/`: Model outputs, if needed.
- `reports/`: Drafts, final reports, and presentation files.
- `docs/`: Project planning, context, and references.

## Reproducibility Notes

Document how to reproduce the analysis here.
```

## Suggested .gitignore Content

``` gitignore
# Data that should not be committed
data/raw/
data/interim/

# Sensitive files
*.key
*.pem
.env
.Renviron

# Temporary files
.DS_Store
Thumbs.db
*.tmp
*.log

# R session and data files
.Rhistory
.RData
.Rproj.user/
*.rds
*.RDS
*.rda
*.RData

# Python cache and data files
__pycache__/
*.pyc
*.pkl
*.pickle
*.joblib
*.npy
*.npz
*.parquet
*.feather

# Stata data files
*.dta
*.gph
*.ster

# Large or compressed files
*.zip
*.tar
*.tar.gz
*.tgz
*.7z
*.rar
*.gz
*.bz2
*.xz

```

## Suggested docs/context.md Content

``` markdown
# Project Context

## Research Question

State the main research question.

## Motivation

Explain why the project matters.

## Data Sources

List data sources and access notes.

## Expected Outputs

Describe expected papers, reports, tables, figures, dashboards, or presentations.

## Folder Structure

Briefly explain any project-specific folder choices.

## Coding Standards

Describe preferred coding style, naming conventions, and package choices.

## Validation Checks

List checks that should be run during data cleaning and analysis.

## Rules for AI Assistance

- Do not invent data, citations, or results.
- Do not delete or overwrite files without explicit approval.
- Explain planned file changes before editing.
- Run available checks after making code changes.
- Keep researcher judgment central.
```

## Suggested docs/plan.md Content

``` markdown
# Project Plan

## Goals

- Define the main research goal.

## Tasks

- [ ] Collect data
- [ ] Clean data
- [ ] Construct variables
- [ ] Run descriptive analysis
- [ ] Run main models
- [ ] Create tables and figures
- [ ] Draft report or paper
- [ ] Review and revise

## Timeline

Add project milestones and deadlines.
```

## Suggested docs/references.md Content

``` markdown
# References

Add key papers, datasets, documentation links, and notes here.
```

## Completion Checklist

After creating the scaffold, report:

- Which folders were created.
- Which files were created.
- Which existing files were left unchanged.
- Whether `.gitignore` was created or already existed.
- Any issues or assumptions.
