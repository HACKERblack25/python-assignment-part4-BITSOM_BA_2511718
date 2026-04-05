# 📊 Assignment — Part 4: Data Visualization & Machine Learning

## 📌 Overview

This project focuses on analyzing student performance data, creating meaningful visualizations, and building a machine learning model to predict whether a student will pass or fail.

The workflow covers:

* Data exploration using Pandas
* Data visualization using Matplotlib and Seaborn
* Building a classification model using Logistic Regression

---

## 📂 Project Structure

```
python-assignment-part4/
│
├── part4_visualization_ml.ipynb   # Main notebook (all code + outputs)
├── students.csv                  # Dataset used for analysis
│
├── plot1_bar.png                 # Avg score per subject (Matplotlib)
├── plot2_hist.png                # Math score distribution
├── plot3_scatter.png             # Study hours vs avg score
├── plot4_box.png                 # Attendance vs pass/fail
├── plot5_line.png                # Math vs Science trend
│
├── plot6_seaborn_bar.png         # Seaborn bar plot (Pass vs Fail)
├── plot7_seaborn_scatter.png     # Seaborn scatter + regression
│
├── plot8_feature_importance.png  # ML feature importance
└── README.md                     # Project documentation
```

---

## 📊 Dataset Description

The dataset contains performance data of 15 students with the following columns:

* `name` → Student name
* `math, science, english, history, pe` → Subject scores
* `attendance_pct` → Attendance percentage
* `study_hours_per_day` → Daily study hours
* `passed` → Target variable (1 = Pass, 0 = Fail)

---

## 🧪 Task 1 — Data Exploration

Performed using **Pandas**:

* Displayed first 5 rows using `.head()`
* Checked dataset shape and data types
* Generated summary statistics using `.describe()`
* Counted pass vs fail students
* Compared subject-wise averages for passing vs failing students
* Identified the top-performing student based on average score

---

## 📈 Task 2 — Data Visualization (Matplotlib)

Created and saved the following plots:

1. **Bar Chart** — Average score per subject
2. **Histogram** — Distribution of math scores (with mean line)
3. **Scatter Plot** — Study hours vs average score (Pass vs Fail)
4. **Box Plot** — Attendance comparison (Pass vs Fail)
5. **Line Plot** — Math vs Science scores across students

👉 All plots include titles, labels, and legends where required.

---

## 🎨 Task 3 — Data Visualization (Seaborn)

Created advanced visualizations using Seaborn:

* **Bar Plot (Subplots)**
  Compared average Math and Science scores for Pass vs Fail students

* **Scatter Plot with Regression**
  Visualized relationship between attendance and average score
  Added regression lines for both Pass and Fail groups

💡 *Observation:*
Seaborn simplifies statistical visualization and reduces code compared to Matplotlib, while Matplotlib provides more customization control.

---

## 🤖 Task 4 — Machine Learning

### Model Used:

* **Logistic Regression**

### Steps Performed:

1. **Data Preparation**

   * Selected features (X) and target (y)
   * Split data into training (80%) and testing (20%)
   * Scaled features using `StandardScaler`

2. **Model Training**

   * Trained Logistic Regression model on scaled data
   * Evaluated training accuracy

3. **Model Evaluation**

   * Predicted on test data
   * Calculated test accuracy
   * Compared actual vs predicted results with student names

4. **Feature Importance**

   * Extracted coefficients from the model
   * Visualized importance using a horizontal bar chart
   * Positive values → increase chance of passing
   * Negative values → increase chance of failing

5. **New Student Prediction**

   * Predicted result for a custom student input
   * Displayed prediction probability

---

## 📌 Key Insights

* Students with higher **study hours** and **attendance** are more likely to pass
* Strong performance across subjects correlates with higher pass probability
* Logistic Regression provides interpretable results through feature coefficients

---

## ⚠️ Notes

* Dataset is small (15 records), so accuracy may vary
* Focus is on understanding workflow, not achieving perfect predictions

---

## ✅ Final Status

✔ Data cleaned and analyzed
✔ 7 visualizations created
✔ Machine learning model built and evaluated
✔ Feature importance visualized
✔ Project successfully completed
