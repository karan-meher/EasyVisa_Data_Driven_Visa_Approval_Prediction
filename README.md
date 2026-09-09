# EasyVisa — Data-Driven Visa Approval Prediction

## 📌 Project Overview

The **EasyVisa** project uses machine learning to predict whether a visa application is likely to be **Certified** or **Denied** based on applicant and employer-related information.

The project follows a complete data science and machine learning workflow, including:

* Data exploration and cleaning
* Exploratory Data Analysis (EDA)
* Feature engineering and encoding
* Train/validation/test splitting
* Handling class imbalance
* Comparison of multiple classification algorithms
* Hyperparameter tuning
* Model evaluation using classification metrics
* Feature importance analysis
* Business insights and recommendations

The goal is to identify the factors that have the greatest influence on visa certification and build a machine learning model that can assist in predicting visa application outcomes.

---

## 🎯 Objective

* Predict visa application status: **Certified / Denied**
* Identify the important factors influencing visa approval
* Compare different machine learning classification models
* Select the best-performing model for prediction

## 📊 Dataset

The dataset contains **25,480 visa application records** and **12 columns**.

## Dataset Features

| Feature                 | Description                                      |
| ----------------------- | ------------------------------------------------ |
| `case_id`               | Unique identifier for each visa application      |
| `continent`             | Continent of the applicant                       |
| `education_of_employee` | Education level of the employee                  |
| `has_job_experience`    | Whether the employee has previous job experience |
| `requires_job_training` | Whether the employee requires job training       |
| `no_of_employees`       | Number of employees in the organization          |
| `yr_of_estab`           | Year in which the organization was established   |
| `region_of_employment`  | Region where the employee will work              |
| `prevailing_wage`       | Prevailing wage offered to the employee          |
| `unit_of_wage`          | Wage unit such as Year, Hour, Week, or Month     |
| `full_time_position`    | Whether the position is full-time                |
| `case_status`           | Target variable: `Certified` or `Denied`         |


**Target Variable:** `case_status`

* **Certified**
* **Denied**

## 🤖 Machine Learning Models

The following models were evaluated:

* Random Forest
* Gradient Boosting
* AdaBoost
* XGBoost
* Decision Tree
* Bagging Classifier

**Gradient Boosting** was selected as the final model after model comparison and hyperparameter tuning.

## 📈 Model Performance

The final Gradient Boosting model achieved the following results on the test dataset:

| Metric    |      Score |
| --------- | ---------: |
| Accuracy  | **75.16%** |
| Precision | **78.61%** |
| Recall    | **86.30%** |
| F1 Score  | **82.28%** |

## 🔍 Key Insights

The analysis identified the following as important factors in visa approval:

* **Education of the employee**
* **Region of employment**
* **Prevailing wage**

Higher education levels, relevant job experience, and other applicant/employer characteristics showed meaningful relationships with visa certification.

## 🧰 Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Imbalanced-learn**
* **XGBoost**
* **Jupyter Notebook**

## 📁 Project Files

```text
EasyVisa/
├── EasyVisa.csv
├── EasyVisa_Data_Driven_Visa_Approval_Prediction.ipynb
└── README.md
```

## 📌 Conclusion

This project demonstrates an end-to-end machine learning approach for predicting visa application outcomes.

After performing data cleaning, exploratory analysis, class balancing, model comparison, and hyperparameter tuning, the **Gradient Boosting Classifier trained on oversampled data** was selected as the final model.

The final model achieved:

**82.28% F1 Score on the unseen test dataset**

The analysis also highlighted **employee education, region of employment, and prevailing wage** as important predictive features.

Overall, the project demonstrates how machine learning can be used to uncover patterns in visa application data and support data-driven analysis of visa certification outcomes.
