# Diabetes Hospital Readmission: SQL, Python and Tableau

Predicting which diabetic patients are readmitted within 30 days of discharge.

## Dashboard
[View the interactive Tableau dashboard](PASTE-YOUR-TABLEAU-LINK)

![Dashboard](images/dashboard.png)

## What I did
1. **Cleaned** 101,766 hospital visits with pandas (missing values, invalid rows, new features).
2. **Built a SQLite database** with patients, encounters and lookup tables, plus a joined view.
3. **Trained a Random Forest** model, split by patient so no patient appears in both train and test.
4. **Visualized** the results in Tableau Public.

## Results
- ROC-AUC: [YOUR NUMBER]
- Actual 30-day readmission rate by predicted risk band: Low 5.4%, Medium 9.7%, High 18.9%
- Strongest predictor: number of earlier inpatient stays

## Data
Diabetes 130-US Hospitals (1999-2008), UCI Machine Learning Repository:
https://archive.ics.uci.edu/dataset/296/diabetes-130-us-hospitals-for-years-1999-2008
Download `diabetic_data.csv` and `IDS_mapping.csv` into a `data/` folder.

Citation: Strack et al., "Impact of HbA1c Measurement on Hospital Readmission Rates,"
BioMed Research International, 2014.

## How to run
pip install -r requirements.txt, then run `project.ipynb` from top to bottom.

## Tools
Python (pandas, scikit-learn), SQLite, Tableau Public
