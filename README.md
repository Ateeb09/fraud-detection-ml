# Unsupervised Fraud Detection (Machine Learning) 
 
## Problem Statement 
Detect fraudulent transactions using unsupervised learning techniques due to extreme class imbalance and limited reliable fraud labels. 
 
## Dataset 
Transaction dataset with highly imbalanced fraud cases (~2%%). 
Fraud labels are used **only for evaluation**, not for training. 
 
## Approach 
- Exploratory Data Analysis (EDA) 
- Feature Engineering and Scaling 
- Isolation Forest (baseline anomaly detection) 
- Autoencoder (deep learning reconstruction model) 
- Threshold tuning and PCA-based failure analysis 
 
## Models Used 
- Isolation Forest (scikit-learn) 
- Autoencoder (PyTorch) 
 
## Results Summary 
- Both models failed to detect rare fraud cases under strict thresholds. 
- Threshold tuning increased sensitivity but led to higher false positives. 
- Isolation Forest showed better stability and lower false-positive rates. 
- PCA visualization confirmed strong overlap between fraud and normal samples. 
 
## Key Insights 
- Accuracy is misleading for highly imbalanced datasets. 
- Model complexity cannot compensate for poor feature separability. 
- Simpler models may outperform deep models when data is limited. 
 
## Project Scope 
This repository focuses on **model development and analysis only**. 
No API, frontend, or database is included. 
 
## Future Work 
- Temporal and behavioral feature engineering 
- Hybrid anomaly detection approaches 
- Deployment via API with database-backed logging 
