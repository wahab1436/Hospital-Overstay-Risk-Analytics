Hospital Overstay Risk Analytics

Predict hospital-level overstay risk using real-world inpatient data with dynamic insights and an interactive dashboard.

Project Overview

This project provides a full-stack pipeline for analyzing hospital-level inpatient data to predict overstay risk. It handles raw CSV datasets, performs cleaning, feature engineering, and runs live ML predictions using RandomForest/XGBoost (optional Neural Network). A professional Streamlit dashboard delivers dynamic insights, interactive visualizations, and downloadable results.

Key Features

Live ML Predictions: Upload any hospital-level CSV to get risk probabilities and labels (Low / Medium / High).

Dynamic Insights: Textual summaries and SHAP-based visual explanations update per dataset.

Interactive Dashboard:

Upload & preview CSV

Risk prediction tables & histograms

Feature contribution analysis

Download predictions in CSV

Optional Enhancements: Hospital clustering, ensemble models, Neural Network support.

Dataset

Source: Medicare Inpatient Hospitals – by Provider and Service (CSV)

Type: Hospital-level aggregated data (>100,000 rows)

Columns: Hospital ID, total discharges, average LOS, charges/payments, hospital type/region

Installation
git clone <repo_url>
cd hospital_overstay_mvp
pip install -r requirements.txt
streamlit run frontend/dashboard.py

Usage

Upload a hospital-level CSV dataset.

Preview data and summary statistics.

View predicted overstay risk and risk labels.

Explore feature insights via SHAP plots and textual summaries.

Download CSV with predictions (and optional cluster labels).

Project Structure
hospital_overstay_mvp/
├── data/                  # Raw and processed datasets
├── backend/               # Data ingestion, cleaning, feature engineering, ML
│   ├── ingestion.py
│   ├── cleaning.py
│   ├── features.py
│   └── ml_model.py
├── frontend/              # Streamlit dashboard
│   └── dashboard.py
├── models/                # Trained ML models
├── reports/               # Model evaluation & SHAP analysis
├── requirements.txt       # Python dependencies
└── README.md

Evaluation Metrics

Supervised ML: ROC-AUC, Precision, Recall, F1-score

Clustering (optional): Silhouette score

Deployment

Platform: Streamlit Cloud / Hugging Face Spaces

Live ML Predictions: Upload CSV → dashboard updates dynamically → download results

Technologies Used

Python 3.x

Pandas, NumPy

Scikit-learn, XGBoost

SHAP for explainability

Streamlit, Plotly/Altair for interactive dashboard

Portfolio Value

Demonstrates real-world data handling, feature engineering, and ML modeling

Provides dynamic, live ML insights with professional visualization

Fully deployable, recruiter-ready full-stack project
