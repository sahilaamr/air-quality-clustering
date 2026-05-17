# Global Air Quality Clustering Analysis (2023)

![Python](https://img.shields.io/badge/Python-3.x-blue)
![sklearn](https://img.shields.io/badge/sklearn-KMeans%20%7C%20PCA-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## Overview
This project analyzes global air quality data from 999 city-level records 
across multiple countries (2023) using unsupervised machine learning techniques. 
K-Means Clustering and Principal Component Analysis (PCA) were applied to 
group cities by pollution patterns and identify dominant environmental factors 
affecting air quality.

> Dataset source: [Global Air Quality Data – Kaggle (WAQI)](https://www.kaggle.com/)

---

## Research Questions
- Do meteorological factors (wind speed, temperature, humidity) significantly 
  influence pollutant concentration levels?
- How are pollutants distributed across different city clusters?
- Which country/city records the highest overall pollution levels?

---

## Methods & Tools
| Step | Method/Tool |
|------|------------|
| Data Cleaning | pandas, isnull check |
| Normalization | MinMaxScaler (sklearn) |
| Optimal Cluster Selection | Elbow Method + Silhouette Coefficient |
| Clustering | K-Means (k=7) |
| Dimensionality Reduction | Principal Component Analysis (PCA) |
| Regression Analysis | Linear Regression (sklearn) |
| Visualization | matplotlib, seaborn |
| Environment | Google Colab |

---

## Key Findings
- **7 distinct pollution clusters** identified, each with unique pollutant profiles:
  - Cluster 3: High pollution, warm temperature, low wind speed
  - Cluster 4: High PM2.5 & PM10 with highest humidity levels
  - Cluster 5: Low-moderate pollution, high temperature, strong wind
- **Berlin, Germany** recorded the highest total pollutant concentration 
  (612.83) across all cities in the dataset
- **PM10 and O3** were the dominant pollutants across most clusters, 
  detected in cities like Johannesburg, Paris, Toronto, and Seoul
- Meteorological factors (temperature, humidity, wind speed) showed 
  **very low influence** on pollutant levels — all R² scores near 0, 
  confirming pollution is driven by human activity rather than weather


