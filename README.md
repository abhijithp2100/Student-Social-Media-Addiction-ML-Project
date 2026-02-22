# Student Social Media Addiction – Machine Learning Project

## Project Overview

This project applies Machine Learning to analyze 705 student records and predict Social Media Addiction Scores using behavioral and lifestyle features.

The dataset contains 13 variables covering daily usage hours, sleep duration, mental health score, academic impact, platform usage, and demographics.

---

## Dataset Summary

- Total Records: 705  
- Total Features: 13  
- Target Variable: Addicted_Score (1–10 scale)  
- Average Addiction Score: 6.44  
- Average Daily Usage: 4.92 hours  
- Average Sleep Duration: 6.87 hours  
- Students Academically Affected: 64.26%  

---

## Key Correlations

- Addiction Score vs Daily Usage: 0.83 (strong positive)
- Addiction Score vs Sleep Hours: -0.76 (strong negative)
- Addiction Score vs Mental Health: -0.95 (very strong negative)

---

## Data Preprocessing

- Removed 3 non-predictive columns (Student_ID, Country, Conflicts_Over_Social_Media)
- Train-Test Split: 75% Training, 25% Testing
- Label Encoding + One-Hot Encoding applied
- Min-Max Scaling applied to 4 numerical features

---

## Models Used

### 1. Linear Regression
- R² Score: ~0.95  
- MAE: Low prediction error  
- Strong linear relationship between features and addiction score  

### 2. K-Nearest Neighbors (KNN) Regression
- Optimal K: 3  
- R² Score: ~0.94  
- MSE: ~0.12  
- Captures non-linear relationships effectively  

---

## Key Findings

- Students with higher daily usage (4–6+ hours) show significantly higher addiction scores.
- Higher addiction levels are associated with reduced sleep (4–6 hours range).
- Mental health score shows a strong inverse relationship with addiction.
- Students academically affected tend to have addiction scores between 7–8.

---

## Tools & Technologies

- Python  
- Pandas & NumPy  
- Matplotlib & Seaborn  
- Scikit-learn  

---

## Conclusion

The models explain approximately 94–95% of the variance in addiction scores, indicating strong predictive relationships between behavioral features and addiction levels. This project demonstrates structured EDA, preprocessing, regression modeling, and model comparison on real-world behavioral data.
