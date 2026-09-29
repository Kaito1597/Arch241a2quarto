# ARCH 241 — Assignment #2

Statistical analysis of a thermal comfort chamber study.

**Author:** Kaito Funada
**Rendered report:** *paste your GitHub Pages link here after you enable it, or
link `analysis.html` in the repo*
[analysis.html](analysis.html)

## What is in here

```
.
├── analysis.qmd      # the analysis — this is the file you edit
├── analysis.html     # the rendered report — commit this too
├── data/
│   └── arch241a2.rda # the dataset, unmodified
├── README.md
└── .gitignore
```

## How to reproduce this

1. Install [R](https://www.r-project.org/),
   [RStudio](https://posit.co/products/open-source/rstudio/) and
   [Quarto](https://quarto.org/docs/get-started/).
2. Install the packages used here:
   ```r
   install.packages(c("ggplot2", "dplyr", "tidyr", "GGally"))
   ```
3. Open `analysis.qmd` in RStudio and click **Render** — or run
   `quarto render analysis.qmd` in a terminal.

## Findings


1.The dataset contains 210 observations that are balanced across sex and experimental conditions
2.TS was roughly symmetric, while TC looks not.
3.Sex and subject look no influence on TS, but experimental conditions have an impact on TS.
4.TS is strongly correlated with Top and PMV
5.TC deviated from normality, whereas TS is normally distributed.
6.Sex did not have a statistically significant effect on TS
7.The linear regression model explain well the relationship between TS and Top.
8.TS differed significantly across experimental conditions.
