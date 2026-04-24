# ctdna-mpp-ipsw-simulation

This repository contains the R code used to reproduce the **simulation study** reported in **Section 3** and **Table 1** of the manuscript:

**Marginal Regression Analysis of Marked Point Processes for ctDNA Data with Informative Censoring**

The repository is intended to provide a minimal, simulation-only code archive for reproducibility.

## Repository contents

- `simulate_analysis.Rmd` — main R Markdown file for reproducing the simulation study.
- `results/` — optional directory for saving generated output files.
- `LICENSE` — MIT License.
- `.gitignore` — excludes common temporary and local files.

## Simulation scope

The code in this repository reproduces the simulation settings corresponding to the final manuscript version and **Table 1**, including:

- sample sizes `n = 200` and `n = 500`;
- low and high censoring scenarios;
- four heterogeneity levels `σ² ∈ {0, 0.1, 0.25, 0.5}`;
- `200` simulation replicates for each scenario;
- IPSW estimation using a two-step procedure based on Cox-model-derived survival weights and a weighted objective function.

## Software requirements

The code was written in **R** and uses the following packages:

- `survival`
- `writexl`
- `dplyr`

## How to run

1. Open `simulate_analysis.Rmd` in RStudio (or another R Markdown-compatible environment).
2. Install any missing packages.
3. Run all code chunks sequentially.
4. Save any generated summary tables or exported files in the `results/` folder if desired.

## Data availability

This repository contains **simulation code only**.

The clinical trial data used in the manuscript's case study are **not included** in this repository and are **not publicly distributed here**.

## Reproducibility note

This repository is designed to reproduce the simulation results corresponding to **Table 1**. The manuscript text should be interpreted according to the final simulation settings aligned with those reported results.

## Suggested code availability statement

The R code used to reproduce the simulation study reported in Section 3 is publicly available in this GitHub repository. The clinical trial data used in the case study are not publicly available.
