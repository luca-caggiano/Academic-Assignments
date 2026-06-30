
# The Colonial Origins of Comparative Development: A Python Replication



## Overview

This folder contains a Python-based replication of the highly influential economic paper *"The Colonial Origins of Comparative Development: An Empirical Investigation"* by Acemoglu, Johnson, and Robinson (2001).

Originally assigned as a practical university exercise using Stata, I have completely reproduced the analysis in Python.

## Objective

The primary objective of this project is to practice and demonstrate technical skills in dealing with real-world data and statistical modeling. This project shows the ability to:
* **Implement Advanced Econometrics:** Move beyond basic regressions to implement Instrumental Variable (IV) strategies (Two-Stage Least Squares).
* **Validate Statistical Assumptions:** Assess the credibility of instruments and conduct First Stage relevance checks.
* **Communicate Results:** Generate tables to clearly communicate statistical findings.

## The Data

The analysis relies on the dataset compiled by the authors, which includes:
* **Economic Outcomes:** Log GDP per capita (PPP, 1995) and log output per worker.
* **Institutional Metrics:** Average protection against expropriation risk.
* **Historical Data:** Log of European settler mortality, used as the primary instrumental variable.
* **Geographic Controls:** Latitude (distance from the equator) and continent dummies (Africa, Asia, Other).


## Technologies & Libraries Used

* **Language:** Python 3
* **Data Manipulation & Visualization:** `pandas`, `numpy`, `matplotlib.pyplot`, `seaborn`
* **Econometric Modeling:** `statsmodels` (for OLS estimation), `linearmodels.iv` (for IV-2SLS estimation)
* **Result Formatting:** `stargazer` 



## Methodology & Key Steps

1. **Visualizing the Reduced Form:** Recreating the scatter plot mapping log settler mortality to log GDP per capita to illustrate the raw, reduced-form relationship.

2. **Baseline OLS Estimates:** Regressing economic performance on institutional quality, progressively adding geographic controls to highlight the limits of standard OLS (omitted variable bias and reverse causality).


3. **Instrumental Variable (IV-2SLS) Strategy:**
   * **First Stage:** Validating the instrument by regressing current institutions on historical settler mortality.

   * **Second Stage:** Estimating the causal impact of the exogenous variation in institutions on modern economic performance across different sample restrictions (e.g., excluding Neo-Europes or Africa).





## 💡 Key Findings

The replication successfully confirms the original paper's findings:
* **Institutions Matter:** There is a massive, statistically significant, and causal impact of institutional quality (property rights) on long-term economic development.
* **Geography is Secondary:** Once the endogeneity of institutions is controlled for via the settler mortality instrument, previously significant geographic variables (like latitude or continent dummies) lose their explanatory power.

## References
Acemoglu, Daron, Simon Johnson, and James A. Robinson. 2001. "The Colonial Origins of Comparative Development: An Empirical Investigation." American Economic Review 91 (5): 1369–1401.