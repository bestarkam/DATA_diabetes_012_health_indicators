# Healthcare Predictive Analysis: Diabetes Health Indicators

## Description
This project focuses on the predictive analysis of health indicators related to diabetes using the 2015 "Diabetes Health Indicators" dataset from the BRFSS (Behavioral Risk Factor Surveillance System). The goal is to explore risk factors and build machine learning models capable of identifying individuals at risk for diabetes or prediabetes.

## Project Structure
```text
├── db/                     # Raw data (CSV)
├── notebooks/              # Jupyter Notebooks for EDA and modeling
├── outputs/                # Results, plots, and exported models
│   └── figures/            # Generated visualizations
├── report/                 # Reports and additional documentation
└── requirements.txt        # Project dependencies
```

## Data
The dataset used in this project is the **Diabetes Health Indicators Dataset**, which can be downloaded from [Kaggle](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset).

The specific file used is `diabetes_012_health_indicators_BRFSS2015.csv`. It contains approximately 253,680 entries with 22 variables, including:
- **Target Variable (`Diabetes_012`)**: 0 = no diabetes, 1 = prediabetes, 2 = diabetes.
- **Key Indicators**: HighBP (hypertension), HighChol (high cholesterol), BMI, Smoker, Stroke, HeartDiseaseorAttack, PhysActivity, etc.

## Installation
To run this project locally, ensure you have Python installed, then install the necessary dependencies:

```bash
pip install -r requirements.txt
```

## Usage
1. Explore the analysis notebook: `notebooks/ada_diabetes_analysis.ipynb`.
2. Generated visualizations are available in the `outputs/figures/` folder.

## Analysis Summary (EDA)
- **Class Imbalance**: Approximately 83% of individuals do not have diabetes, requiring specific attention during modeling (e.g., resampling or adapted metrics).
- **BMI Distribution**: Most individuals fall within the 25-35 range (overweight/obese).
- **Correlated Factors**: Hypertension and high cholesterol appear as strong predictors in preliminary analyses.

## Technologies Used
- **Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost
