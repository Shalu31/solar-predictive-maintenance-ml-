# Predictive Maintenance for Solar Power Plants 🌞

## Overview
This project builds a machine learning–based predictive maintenance system to detect
early degradation and potential failures in solar inverters using time-series sensor telemetry.

The solution enables proactive maintenance planning, improves uptime reliability,
and reduces unplanned downtime.

---

## Dataset
Sensor telemetry collected from solar power plants, including:
- DC power and AC power output
- Energy yield metrics
- Timestamped inverter-level data

---

## Feature Engineering
- Temporal features: hour, day, month
- Leakage-safe rolling DC power statistics
- Inverter-level encoding
- Historical efficiency-based failure labeling

---

## Modeling Approach
- Problem framed as a binary classification task (failure vs normal)
- Time-based train/test split to prevent data leakage
- Models used:
  - Random Forest Classifier
  - Gradient Boosting Classifier

---

## Evaluation Metrics
- ROC–AUC (primary metric for imbalanced failure data)
- Precision, Recall, F1-score
- Confusion Matrix

---

## Results
- Strong separation between failure and non-failure cases
- Robust generalization with realistic performance after leakage prevention
- Interpretable feature importance for operational trust

---

## Business Impact
- Early identification of inverter degradation
- Reduced unplanned downtime
- Improved maintenance scheduling and power loss prevention

---

## Visualizations
- ROC–AUC curves
- Feature importance
- Power generation trends
- Failure events over time

---

## Tech Stack
- Python, Pandas, NumPy
- Scikit-learn
- Matplotlib

---

## How to Run
```bash
pip install -r requirements.txt
python src/train_model.py
