# Titanic Dataset - Data Cleaning & Preprocessing

This repository contains a step-by-step implementation of data cleaning and preprocessing techniques on the *Titanic dataset* using Python. The goal is to prepare the raw data for machine learning models.

---

##  Objective

To explore and clean the Titanic dataset by:
- Handling missing data
- Encoding categorical features
- Scaling numerical features
- Detecting and removing outliers
- Visualizing distributions

---

## Tools & Libraries Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn

---

##  Dataset Overview

The dataset includes the following features:

| Column       | Description                         |
|--------------|-------------------------------------|
| PassengerId  | Unique ID for each passenger        |
| Survived     | Survival (0 = No, 1 = Yes)          |
| Pclass       | Ticket class (1, 2, 3)              |
| Name         | Passenger name                      |
| Sex          | Gender                              |
| Age          | Age in years                        |
| SibSp        | # of siblings/spouses aboard        |
| Parch        | # of parents/children aboard        |
| Ticket       | Ticket number                       |
| Fare         | Fare paid for the ticket            |
| Cabin        | Cabin number (many missing)         |
| Embarked     | Port of embarkation (C, Q, S)       |

---

##  Data Preprocessing Steps

1. *Missing Value Handling*
   - Age: Filled with median
   - Embarked: Filled with mode
   - Cabin: Dropped due to many nulls

2. *Encoding Categorical Data*
   - Sex: Label encoded (male = 0, female = 1)
   - Embarked: One-hot encoded

3. *Feature Scaling*
   - Age and Fare: Standardized using StandardScaler

4. *Outlier Removal*
   - Detected and removed outliers in Fare using the IQR method

5. *Visualization*
   - Used boxplots to identify outliers
   - Used distribution plots to understand feature spread

---

##  Results

After preprocessing:
- The dataset is clean, structured, and ready for modeling.
- No missing values.
- All features are in appropriate formats.

---

##  How to Run

1. Clone the repository:
   ```bash
   https://github.com/priya-72706/Data-Cleaning-Preprocessing
   cd titanic-preprocessing
