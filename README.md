# student-academic-performance-prediction
# 🎓 Student Academic Performance Prediction

This project explores and predicts student exam scores using behavioral and demographic data. Through data cleaning, exploratory analysis, feature engineering, and regression modeling, we identify key academic drivers and forecast performance outcomes.

---

## 📂 Project Overview

- **Goal**: Predict student exam scores based on study habits, attendance, tutoring access, and parental background.
- **Dataset**: Simulated academic performance data of 4,000 students ([Source](https://www.kaggle.com/datasets/firedmosquito831/student-academic-performance-simulation-4000)).
- **Approach**: End-to-end machine learning pipeline with EDA and regression modeling in Python using `pandas`, `seaborn`, `scikit-learn`, and `matplotlib`.

---

## 📊 Dataset Summary

| Feature               | Description                                 |
|-----------------------|---------------------------------------------|
| Gender                | Male or Female                              |
| HoursStudied/Week     | Continuous variable (0 to 16 hours)         |
| Tutoring              | Whether the student receives tutoring       |
| Region                | Urban or Rural                              |
| Attendance (%)        | Attendance percentage                       |
| Parent Education      | Education level of parent                   |
| Exam Score            | Final exam score (Target)                  |

---

## 🧹 Data Cleaning & Feature Engineering

- Missing values in **Parent Education** filled with `"Unknown"`.
- Created new feature: **Study_Level** based on `HoursStudied/Week`:
  - Low, Medium, High, Very High
- Encoded categorical features using `LabelEncoder`.

---

## 📈 Exploratory Data Analysis (EDA)

Key insights discovered:

- 📚 **Tutoring** improves exam performance on average.
- ⏱️ **Hours studied** correlates strongly with higher exam scores.
- 🧾 **Parental education** shows moderate influence.
- 🧍 **Gender** and 🏘️ **Region** show minimal performance impact.

Visualizations included:
- Boxplots by category
- Heatmap of feature correlation
- Distribution plots for continuous features

---

## 🤖 Model: Random Forest Regressor

- Split data: 80% training, 20% testing
- Model: `RandomForestRegressor` from `sklearn.ensemble`
- Evaluated using:
  - 📉 Mean Absolute Error (MAE): `4.19`
  - 📊 Mean Squared Error (MSE): `29.02`
  - ✅ R² Score: `0.90`

---

## 📝 Outputs

| File                          | Description                              |
|-------------------------------|------------------------------------------|
| `Student_Academic_Evalution.ipynb` | Full analysis notebook (EDA → Model)     |
| `predictions.csv`             | Original features + actual & predicted scores |
| `SAP-4000.csv`                | Cleaned dataset used for modeling        |
| `exam_score_model.pkl`        | Trained model (optional for deployment)  |

---

## 📌 Conclusion

The model demonstrates high accuracy in predicting exam scores based on behavioral inputs. **Tutoring**, **hours studied**, and **attendance** are the strongest predictors, making this model useful for early intervention strategies in educational settings.

---

## 🚀 Future Work

- Integrate Power BI for dashboarding
- Explore deep learning for more complex patterns
- Include student feedback or motivation levels as predictors (if available)

---

## 🛠️ Tools & Libraries

- Python, Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🙌 Author

**Asra Pervaiz**  
*Data Scientist | Python + Power BI Enthusiast*

[GitHub](https://github.com/pervaizasra) | [LinkedIn](https://www.linkedin.com/in/asra-pervaiz-712b7b1b5/)

---
