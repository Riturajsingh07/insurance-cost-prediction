# 🏥 Insurance Cost Prediction

A Machine Learning project that predicts **medical insurance charges** based on personal and demographic information such as age, BMI, number of children, smoking status, gender, and region.

The project uses **Python, Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn** to perform data preprocessing, exploratory data analysis, model training, and evaluation.

---

## 📌 Project Overview

Medical insurance costs can vary significantly depending on an individual's characteristics and lifestyle factors.

This project builds a **Linear Regression model** to predict insurance charges and evaluates its performance using standard regression metrics.

### 🎯 Objectives

* Analyze factors affecting medical insurance charges
* Clean and preprocess the dataset
* Perform Exploratory Data Analysis (EDA)
* Convert categorical variables into numerical features
* Train a Linear Regression model
* Compare model predictions with actual insurance charges
* Evaluate model performance using MAE, RMSE, and R²
* Analyze prediction errors using residual analysis

---

## 📊 Dataset

The dataset contains information about individuals and their medical insurance costs.

### Main Features

| Feature    | Description                              |
| ---------- | ---------------------------------------- |
| `age`      | Age of the individual                    |
| `sex`      | Gender of the individual                 |
| `bmi`      | Body Mass Index                          |
| `children` | Number of children/dependents            |
| `smoker`   | Smoking status                           |
| `region`   | Residential region                       |
| `charges`  | Medical insurance cost — target variable |

**Target Variable:** `charges`

---

## 🛠️ Technologies Used

* **Python**
* **Pandas** – Data manipulation and preprocessing
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Scikit-learn** – Machine Learning
* **Jupyter Notebook** – Development and analysis

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Feature Encoding
   ↓
Train-Test Split
   ↓
Linear Regression Model
   ↓
Prediction
   ↓
Model Evaluation
   ↓
Residual Analysis
```

---

## 🔍 Exploratory Data Analysis

The project explores relationships between insurance charges and important variables such as:

* Age
* BMI
* Smoking status
* Number of children
* Gender
* Region

Visualizations are used to identify patterns and understand which features may have a stronger relationship with insurance costs.

---

## 🤖 Machine Learning Model

### Linear Regression

A Linear Regression model is trained to predict medical insurance charges.

The dataset is divided into:

* **Training set** – used to train the model
* **Testing set** – used to evaluate predictions on unseen data

The general relationship learned by the model can be represented as:

```text
Predicted Charges = β₀ + β₁X₁ + β₂X₂ + ... + βₙXₙ
```

---

## 📈 Model Evaluation

The model is evaluated using:

### Mean Absolute Error (MAE)

Measures the average absolute difference between actual and predicted insurance charges.

```text
MAE = average(|Actual - Predicted|)
```

### Root Mean Squared Error (RMSE)

Measures prediction error while giving greater weight to larger errors.

```text
RMSE = √average((Actual - Predicted)²)
```

### R² Score

Measures how much variation in the target variable is explained by the model.

```text
R² = 1 - (SS_res / SS_total)
```

> The actual metric values are generated when the notebook/script is executed. They are intentionally not hard-coded here.

---

## 📉 Residual Analysis

Residuals are calculated as:

```python
residuals = y_test - predictions
```

A residual plot is used to analyze the difference between actual and predicted values.

```python
plt.scatter(predictions, residuals)

plt.axhline(0, linestyle="--")

plt.xlabel("Predicted charges")
plt.ylabel("Residual: actual minus predicted")
plt.title("Residuals")
plt.show()
```

This helps identify patterns in prediction errors and assess whether the model is capturing the relationship between the features and target effectively.

---

## 📁 Project Structure

```text
insurance-cost-prediction/
│
├── insurance.csv
├── insurance_cost_prediction.ipynb
├── README.md
│
└── images/
    ├── eda.png
    ├── actual_vs_predicted.png
    └── residuals.png
```

*Update the filenames above if your actual repository uses different names.*

---

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/Riturajsingh07/insurance-cost-prediction.git
```

### 2. Navigate to the project directory

```bash
cd insurance-cost-prediction
```

### 3. Install required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and run the cells sequentially.

---

## 💡 Key Learnings

Through this project, I practiced:

* Data cleaning and preprocessing
* Exploratory Data Analysis
* Handling categorical variables
* Feature engineering
* Train-test splitting
* Linear Regression
* Model prediction
* MAE, RMSE, and R² evaluation
* Actual vs. predicted visualization
* Residual analysis
* Building an end-to-end Machine Learning workflow

---

## 🔮 Future Improvements

Possible improvements include:

* Compare Linear Regression with Random Forest and Gradient Boosting
* Perform feature scaling and advanced feature engineering
* Use cross-validation
* Perform hyperparameter tuning
* Build a prediction interface using Streamlit
* Deploy the model as a web application
* Add automated model evaluation

---

## 👨‍💻 Author

**Rituraj Singh Chouhan**

🎓 B.Tech Computer Science & Engineering
📍 Indore, Madhya Pradesh, India

* GitHub: [Riturajsingh07](https://github.com/Riturajsingh07)
* LinkedIn: [Rituraj Singh](https://www.linkedin.com/in/rituraj-singh-171b8a2b7)

---

## ⭐ If you found this project useful

Feel free to **star ⭐ the repository** and explore the project.
