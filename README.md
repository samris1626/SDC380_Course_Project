# SDC380_Course_Project
# Stroke Prediction Data Analysis, Visualization & Machine Learning

An exploratory data analysis and predictive modeling project using Python in Jupyter Notebook to analyze demographic factors, health metrics, and lifestyle variables associated with stroke incidence, as well as predict stroke outcomes using Machine Learning.

---

## 📌 Project Overview

This project analyzes patient data from `Stroke_Prediction_Dataset.xlsx` to identify patterns, correlation trends, and risk distributions among stroke patients. Beyond data visualization, the project utilizes a **Logistic Regression** machine learning model to predict stroke likelihood, evaluate feature importance, and analyze key risk factors such as **Age**, **BMI**, **Average Glucose Level**, and **Work Type**.

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
5. **Data Preprocessing:** Standardized column names and applied One-Hot Encoding (`pd.get_dummies`) to convert categorical variables into binary indicators.
6. **Data Splitting:** Divided data into an 80/20 train-test split (`train_test_split`) for objective model evaluation.
7. **Model Training:** Built and trained a Logistic Regression classification model.
8. **Performance Evaluation:** Evaluated model performance across key metrics including MAE, MSE, $R^2$, Accuracy, Precision, and Recall.
9. **Feature Importance Ranking:** Extracted and ranked model coefficients to determine the strongest predictors for stroke risk.

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the required packages installed in your Python environment:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl ipython
