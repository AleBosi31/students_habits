# 🎓 Student Well-Being and Academic Performance

This project explores the relationship between students' psychophysical well-being and their academic performance using a dataset of lifestyle habits and exam scores. The goal is to determine whether healthy behaviors — such as proper sleep, exercise, screen time management, and mental health — are linked to improved academic outcomes.

---

## 📘 Introduction

Academic performance is shaped by more than just study hours or classroom attendance. In recent years, increasing attention has been given to the impact of mental and physical well-being on learning. This project investigates to what extent lifestyle habits influence students' final exam scores.

Using exploratory data analysis, correlation studies, and predictive modeling (Linear Regression and Random Forest), we aim to answer the question:

> _"Can students who take better care of their bodies and minds perform better academically?"_

---

## 📊 Dataset Overview

The dataset contains records from 909 students, including the following key features:

- `study_hours_per_day`
- `attendance_percentage`
- `sleep_hours`
- `exercise_frequency`
- `mental_health_rating` (scale 1–10)
- `screentime_hours` (social media + Netflix)
- `diet_quality` (encoded as Poor = 0, Fair = 1, Good = 2)
- `exam_score` (target variable)

Descriptive statistics indicate:
- Average exam score: ~69.6  
- Average screentime: ~4.3 hours/day  
- Average mental health rating: ~5.5  
- Study hours and screentime show strong influence on performance.

---

## 🔍 Exploratory Data Analysis

Several visualizations were used to explore patterns and relationships:
- **Boxplots** for diet quality and exam scores
- **Scatterplots** for sleep, exercise, mental health, screentime vs. performance
- **Correlation heatmap** to assess linear relationships

Key observations:
- Higher `study_hours` → significantly better exam scores
- Better `mental_health_rating` → moderately better scores
- More `screentime_hours` → slightly worse academic outcomes
- `sleep`, `exercise`, and `diet` showed weaker associations

---

## 🤖 Predictive Modeling

Two models were trained and compared:

| Model               | MAE  | RMSE | R²   |
|--------------------|------|------|------|
| Linear Regression  | 4.37 | 5.46 | 0.89 |
| Random Forest      | 4.39 | 5.62 | 0.88 |

- **Linear Regression** performed slightly better and offered interpretability through coefficients.
- **Random Forest** confirmed the same variable importance, with `study_hours_per_day` dominating both models.

---

## 📌 Conclusions

- **Study habits** are by far the strongest driver of academic success.
- **Mental well-being** and **screentime** also play relevant roles.
- Other wellness factors (sleep, diet, exercise) may support performance indirectly but are not strong predictors on their own.
- The findings suggest that promoting better mental health and limiting screen time, in addition to fostering strong study routines, could benefit students' academic outcomes.

---

## 🛠️ Tech Stack

- Python (pandas, seaborn, matplotlib, scikit-learn)
- Jupyter Notebook
- Visualizations with `seaborn` and `matplotlib`
- Modeling with `scikit-learn`
