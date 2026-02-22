# Student Social Media Addiction – Machine Learning Project

## Project Overview

This project applies Machine Learning techniques to analyze 705 student records and predict Social Media Addiction Scores using behavioral and lifestyle features.

The dataset contains 13 variables covering daily usage hours, sleep duration, mental health score, academic impact, platform usage, and demographic attributes. The objective is to build and evaluate regression models capable of predicting addiction levels based on these features.

---

## Project Structure

```
Student Social Media Addiction ML Project
│
├── data
│   └── Students Social Media Addiction.csv
│
├── report
│   └── Student Social Media Addiction Project Report.pdf
│
├── scripts
│   └── Students Social Media Addiction ML.ipynb
│
└── visualizations
    ├── 01_usage_distribution.png
    ├── 02_addiction_distribution.png
    ├── 03_usage_boxplot.png
    ├── 04_addiction_vs_sleep.png
    ├── 05_addiction_vs_academic_impact.png
    ├── 06_addiction_by_gender_academic.png
    ├── 07_addiction_by_relationship_status.png
    ├── 08_correlation_heatmap.png
    ├── dashboard-preview.png
    ├── dataset_sample.png
    └── statistical_summary.png
```

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

## Data Preprocessing

- Removed 3 non-predictive columns (Student_ID, Country, Conflicts_Over_Social_Media)  
- 75% Training / 25% Testing split  
- Label Encoding and One-Hot Encoding applied to categorical features  
- Min-Max Scaling applied to numerical features  
- No missing values detected  

---

## Models Used

### Linear Regression
- R² Score: ~0.95  
- Low Mean Absolute Error  
- Demonstrates strong linear relationships between features and addiction score  

### K-Nearest Neighbors (KNN) Regression
- Optimal K: 3  
- R² Score: ~0.94  
- Mean Squared Error: ~0.12  
- Captures local and non-linear patterns  

---

## Key Findings (Machine Learning Insights)

- Linear Regression explains approximately 95% of the variance in addiction scores.
- KNN Regression achieved comparable performance (~94% R²), validating model stability.
- Similar performance across both models suggests predominantly linear relationships in the dataset.
- Strong feature correlations significantly contribute to predictive accuracy.
- Proper preprocessing (split before encoding, scaling, encoding strategy) helped prevent data leakage.
- Low prediction error indicates strong generalization on unseen test data.
- Simpler models performed competitively due to strong linear dependencies among features.

---

## Tools & Technologies

- Python  
- Pandas & NumPy  
- Matplotlib & Seaborn  
- Scikit-learn  

---

## Conclusion

The regression models demonstrate high predictive performance, with R² values around 0.94–0.95. The results indicate strong linear relationships between daily usage, sleep duration, mental health, and social media addiction levels.

This project showcases end-to-end machine learning workflow including EDA, preprocessing, feature engineering, regression modeling, evaluation, and model comparison.
