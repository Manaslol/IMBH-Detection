# IMBH-Detection

# Detecting Intermediate-Mass Black Holes in Globular Clusters

This project frames IMBH discovery in globular clusters as an unsupervised anomaly-detection problem using the Baumgardt et al. (2023) catalog.

## Data
- Fundamental Parameters of Galactic Globular Clusters (v4, March 2023)

## Method
- Robust preprocessing (log-scaling, median imputation, RobustScaler)
- Ensemble anomaly detection: Isolation Forest, LOF, Elliptic Envelope, PCA reconstruction
- Voting-based consensus to flag outliers

## Results
- Statistically significant outlier clusters identified
- Known high-interest systems (e.g., Omega Centauri) recovered

## How to run
```bash
pip install -r requirements.txt
jupyter notebook imbh_detection.ipynb
