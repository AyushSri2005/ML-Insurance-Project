# Insurance Data Analysis & Feature Engineering

> Exploratory data analysis and feature engineering on medical insurance data to understand the factors associated with insurance charges.

## 📌 Overview

This project explores a medical insurance dataset to understand how demographic, lifestyle, and health-related factors are associated with insurance charges.

Rather than jumping directly into model training, the project focuses on building a strong understanding of the data first — including data cleaning, exploratory analysis, feature engineering, scaling, correlation analysis, and statistical feature selection.

The notebook follows a practical data science workflow and prepares the dataset for a future machine learning prediction stage.

---

## 🎯 Objectives

- Understand the structure and distribution of the insurance dataset
- Identify patterns and relationships between features and insurance charges
- Clean and prepare the data for analysis
- Convert categorical variables into numerical representations
- Create meaningful features from existing data
- Analyze feature relationships using statistical techniques
- Identify features that may be useful for future predictive modeling

---

## 📊 Dataset

The dataset contains **1,338 records** and the following 7 original features:

| Feature | Description |
|---|---|
| `age` | Age of the individual |
| `sex` | Gender |
| `bmi` | Body Mass Index |
| `children` | Number of children/dependents |
| `smoker` | Smoking status |
| `region` | Residential region |
| `charges` | Medical insurance charges |

### Target

`charges` represents the medical insurance cost associated with each individual.

---

## 🔍 What I Did

### 1. Data Exploration

The dataset was initially explored to understand:

- Shape and structure
- Data types
- Statistical summary
- Feature distributions
- Categorical value counts
- Missing values
- Duplicate records

The dataset contains no missing values. One duplicate record was identified and removed, leaving **1,337 records** for further analysis.

### 2. Data Cleaning

The preprocessing stage includes:

- Removing duplicate records
- Converting categorical variables into numerical representations
- Preparing the dataset for statistical analysis
- Maintaining a clean and consistent feature structure

### 3. Feature Engineering

Additional features were created to capture useful information from the original data.

#### BMI Categories

BMI was divided into four categories:

- Underweight
- Normal
- Overweight
- Obese

The categorical BMI feature was then transformed using one-hot encoding.

### 4. Feature Scaling

Standardization was applied to numerical features such as:

- `age`
- `bmi`
- `children`

This brings the numerical features onto a comparable scale and prepares them for downstream machine learning algorithms.

### 5. Correlation Analysis

Pearson correlation was used to examine the relationship between individual features and insurance charges.

In the analysis, `is_smoker` showed the strongest positive Pearson correlation with `charges`, followed by `age` and BMI-related features.

This provides an initial indication of which variables may be particularly useful for further analysis.

### 6. Statistical Feature Selection

Chi-square tests were also applied to categorical features to examine their relationship with binned insurance charges.

This analysis was used to identify categorical variables that may provide useful information for future predictive modeling.

---

## 📈 Key Findings

Some of the main observations from the analysis include:

- Smoking status has a strong relationship with insurance charges in this dataset.
- Age shows a positive relationship with insurance charges.
- BMI-related features also show measurable associations with charges.
- Some regional and categorical features show weaker statistical relationships.
- Feature engineering can provide additional information beyond the original raw variables.

These findings are based on exploratory and statistical analysis of this dataset and should not be interpreted as causal relationships.

---

## 🛠️ Tech Stack

### Programming Language
- Python

### Data Analysis
- Pandas
- NumPy

### Visualization
- Matplotlib
- Seaborn

### Statistical Analysis
- SciPy

### Development
- Jupyter Notebook
- Visual Studio Code

### Version Control
- Git
- GitHub

---

## 🔄 Project Workflow

```text
Raw Dataset
     ↓
Data Understanding
     ↓
Data Cleaning
     ↓
Exploratory Data Analysis
     ↓
Categorical Encoding
     ↓
Feature Engineering
     ↓
Feature Scaling
     ↓
Correlation Analysis
     ↓
Statistical Feature Selection
     ↓
Prepared Dataset
