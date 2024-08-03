# Universal Bank Prediction

## Project Description

This project involves building a machine learning model to predict whether customers of Universal Bank will accept a personal loan or not. The dataset contains various attributes of the customers such as age, income, education level, and more.

## Dataset Description

The dataset `UniversalBank.csv` includes the following features:

- **ID**: Customer ID
- **Age**: Customer's age
- **Experience**: Number of years of professional experience
- **Income**: Annual income of the customer (in thousands)
- **ZIP Code**: Customer's residential ZIP code
- **Family**: Size of the customer's family
- **CCAvg**: Average spending on credit cards per month (in thousands)
- **Education**: Education level (1: Undergrad, 2: Graduate, 3: Advanced/Professional)
- **Mortgage**: Value of the mortgage (if any)
- **Personal Loan**: Indicator if the customer accepted a personal loan (1: Yes, 0: No)
- **Securities Account**: Indicator if the customer has a securities account with the bank (1: Yes, 0: No)
- **CD Account**: Indicator if the customer has a certificate of deposit account (1: Yes, 0: No)
- **Online**: Indicator if the customer uses internet banking facilities (1: Yes, 0: No)
- **CreditCard**: Indicator if the customer uses a credit card issued by UniversalBank (1: Yes, 0: No)

## Requirements

To run the notebook, you need to install the following Python packages:

- pandas
- numpy
- scikit-learn
- imbalanced-learn

You can install these packages using pip:

\`\`\`bash
pip install pandas numpy scikit-learn imbalanced-learn
\`\`\`

## Usage

1. Clone the repository.
2. Open the Jupyter Notebook `Universal_bank_prediction.ipynb`.
3. Follow the steps in the notebook to preprocess the data, train the model, and evaluate its performance.

## Code Explanation

### 1. Data Loading and Preprocessing

- **Load the dataset** using pandas.
- **Drop irrelevant columns** (`ID` and `ZIP Code`).
- **Separate the features** (`X`) and the target variable (`y`).

### 2. Data Splitting

- **Split the data** into training and testing sets using `train_test_split`.

### 3. Data Balancing

- **Use SMOTE** (Synthetic Minority Over-sampling Technique) to balance the classes in the training set.

### 4. Feature Scaling

- **Standardize the features** using `StandardScaler`.

### 5. Model Training and Evaluation

- **Train a Support Vector Machine (SVM) classifier**.
- **Evaluate the model** using accuracy score, classification report, and confusion matrix.
