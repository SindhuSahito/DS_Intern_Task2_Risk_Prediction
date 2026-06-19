# DS_Intern_Task2_Credit_Risk_Prediction

## 📌 Project Overview

This project focuses on predicting the credit risk of loan applicants using machine learning classification techniques. The objective is to determine whether an applicant is likely to default on a loan based on demographic and financial information.

The project includes:

- Data Loading and Exploration
- Missing Value Handling
- Data Visualization
- Feature Engineering
- Data Preprocessing
- Machine Learning Model Training
- Model Evaluation
- Confusion Matrix Visualization

---

## 🎯 Objective

Build and evaluate classification models to predict loan default risk using applicant information such as income, education, loan amount, marital status, and employment details.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📂 Dataset

**Dataset Used:** `test-selected-columns.csv`

### Features Included

- Loan_ID
- Gender
- Married
- Dependents
- Education
- Self_Employed
- ApplicantIncome
- CoapplicantIncome
- LoanAmount
- Loan_Amount_Term

---

## 🔍 Project Workflow

### 1️⃣ Data Loading

- Imported required Python libraries
- Loaded dataset using Pandas
- Examined dataset structure using:
  - `.shape`
  - `.columns`
  - `.head()`

### 2️⃣ Missing Value Handling

#### Categorical Features

Missing values were filled using **Mode**:

- Gender
- Married
- Dependents
- Self_Employed

#### Numerical Features

Missing values were filled using **Median**:

- LoanAmount
- Loan_Amount_Term

### 3️⃣ Exploratory Data Analysis (EDA)

Performed visual analysis to understand data distribution and trends.

#### Visualizations Created

✅ Loan Amount Distribution

✅ Applicant Income Distribution

✅ Loan Amount Distribution by Education Level

### 4️⃣ Feature Engineering

Since the dataset did not contain a target variable (`Loan_Status`), a synthetic target variable was created using a debt-to-income ratio approach.

#### Target Variable Logic

- Higher Debt-to-Income Ratio → Higher Risk
- Lower Debt-to-Income Ratio → Lower Risk

Target Classes:

- `1` = Risk / Default
- `0` = Safe

### 5️⃣ Data Preprocessing

#### Label Encoding

Applied Label Encoding on:

- Gender
- Married
- Dependents
- Education
- Self_Employed

#### Feature Scaling

Used `StandardScaler()` to improve Logistic Regression performance.

#### Train-Test Split

- Training Data: 80%
- Testing Data: 20%
- Random State: 42

---

## 🤖 Machine Learning Models

### Model 1: Logistic Regression

Used Logistic Regression as a baseline classification model.

#### Evaluation Metrics

- Accuracy Score
- Classification Report
- Confusion Matrix

### Model 2: Decision Tree Classifier

Used Decision Tree Classifier for comparison.

#### Configuration

```python
max_depth = 4
random_state = 42
```

#### Evaluation Metrics

- Accuracy Score
- Classification Report
- Confusion Matrix

---

## 📊 Model Evaluation

The following metrics were used:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Confusion Matrix Visualization

Generated heatmaps for:

- Logistic Regression
- Decision Tree Classifier

to compare prediction performance and classification errors.

---

## 📈 Key Insights

- Missing values were handled using statistical imputation techniques.
- Applicant income and loan amount distributions showed right-skewed patterns.
- Education level influenced loan amount distributions.
- Both Logistic Regression and Decision Tree models provided baseline predictive performance.
- Reducing False Negatives is important in credit risk prediction because risky applicants incorrectly classified as safe may cause financial losses.

---

## 🚀 Future Improvements

- Use a real target variable (`Loan_Status`)
- Apply One-Hot Encoding
- Perform Hyperparameter Tuning
- Implement Cross Validation
- Test advanced models:
  - Random Forest
  - XGBoost
  - Gradient Boosting
- Handle class imbalance using SMOTE

---

## ▶️ How to Run

### Clone Repository

```bash
git clone https://github.com/your-username/DS_Intern_Task2_Credit_Risk_Prediction.git
```

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

### Run

Open the notebook and execute all cells sequentially.

---

## 📌 Internship Task

**Task 2: Credit Risk Prediction**

Developed as part of a Data Science / Data Analytics Internship to demonstrate:

- Data Cleaning
- Data Visualization
- Feature Engineering
- Classification Modeling
- Model Evaluation

---

## 👨‍💻 Author

**Sindhu**

Data Science & Data Analytics Enthusiast
