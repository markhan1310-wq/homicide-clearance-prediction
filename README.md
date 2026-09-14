# Explainable Machine Learning for Predicting Homicide Clearance in the United States

Code and analysis accompanying the MSc Research Project:

**Explainable Machine Learning for Predicting Homicide Clearance in the
United States: Extending Case-Level Models with Agency and County-Level Data**

The analysis combines:
- Murder Accountability Project Supplementary Homicide Reports (MAP SHR)
- 2020 Law Enforcement Management and Administrative Statistics (LEMAS)
- 2019–2023 American Community Survey (ACS) five-year estimates

Five machine-learning models are evaluated:
- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- Feed-forward Neural Network

Models are evaluated using repeated stratified 80/20 train/test splits.

## Repository structure

- `notebooks/` – analysis notebooks
- `figures/` – model figures
- `results/` – model outputs

## Workflow
1. Data preparation and cleaning
2. MAP-LEMAS-ACS data fusion
3. Feature engineering
4. Missing-data handling
5. Encoding and scaling
6. Model training and evaluation
7. SHAP analysis
8. Subgroup fairness analysis
9. Random forest depth sensitivity analysis

## Data 
The MAP SHR snapshot used in the analysis was `SHR76 24a.csv`.
The snapshot has been archived on Zenodo.

LEMAS data are from the 2020 survey (ICPSR 38651).

ACS data are the 2019–2023 five-year estimates, using:
- S1701 for poverty
- B23025 for unemployment

## Reproducibility
The notebooks are intended to be run in numerical order.

The raw datasets are not redistributed through this repository.
See `data/README.md` for source information.

## License

CC BY 4.0

  
