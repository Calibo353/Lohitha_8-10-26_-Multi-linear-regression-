# Advertising Sales Prediction using Multiple Linear Regression

## 📌 Overview

This project focuses on predicting **product sales based on advertising expenditure** across three different channels: **TV, Radio, and Newspaper**.

The project uses **Multiple Linear Regression** to understand the relationship between advertising spending and sales, evaluate the model's performance, and predict sales for a new advertising budget.

---

## 🎯 Problem Statement

A company invests money in different advertising channels to increase product sales. However, it needs to understand which advertising channels have a stronger relationship with sales.

The objective of this project is to:

- Analyze advertising expenditure across different channels.
- Understand the relationship between advertising spending and sales.
- Build a Multiple Linear Regression model.
- Evaluate the model's performance.
- Predict sales based on a new advertising budget.
- Interpret the model coefficients from a business perspective.

---

## 🎯 Objectives

- Load and inspect the advertising dataset.
- Perform basic data analysis.
- Identify independent and dependent variables.
- Split the dataset into training and testing data.
- Build a Multiple Linear Regression model.
- Train the model using the training dataset.
- Predict sales for the test dataset.
- Evaluate the model using regression metrics.
- Predict sales for a new advertising budget.
- Interpret the model coefficients.

---

## 📊 Dataset

The dataset contains advertising expenditure and corresponding product sales.

### Features

| Feature | Description |
|---|---|
| TV | Advertising expenditure on TV |
| Radio | Advertising expenditure on Radio |
| Newspaper | Advertising expenditure on Newspaper |

### Target Variable

| Target | Description |
|---|---|
| Sales | Product sales |

The independent variables used for prediction are:

```text
TV
Radio
Newspaper
```

The dependent variable is:

```text
Sales
```

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Scikit-learn**
- **Jupyter Notebook**

---

## 🔄 Methodology

### 1. Import Libraries

The required Python libraries were imported for data manipulation, visualization, model building, and evaluation.

### 2. Load the Dataset

The advertising dataset was loaded using Pandas and its structure was inspected.

### 3. Select Features and Target

The independent variables were:

```text
TV
Radio
Newspaper
```

The target variable was:

```text
Sales
```

### 4. Split the Dataset

The dataset was divided into:

- Training data
- Testing data

using `train_test_split()` from Scikit-learn.

### 5. Build the Model

A **Multiple Linear Regression** model was created using `LinearRegression()`.

The mathematical equation is:

```text
Sales = β₀ + β₁(TV) + β₂(Radio) + β₃(Newspaper)
```

Where:

- `β₀` = Intercept
- `β₁` = TV coefficient
- `β₂` = Radio coefficient
- `β₃` = Newspaper coefficient

### 6. Train the Model

The model was trained using the training dataset.

### 7. Make Predictions

The trained model was used to predict sales values for the testing dataset.

### 8. Evaluate the Model

The following evaluation metrics were used:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## 📈 Model Coefficients

The trained model produced the following coefficients:

| Parameter | Coefficient |
|---|---:|
| Intercept | 4.7141 |
| TV | 0.0545 |
| Radio | 0.1009 |
| Newspaper | 0.0043 |

The resulting model can be represented approximately as:

```text
Sales = 4.7141 + (0.0545 × TV) + (0.1009 × Radio) + (0.0043 × Newspaper)
```

### Interpretation

- **TV:** A positive coefficient indicates that higher TV advertising expenditure is associated with higher predicted sales, while keeping the other variables constant.
- **Radio:** Radio has the largest coefficient among the three advertising channels in this model.
- **Newspaper:** Newspaper has a much smaller coefficient compared with TV and Radio.

> **Note:** Coefficients indicate the model's estimated relationship with sales. They should not automatically be interpreted as proof of causation.

---

## 📊 Model Performance

The model achieved the following evaluation result:

| Metric | Value |
|---|---:|
| MAE | 1.2748 |

### Mean Absolute Error (MAE)

MAE represents the average absolute difference between the actual sales values and the predicted sales values.

A lower MAE indicates that the predictions are, on average, closer to the actual values.

The project also evaluates the model using:

- **MSE** – Measures the average squared prediction error.
- **RMSE** – Represents the square root of MSE and expresses the error in the same units as the target.
- **R² Score** – Measures how well the model explains the variation in sales.

---

## 🔮 Sales Prediction

After training the model, it can be used to predict sales for a new advertising budget.

For example, a new set of advertising values can be provided for:

```text
TV
Radio
Newspaper
```

The trained model then generates the corresponding predicted sales value.

This demonstrates how Multiple Linear Regression can be used for **sales forecasting based on advertising investment**.

---

## 💡 Business Insights

The project provides the following insights:

1. Advertising expenditure has a measurable relationship with predicted sales.
2. Radio has the largest estimated coefficient among the three advertising channels in this model.
3. TV also shows a positive relationship with predicted sales.
4. Newspaper has a relatively small coefficient compared with TV and Radio.
5. The model can be used as a supporting tool when analyzing advertising budget allocation.
6. Model evaluation metrics help determine how accurately the model predicts sales.

---

## 📁 Project Structure

```text
Advertising-Sales-Prediction/
│
├── Advertising.csv
├── Advertising_Sales_Prediction.ipynb
├── README.md
└── requirements.txt
```

---

## 🚀 How to Run the Project

### Step 1: Clone the Repository

```bash
git clone <your-repository-url>
```

### Step 2: Navigate to the Project Folder

```bash
cd Advertising-Sales-Prediction
```

### Step 3: Install Required Libraries

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

### Step 4: Open Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the Notebook

Open:

```text
Advertising_Sales_Prediction.ipynb
```

and execute the cells step by step.

---

## ✅ Conclusion

This project demonstrates how **Multiple Linear Regression** can be used to predict product sales based on advertising expenditure across TV, Radio, and Newspaper.

The project covers the complete machine learning workflow, including:

```text
Data Loading
     ↓
Data Inspection
     ↓
Feature Selection
     ↓
Train-Test Split
     ↓
Model Training
     ↓
Prediction
     ↓
Model Evaluation
     ↓
Business Interpretation
```

Overall, the project provides practical experience in applying **Multiple Linear Regression to a real-world business prediction problem** and interpreting machine learning results from a business perspective.

---

## 👩‍💻 Author

**Manda Lohitha**

B.Tech – Computer Science and Engineering
