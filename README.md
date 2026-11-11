# Employee Attrition Prediction

Educational machine learning project by Nivedha Sivakumar.

## Changes from the saved notebook
- Removed unused TensorFlow and patsy dependencies
- Replaced arbitrary category numbers with training-fitted one-hot encoding
- Added scaling, imputation, stratified split, baseline and held-out metrics
- Removed raw employee previews and invalid synthetic prediction example

## Run locally
Use Python 3.12, install `pip install -r requirements.txt`, and place an authorized copy of `IBM Attrition Data.csv` beside the notebook (or in `data/` as shown). Dataset redistribution rights have not been established, so input data is not included. Run all notebook cells in order.

## Validation
Executed successfully top-to-bottom on the local source data using Python 3.12. Exact tested package versions are recorded in requirements-lock.txt. Saved charts were visually reviewed. Historical output claims have been removed; new conclusions must follow the revised evaluation.

## Limits
This is a learning project, not a deployed decision system. Holdout scores do not establish external validity, fairness, or causal effects. 

## Observed results

The model detected only 1 of 71 observed departures in the holdout at its default threshold; its accuracy is essentially equal to the majority baseline. ROC AUC is 0.636. Treat this as a limited baseline experiment, not a useful attrition screening system. Further work needs training-only threshold selection and evaluation on fresh data.
