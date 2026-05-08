# Android Malware Classification Using System Call and Binder Call Frequency Features

## Overview
This project focuses on improving Android malware classification accuracy using system-call and binder-call frequency as behavior-based features, while keeping the detection process easy to understand. It analyzes user behavior via a survey (primary data) and evaluates machine learning models on a dynamic malware dataset, CICMalDroid 2020 (secondary data).

## Data Collection
- **Primary Data:** A survey of 31 participants (Al-Hussein Technical University students) aimed at understanding user behavior, security awareness, and practices regarding Android applications.
- **Secondary Data:** CICMalDroid 2020 dataset containing 11,598 rows and 471 columns of system call and binder call frequencies.

## Methodology
The study follows the Research Onion Model:
- **Philosophy:** Pragmatism
- **Approach:** Deduction
- **Methodological Choice:** Mixed method (Quantitative for malware dataset, Qualitative for survey)
- **Time Horizons:** Cross-sectional
- **Techniques & Procedures:** Python (pandas, NumPy, scikit-learn, xgboost) for ML; Google Forms for the survey.

### Machine Learning Models
Five models were trained and evaluated (80% train, 20% test split):
- Random Forest
- Support Vector Machine (SVM)
- XGBoost
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes

## Key Results
- **XGBoost** achieved the highest accuracy of **94.22%** after feature selection (reducing from 471 to 100 features).
- **Random Forest** achieved an accuracy of **93.97%**.
- The survey results indicated that frequent app installations, low permission awareness, and limited use of mobile security tools increase the risk of malware exposure.

## Conclusion
The study confirms that automated behavior-based malware detection using system call frequency and ensemble machine learning models like XGBoost and Random Forest is highly effective and interpretable. It also highlights the need for improved user security awareness.
