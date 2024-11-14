
# **Credit Card Fraud Detection**

## **Project Overview**
This project predicts fraudulent credit card transactions using machine learning models. The dataset, taken from Kaggle, contains 2,84,807 transactions, with only 492 fraudulent ones, which makes this a **highly imbalanced dataset**. The goal is to use machine learning techniques to detect fraudulent transactions effectively and efficiently.

## **Problem Statement**
Credit card fraud detection has become a critical issue in the banking sector. With the rise in online transactions, fraud is a major concern that causes financial losses and undermines trust in digital payments. In this project, we predict fraudulent transactions using machine learning models.

## **Business Problem Overview**
Many banks aim to retain high-value customers, but fraud poses a significant threat. Fraudulent transactions result in financial losses and damage to trust and credibility. It is estimated that by 2020, banking fraud would account for $30 billion worldwide. Machine learning techniques can help financial institutions monitor and prevent fraud effectively.

## **Understanding and Defining Fraud**
Credit card fraud includes any dishonest activity to obtain unauthorized information for financial gain. Common fraud methods include:
- **Skimming**: Copying data from the card’s magnetic strip.
- **Manipulation**: Altering genuine cards.
- **Counterfeit Cards**: Creating fake cards.
- **Stolen/Lost Cards**: Unauthorized use of lost or stolen cards.
- **Fraudulent Telemarketing**: Scams that involve fraudulent calls asking for card details.

## **Dataset Description**
The dataset consists of credit card transactions made by European cardholders over two days in September 2013. Out of 2,84,807 transactions, only 492 are fraudulent. The dataset includes:
- **Time**: Time elapsed between the first transaction and subsequent ones.
- **Amount**: Transaction amount.
- **V1 to V28**: Features derived using Principal Component Analysis (PCA) for confidentiality.
- **Class**: The target variable (1 for fraud, 0 for non-fraud).

> **Note**: The dataset is highly imbalanced, with fraudulent transactions making up only 0.172% of all transactions.

## **Project Pipeline**
The project pipeline is divided into four main stages:

1. **Data Understanding**:
   - Load and explore the dataset.
   - Examine the features and identify the relevant ones for model building.

2. **Exploratory Data Analysis (EDA)**:
   - Perform univariate and bivariate analysis.
   - Check for skewness or data imbalances and address them if necessary.

3. **Train/Test Split**:
   - Split the data into training and testing datasets.
   - Apply stratified sampling to preserve the distribution of fraudulent transactions.

4. **Model Building and Hyperparameter Tuning**:
   - Train multiple machine learning models like Logistic Regression, Random Forest, and SVC.
   - Apply **SMOTE** (Synthetic Minority Over-sampling Technique) to handle class imbalance.
   - Fine-tune hyperparameters to improve model performance.

5. **Model Evaluation**:
   - Evaluate the models using precision, recall, F1-score, and ROC-AUC score.
   - Emphasize the detection of fraudulent transactions (positive class).

## **Technologies Used**
- **Python** (3.x)
- **Libraries**: pandas, numpy, scikit-learn, imbalanced-learn, matplotlib, seaborn, joblib
