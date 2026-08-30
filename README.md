# SDC380_Course_Project
# Stroke Prediction Data Analysis, Visualization & Machine Learning

An end-to-end data science project using Python in Jupyter Notebook to analyze demographic factors, health metrics, and lifestyle variables associated with stroke incidence, predict stroke outcomes, and simulate healthcare intervention strategies.

---

## 📌 Project Overview

This project analyzes patient data from `Stroke_Prediction_Dataset.xlsx` to identify patterns, correlation trends, and risk distributions among stroke patients. Beyond data visualization and exploratory analysis, the project utilizes a **Logistic Regression** machine learning model to predict stroke likelihood, evaluate feature importance, and perform scenario-based counterfactual modeling. Specifically, it simulates targeted health interventions—such as reductions in **Body Mass Index (BMI)** and **Stress Levels**—to measure their impact on patient stroke risk.

---

## 🛠️ Data & Tools Used

* **Language:** Python 3.x
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `openpyxl`, `IPython`
* **Environment:** Jupyter Notebook / Anaconda
* **Dataset File Path:** `C:\Files\Excel\Project\Stroke_Prediction_Dataset.xlsx`

---

## 📊 Key Tasks & Methodology

### Data Visualization & EDA
1. **Age Distribution:** Histogram showing the age spread across all patients in the dataset.
2. **Work Type Breakdown:** Bar chart representing the distribution of employment types among patients diagnosed with a stroke.
3. **Age vs. BMI Relationship:** Scatter plot evaluating Body Mass Index against age specifically for stroke-diagnosed patients.
4. **Correlation Analysis:** Heatmap displaying correlation coefficients between numerical health variables (`Age`, `Body Mass Index (BMI)`, and `Average Glucose Level`).

### Machine Learning & Modeling
5. **Data Preprocessing:** Standardized column names, handled target variable parsing, and applied One-Hot Encoding (`pd.get_dummies`) to convert categorical variables into binary indicators.
6. **Data Splitting:** Divided data into an 80/20 train-test split (`train_test_split`) with a fixed random state for reproducible model evaluation.
7. **Model Training:** Built and trained a Logistic Regression classification model (`max_iter=1000`).
8. **Performance Evaluation:** Evaluated model performance across regression and classification metrics including MAE, MSE, $R^2$, Accuracy, Precision, and Recall.
9. **Feature Importance Ranking:** Extracted and ranked model coefficients to determine the strongest positive and negative predictors of stroke risk.

### Scenario Modeling & Simulated Interventions
10. **Actionable Feature Identification:** Analyzed model coefficients to separate fixed traits (e.g., Age) from modifiable lifestyle factors (e.g., BMI, Stress Levels).
11. **Simulated Interventions:** Filtered high-risk patients (predicted stroke risk greater than the median) and calculated post-intervention risk by simulating a 10% reduction in BMI and a 5% reduction in Stress Levels.
12. **Comparative Visualization:** Generated pre- vs. post-intervention scatter plots comparing individual patient stroke likelihoods to visualize intervention effectiveness against a baseline reference line.
13. **Policy & Clinical Recommendations:** Translated modeling insights into actionable public health strategies, healthcare policy proposals, and targeted preventive care thresholds.

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the required packages installed in your Python environment:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl ipython
