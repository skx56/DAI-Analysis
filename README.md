# Restaurant Tip Prediction and Regression Analysis

<p align="center">
<img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge" />
  <img alt="Jupyter" src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge" />
  <img alt="Pandas" src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge" />
  <img alt="scikit-learn" src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge" />
  <img alt="Data Science" src="https://img.shields.io/badge/Data%20Science-1F77B4?style=for-the-badge" />
</p>

<p align="center">
  <strong>A regression-analysis workflow for modeling restaurant tip behavior from dining attributes and statistical diagnostics.</strong>
</p>

This project explores the relationship between dining context, customer behavior, and tip amount through a notebook-based machine learning workflow. It emphasizes data understanding, model selection, diagnostics, and interpretation.

## Core Capabilities

- Loads and analyzes restaurant tipping data in a reproducible notebook.
- Builds regression models for tip prediction.
- Evaluates model behavior through statistical and visual diagnostics.
- Documents insights around feature impact and prediction quality.

## Technical Architecture

The project is organized as a Jupyter notebook analysis with a README summary. The notebook contains the complete workflow from exploration through modeling and evaluation.

## Architecture Diagram

```mermaid
%%{init: {"flowchart": {"nodeSpacing": 55, "rankSpacing": 70, "curve": "basis"}, "themeVariables": {"fontSize": "16px", "fontFamily": "Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif"}}}%%
flowchart TD
  Data["Restaurant Tip Dataset"] --> Notebook["Jupyter Analysis Notebook"]
  Notebook --> EDA["Exploratory Analysis"]
  EDA --> Features["Feature Preparation"]
  Features --> Model["Regression Modeling"]
  Model --> Diagnostics["Statistical Diagnostics"]
  Diagnostics --> Insights["Tip Prediction Insights"]

  classDef inputs fill:#E0F2FE,stroke:#0284C7,color:#0C4A6E,stroke-width:2.5px;
  classDef process fill:#EDE9FE,stroke:#7C3AED,color:#4C1D95,stroke-width:2.5px;
  classDef data fill:#CCFBF1,stroke:#0D9488,color:#134E4A,stroke-width:2.5px;
  classDef agent fill:#FCE7F3,stroke:#DB2777,color:#831843,stroke-width:2.5px;
  classDef output fill:#FEF9C3,stroke:#CA8A04,color:#713F12,stroke-width:2.5px;
  class Data inputs;
  class Notebook,EDA,Features,Diagnostics process;
  class Model agent;
  class Insights output;
  linkStyle default stroke:#475569,stroke-width:2.5px;
```

## Technology Stack

- Python notebook workflow.
- Pandas and NumPy for data handling.
- scikit-learn style regression workflow.
- Visualization and statistical diagnostics for interpretation.

## Repository Structure

- `DAI_assignment2(23411030).ipynb` - End-to-end restaurant tip prediction notebook.
- `README.md` - Project documentation.

## Getting Started

```bash
python -m venv .venv
source .venv/bin/activate
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

```bash
jupyter notebook
```

## Professional Context

This project demonstrates practical regression analysis, notebook communication, and data-driven reasoning for behavioral prediction.
