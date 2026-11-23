# Dependence and Network Structure in the WTI Crude Oil Market

This project was undertaken in completion of **COMP0047 Data Science**, a required module in the **MSc Computational Finance** programme at **University College London (UCL)**.

This exploratory study examines how different methods describe relationships among market features and with West Texas Intermediate (WTI) crude oil returns.

## Analysis

- **Feature dependence.** Compares Pearson, Spearman and Kendall correlations with normalised mutual information to rank features by their association with next-day WTI log returns.
- **Network structure.** Uses pairwise normalised mutual information to construct a minimum spanning tree (MST), a planar maximally filtered graph (PMFG) and a triangulated maximally filtered graph (TMFG) of the features.
- **Directional dependence.** Uses pairwise Granger causality tests and two transfer entropy estimators, histogram-based and Gaussian, to examine relationships between features and same-day WTI log returns in both directions.

## Data and Contributions

The analysis uses 1,895 daily observations and 76 features from 31 January 2017 to 3 March 2026. The features cover market prices and volatility, oil inventories, geopolitical indicators and survey data.

The group coursework supplied the starting dataset and baseline diagnostics. The extended dependence, network and directional analyses are individual work.

## Project Files

- [Analysis notebook](Code/WTI_Crude_Oil_Analysis.ipynb)
- [Full report](WTI_Crude_Oil_Analysis_Report.pdf)

Note: A later review identified that the MST and PMFG community analysis used distances as connection strengths. The notebook and the report retain the original calculations, including the affected PMFG weighted clustering results. All work presented here is shown as originally submitted.

Run the notebook with `Code/` as the working directory. It reads the prepared dataset from `Data/` and saves plots to `Figures/`.
