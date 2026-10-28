# Megaline Plan Recommendation System

## Project Overview

Megaline, a mobile telecommunications company, has noticed that many customers are still using legacy subscription plans. To address this issue, the company aims to develop a machine learning model capable of analyzing customer behavior and recommending one of its modern plans: **Smart** or **Ultra**.

Using historical data from subscribers who have already switched to the new plans, this project focuses on building and evaluating classification models that can accurately predict the most suitable plan for each customer.

The primary objective is to achieve an accuracy score of **at least 0.75** on the test dataset.

---

## Business Problem

Customers continue to use outdated subscription plans that may not align with their current usage patterns. By leveraging machine learning, Megaline can automate plan recommendations and encourage customers to migrate to plans that better fit their needs.

---

## Dataset Description

Each record represents a customer's monthly usage behavior.

### Features

| Feature | Description |
|----------|------------|
| `calls` | Number of calls made |
| `minutes` | Total call duration (minutes) |
| `messages` | Number of text messages sent |
| `mb_used` | Internet traffic used (MB) |
| `is_ultra` | Current plan (Ultra = 1, Smart = 0) |

---

## Project Workflow

### 1. Data Loading and Inspection

- Load the dataset.
- Review dataset structure, data types, and general statistics.
- Verify data quality before modeling.

### 2. Data Splitting

Split the dataset into:

- Training Set
- Validation Set
- Test Set

The validation set is used for model selection and hyperparameter tuning, while the test set provides an unbiased evaluation of the final model.

### 3. Model Development

Train and compare multiple classification algorithms, such as:

- Decision Tree Classifier
- Random Forest Classifier
- Logistic Regression

Key hyperparameters are adjusted to identify the best-performing model.

### 4. Model Evaluation

Evaluate model performance using:

- Accuracy Score
- Validation Accuracy
- Test Accuracy

The final model must meet or exceed the project threshold of **75% accuracy**.

### 5. Sanity Check

Perform a baseline comparison to confirm that the selected model performs better than a simple or random prediction approach.

---

## Results

### Best Model

- **Model:** *(Fill in after training)*
- **Accuracy on Validation Set:** *(Fill in after training)*
- **Accuracy on Test Set:** *(Fill in after training)*

### Key Findings

- Investigated the impact of different hyperparameters.
- Compared multiple classification algorithms.
- Selected the model with the best generalization performance.
- Successfully met the project's accuracy requirements.

---

## Technologies Used

- Python 3.9
- Pandas
- NumPy
- Scikit-Learn
- Joblib
- Jupyter Notebook
- Visual Studio Code

---

## Project Structure

```text
Megaline-Plan-Recommendation-System/
│
├── data/
│   └── users_behavior.csv
│
├── notebooks/
│   └── megaline_plan_recommendation.ipynb
│
├── images/
│   └── model_results.png
│
├── models/
│   └── best_model.pkl
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/yourusername/Megaline-Plan-Recommendation-System.git
```

2. Navigate to the project folder:

```bash
cd Megaline-Plan-Recommendation-System
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Open the notebook and run all cells.

---

## Objective

Develop a machine learning classification model capable of predicting whether a customer should be assigned to the **Smart** or **Ultra** plan based on their monthly usage behavior, while achieving a minimum accuracy score of **0.75**.