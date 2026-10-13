# Postoperative Patient Data: Biostatistical Analysis

## Project Overview

This project aims to explore postoperative patient data using Python and statistical methods. The main objectives are to assess data quality, describe patient characteristics, visualize physiological variables, and investigate associations between physiological stability and the patient's destination after recovery.

The project is being developed as a practical portfolio in applied biostatistics, with an emphasis on reproducible analysis, data cleaning, statistical reasoning, and clear communication of results.

**Project status:** In progress.

## Research Question

Which physiological characteristics observed during postoperative recovery are associated with the patient's destination after leaving the recovery area?

## Dataset

The project uses the *Post-Operative Patient Data* dataset, originally documented in 1993.

- **Number of observations:** 90
- **Number of variables:** 9
- **Missing values:** 3, all in the `COMFORT` variable
- **Outcome variable:** `ADM-DECS`

The outcome variable describes three possible destinations:

- `A`: General hospital floor (64 observations)
- `S`: Prepared to go home (24 observations)
- `I`: Intensive Care Unit (2 observations)

The explanatory variables describe internal and surface temperature, oxygen saturation, blood pressure, physiological stability, and perceived comfort.

**Data source:** [UCI Machine Learning Repository — Post-Operative Patient Data](https://archive.ics.uci.edu/)

The original dataset documentation is provided in `data/post-operative.names`.

## Objectives

1. Inspect the structure and quality of the dataset.
2. Identify and document missing values and potential data inconsistencies.
3. Describe the distributions of categorical and numerical variables.
4. Create visualizations to summarize the data.
5. Explore associations between physiological variables and patient destination.
6. Interpret findings while acknowledging statistical and clinical limitations.

## Methods and Tools

The planned analysis will use:

- **Python** for data analysis.
- **pandas** for data manipulation and quality checks.
- **Matplotlib** and **Seaborn** for visualization.
- **SciPy** for statistical testing where appropriate.
- **Jupyter Notebook** for reproducible analysis and documentation.
- **Git and GitHub** for version control and project sharing.

Statistical tests will be selected according to the data structure and their assumptions. The very small Intensive Care Unit group (n = 2) limits reliable comparisons involving that category.

## Repository Structure

```text
projet_biostatistique/
├── data/
│   ├── post-operative.data
│   └── post-operative.names
├── notebooks/
│   └── 01_analyse_postoperatoire.ipynb
├── README.md
└── requirements.txt
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/postoperative-biostatistics-analysis.git
cd postoperative-biostatistics-analysis
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Create a Python environment

```bash
python -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Launch JupyterLab

```bash
python -m jupyter lab
```

Open `notebooks/01_analyse_postoperatoire.ipynb` to explore the analysis.

## Limitations

This is a small, historical dataset intended for educational and exploratory analysis. Its sample size, class imbalance, and age limit its applicability to contemporary clinical practice.

The analysis is not intended to establish causality, provide clinical recommendations, or validate a clinical prediction model.

## Author

Bioinformatics undergraduate student interested in biostatistics, clinical data analysis, and reproducible research.

## Acknowledgements

The dataset was originally developed for research on postoperative patient assessment and decision support. Please consult the original dataset documentation and applicable terms before redistributing the data.
