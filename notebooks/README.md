# Notebooks

This folder contains the Jupyter notebooks used for the analysis.

The notebooks contain saved outputs from the analysis so that the reported results can be inspected without rerunning the entire workflow. Some parts of the analysis, particularly the SHAP explainability analysis, are computationally expensive and may take several hours to reproduce from scratch. Specifically, computing SHAP values across all 10 train/test splits for the Random Forest model takes approximately 6-7 hours in total, given the model's tree depth and test set size. Intermediate results are checkpointed to `results/` as CSV files after each split completes, so an interrupted run can be resumed without starting over.

The raw data files are not included in this repository because of their file size. Place the downloaded source files under the `data/` directory using the following structure:

- data/map/SHR76_24a.csv
- data/lemas/DS0001/38651-0001-Data.tsv
- data/poverty/ACSST5Y2023.S1701-Data.csv
- data/unemployment/ACSDT5Y2023.B23025-Data.csv

The original data can be found from the sources listed in the report's Data Availability section. The MAP data specifically has been archived at https://doi.org/10.5281/zenodo.22739618 to ensure the exact snapshot used in this analysis remains available, since the Murder Accountability Project periodically updates its dataset.
