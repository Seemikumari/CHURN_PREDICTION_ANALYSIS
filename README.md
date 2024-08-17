# 📊 Churn Prediction Analysis

## 📝 Overview

The project focuses on predicting customer churn for a bank using a dataset containing various customer attributes. The analysis encompasses data exploration, preprocessing, and splitting into training and testing sets to develop predictive models.

## 🛠️ Tools and Steps

**Tools:** 🐍 Python, 📊 Pandas, 📈 Matplotlib, 📊 Seaborn, 📊 scikit-learn.

**Steps:**
- 📈 Descriptive Statistics on the Dataset
- 📊 Data Preprocessing
- 📊 Data Splitting into Train and Test Sets
- 📊 Data Exploration
- 📝 Data Storing

## 📈 Descriptive Statistics on the Dataset

The initial dataset was loaded and irrelevant columns were dropped, resulting in a dataset with customer attributes relevant to predicting churn. The dataset consists of 10,000 rows and 11 columns.

## 📊 Data Preprocessing

### Handling Missing Values
There were no missing values in the dataset.

### Feature Engineering
- Gender was converted to binary variables.
- Geography was converted to dummy variables.
- A new feature 'ZeroBalance' was created to identify customers with zero balance.

### Scaling
StandardScaler was used to standardize predictor variables.

## 📊 Data Splitting into Train and Test Sets

### Random Sampling
The dataset was initially split into training and test sets using random sampling, resulting in uneven distribution of churn levels between the sets.

### Stratified Sampling
StratifiedShuffleSplit was used to split the data into more representative training and test sets based on churn levels.

## 📊 Data Exploration

### Churn Distribution
Only approximately 20% of customers in the dataset have churned.

### Geographic and Demographic Insights
- Most customers are from France.
- Germans seem more likely to churn.
- Gender frequencies are relatively even, with females leaving slightly more.
- The majority of customers have a credit card.
- The dataset is evenly split between active and non-active members, with active members being less likely to churn.

### Visualizations
- Bar plots were used to visualize churn distribution by geography, gender, and credit card ownership.
- Histograms were used to visualize the distribution of numerical features.

## 📝 Data Storing

The preprocessed datasets were saved as CSV files:
- `Xtrain.csv`
- `Xtest.csv`
- `ytrain.csv`
- `ytest.csv`

## 📝 Conclusion

The initial data exploration and preprocessing steps have set the foundation for developing predictive models to identify customers at risk of churn. The data has been split into training and test sets, and necessary preprocessing steps, including feature engineering and scaling, have been performed to prepare the data for modeling.
