# Overview

This e-commerce behavior analysis and prediction system is designed to process and analyze customer clickstream data, offering predictive insights through machine learning and interactive visualizations. The project uses a Kaggle Customer Data For Behavior Analysis dataset (https://www.kaggle.com/datasets/shriyashjagtap/e-commerce-customer-for-behavior-analysis) to model customer journeys, predict purchase intentions, and segment behavioral patterns. The system integrates with python with Jupyter Notebook's compatible format and uses a Random Forest classifier to guide predictions. It also includes visual tools like sunburst charts and line graphs for a business-friendly summary of customer navigation and drop-off points. This package includes the original dataset, a paper that elaborates the work in detail and a code file that contains all the visualization implementation and the model evaluation module.

# Requirements

In order to preform the job as expected, please ensure following environment / packages are set properly:

- Operating System with Jupyter Notebook support
- Jupyter Notebook installed
- Python ≥ 3.8
- Required Python libraries:
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
pip install plotly
pip install scikit-learn

# Procedures

1. Prepare Your Dataset
Place the original dataset file ecommerce_customer_data_large.csv in the same folder as the notebook or specify its full path in the code.

2. Run the Notebook
Launch Jupyter Notebook and open code.ipynb. Execute each cell in order. The code will be executed as following:

2.1. Data Cleaning & Enrichment
- Renames columns for clarity
- Fills missing values (e.g., treats missing returns as 0)
- Drops exact duplicates
- Converts and extracts features from datetime fields
- Generates RFM (Recency, Frequency, Monetary) metrics per customer

2.2. Save Enriched Dataset
The enriched dataset is saved as ecommerce_enriched.csv for further modeling or reporting.

2.3 Visualizations
The code file will create charts using matplotlib or plotly to explore customer behavior across:
- Age groups
- Product categories
- Hour-of-day and day-of-week patterns

2.4 Modeling & Evaluation
- Train a Random Forest classifier to predict churn
- Evaluate performance using precision, recall, F1-score, and confusion matrix