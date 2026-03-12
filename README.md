# PhaseShift
### Predicting CRISPR Clinical Trial Phase Advancement Using Machine Learning

## Overview
PhaseShift is an AI-powered machine learning classifier that predicts whether 
a CRISPR clinical trial will advance to Phase 2/3 or remain in Phase 1. Built 
by a 16-year-old diagnosed with hereditary cardiomyopathy, PhaseShift addresses 
the lack of centralized analyzable CRISPR trial data by combining AI extraction, 
feature engineering, and random forest classification.

## Background
Despite ~250 active CRISPR clinical trials, no centralized analyzable dataset 
existed to track which trials are advancing and why. PhaseShift fills that gap 
by automating data extraction from CRISPR Medicine News using OpenAI's API and 
training a machine learning model on the resulting structured dataset.

## Model Performance
- Accuracy: 78%
- Precision: 0.81
- Recall: 0.74
- F1 Score: 0.77
- Algorithm: Random Forest Classifier
- Validation: 5-fold stratified cross-validation

## Top Predictive Features
1. Enrollment Size (0.21)
2. Disease Category (0.21)
3. Gene-Editing Method (0.15)
4. Disease Area (0.10)
5. Start Year (0.09)

## Dataset
~250 CRISPR clinical trials extracted from CRISPR Medicine News using OpenAI API,
validated against 100 manually labeled trials.
https://www.kaggle.com/datasets/maitreyeesen/crispr-clinical-trials-dataset-2016-2025 

## Files
- `phaseshift_ml_model.py` — full ML pipeline code
- `CRISPR_Data.csv` — cleaned structured dataset
- `phaseshift_feature_importance.png` — feature importance chart
- `phaseshift_confusion_matrix.png` — confusion matrix

## How to Run
1. Open Google Colab
2. Upload CRISPR_Data.csv
3. Run phaseshift_ml_model.py cells in order

## Built With
- Python
- scikit-learn
- pandas
- OpenAI API
- BeautifulSoup
- Google Colab

## Author
Maitreyee — Henry M. Gunn High School, Palo Alto CA
Presented at Golden Gate STEM Fair 2026
