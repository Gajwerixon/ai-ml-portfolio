## 📝 Project Summary

The goal of this project is to predict students' exam scores using demographic, academic, and lifestyle-related features.

The project started with an **Exploratory Data Analysis (EDA)** to uncover key patterns and relationships within the data:
* **`study_hours`** showed the strongest positive correlation with `exam_score`.
* **`class_attendance`** and **`sleep_hours`** demonstrated weaker, yet positive, relationships with student performance.
* Noticeable variations in exam scores were also observed across categories like **`sleep_quality`**, **`study_method`**, and **`facility_rating`**.

### ⚙️ Preprocessing Pipeline
Before training the model:
1. **Train/Test Split:** Data was divided into dedicated training and testing sets.
2. **Feature Removal:** Dropped `student_id` as it serves solely as an identifier without predictive value.
3. **Categorical Encoding:** Applied `OneHotEncoder` to transform categorical variables.
4. **Numerical Scaling:** Kept numerical features unchanged.

> 💡 **Feature Expansion:** Preprocessing expanded the original 11 features into **30 numerical features** for model training.

---

## 📉 Baseline Model

A **Linear Regression** model was established as the initial baseline to set a performance benchmark.

### Test Set Performance

| Metric | Score | Description |
| :--- | :---: | :--- |
| **MAE** | **7.86** | Predictions deviate by ~7.86 points on average |
| **RMSE** | **9.77** | Penalizes larger error margins across predictions |
| **R²** | **0.73** | Explains **73%** of the variance in exam scores |

The $R^2$ score of **0.73** indicates that even a simple linear model captures a substantial portion of the underlying relationships in the dataset.