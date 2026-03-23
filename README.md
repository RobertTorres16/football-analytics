# Análisis de Jugadores de Fútbol — MDP I

Análisis estadístico del rendimiento de los futbolistas de la temporada 2022-2023 en las 5 grandes ligas de Europa.

## Descripción General

Este proyecto aplica técnicas de análisis multivariante de datos a un conjunto de **2.689 jugadores**, explorando:

- **PCA (Análisis de Componentes Principales)** — Reducción de dimensionalidad y perfilado de jugadores.
- **Clustering** (Ward, K-Means, K-Medoids) — Segmentación de jugadores según su estilo de juego.
- **Regresión** — Predicción de goles y valor de mercado.
- **Clasificación** — Predicción de la categoría del valor de mercado (Alto / Medio / Bajo).

## Fuentes de Datos

- [Kaggle — 2022/2023 Football Player Stats](https://www.kaggle.com/datasets/vivovinco/20222023-football-player-stats) (basado en datos de FBref).
- Valores de mercado: Transfermarkt (Septiembre de 2022).

## Tecnologías y Herramientas

- **R** — Lenguaje principal para el análisis.
- **R Markdown** — Generación del informe final.
- Paquetes principales: `FactoMineR`, `factoextra`, `dplyr`, `corrplot`, `cluster`, `randomForest`, `caret`.

## Uso

Abre `football_analytics.Rmd` en RStudio y haz clic en **Knit** para generar el informe en HTML.

### Paquetes requeridos

```r
install.packages(c("readxl", "dplyr", "FactoMineR", "factoextra", "corrplot",
                   "gridExtra", "stringr", "writexl", "stringdist",
                   "cluster", "ggsci", "randomForest", "caret", "knitr",
                   "ggplot2", "viridis", "MASS", "NbClust", "clValid", "BiocManager"))

if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install("ropls")
```
