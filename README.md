Hospital Overstay Risk Analytics

Predicting hospital-level overstay risk using real-world inpatient data with dynamic insights and interactive dashboards.

Project Overview

This project provides a full-stack, end-to-end pipeline for analyzing hospital-level inpatient data to predict overstay risk. It handles raw CSV datasets, performs cleaning, feature engineering, and runs live ML predictions using RandomForest/XGBoost with optional Neural Network. A professional Streamlit dashboard delivers dynamic, dataset-specific insights, interactive visualizations, and downloadable results.

Key Features

Live ML Predictions: Upload any hospital-level CSV and get risk probabilities and labels (Low / Medium / High).

Dynamic Insights: Textual and visual explanations update per uploaded dataset using SHAP plots.

Interactive Dashboard:

Upload & preview CSV data

Risk prediction tables and probability distributions

Feature contribution analysis

Download results in CSV format

Professional Styling: Neutral color palette, minimalistic charts, clean fonts.

Optional Enhancements: Hospital clustering (PCA/UMAP), ensemble modeling, Neural Network support.

Dataset

Source: Medicare Inpatient Hospitals – by Provider and Service (CSV)

Type: Hospital-level aggregated data

Columns include: Hospital ID, total discharges, average LOS, payments/charges, hospital type/region, and more

Size: >100,000 rows, real-world data, uncleaned

Installation
# Clone the repo
git clone <repo_url>
cd hospital_overstay_mvp

# Install dependencies
pip install -r requirements.txt

# Run the dashboard
streamlit run frontend/dashboard.py

Usage

Upload a hospital-level CSV dataset.

Preview data and check summary statistics.

View predicted overstay risk probabilities and risk labels.

Explore feature insights via SHAP plots and dynamic textual explanations.

Download CSV with predictions and optional cluster labels.


Evaluation Metrics

Supervised ML: ROC-AUC, Precision, Recall, F1-score

Clustering (optional): silhouette score

Deployment

Platform: Streamlit Cloud / Hugging Face Spaces

Features: Upload new CSV → live predictions → interactive dashboard → download results

Technologies Used

Python 3.x

Pandas, NumPy for data handling

Scikit-learn, XGBoost for ML

SHAP for explainability

Streamlit, Plotly/Altair for interactive dashboard

Portfolio Value

Demonstrates real-world data ingestion, cleaning, feature engineering

Shows dynamic, live ML predictions with professional visualization

Fully deployable full-stack project, recruiter-ready
