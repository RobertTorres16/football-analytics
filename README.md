# Football Player Analysis — MDP I

Statistical analysis of football player performance data from the 2022-2023 season across Europe's top 5 leagues.

## Overview

This project applies multivariate data analysis techniques to a dataset of **2,689 players**, exploring:

- **PCA** — Dimensionality reduction and player profiling
- **Clustering** (Ward, K-Means, K-Medoids) — Segmenting players by playing style
- **Regression** — Predicting goals and market value
- **Classification** — Predicting market value category (High / Medium / Low)

## Data Sources

- [Kaggle — 2022/2023 Football Player Stats](https://www.kaggle.com/datasets/vivovinco/20222023-football-player-stats) (from FBref)
- Market values: Transfermarkt (September 2022)

## Tech Stack

- **R** — Main analysis language
- **R Markdown** — Report generation
- Key packages: `FactoMineR`, `factoextra`, `dplyr`, `corrplot`, `cluster`, `randomForest`, `caret`

## Usage

Open `football_analytics.Rmd` in RStudio and click **Knit** to generate the HTML report.

### Required packages

```r
install.packages(c("readxl", "dplyr", "FactoMineR", "factoextra", "corrplot",
                   "gridExtra", "stringr", "writexl", "stringdist",
                   "cluster", "ggsci", "randomForest", "caret", "knitr",
                   "ggplot2", "viridis", "MASS", "NbClust", "clValid", "BiocManager"))

if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install("ropls")
```
