# Credit Card Fraud Detection

This repository contains an analysis and implementation of credit card fraud detection using machine learning techniques. The dataset used is from a Kaggle competition and includes transactions made by credit cards in September 2013 by European cardholders.

## Dataset

The dataset contains transactions made over two days, where we have 492 frauds out of 284,807 transactions. The features include transaction time, amount, and 28 principal components obtained with PCA (due to confidentiality issues, the original features and more background information are not provided).

## Project Structure

- **data**: Contains the dataset `creditcard.csv`.
- **notebooks**: Jupyter notebooks for data exploration, preprocessing, and modeling.
- **README.md**: This file, providing an overview of the project.

## Libraries Used

- Python 3.8.8
- NumPy 1.20.1
- Pandas 1.2.4
- Matplotlib 3.3.4
- Seaborn 0.11.1
- Scipy 1.6.2
- Scikit-learn (Sklearn) 0.24.1

## Analysis and Modeling

1. **Data Exploration**: Investigated the distribution of transactions and explored patterns in fraud vs. valid transactions.
2. **Preprocessing**: Handled data imbalance, scaled features, and prepared data for modeling.
3. **Modeling**:
   - Implemented Isolation Forest, Local Outlier Factor, and One-Class SVM for anomaly detection.
   - Evaluated models based on accuracy scores and classification reports.
   
## Results

- Isolation Forest achieved an accuracy of 99.75% with 71 errors in predicting fraud cases.
- Local Outlier Factor achieved an accuracy of 99.66% with 97 errors.
- Support Vector Machine (One-Class SVM) achieved an accuracy of 70.10% with 8515 errors.

## Conclusion

Different models were implemented for detecting credit card fraud, with Isolation Forest showing the best performance in terms of accuracy and precision for fraud detection.

For detailed code and analysis, please refer to the Jupyter notebooks provided in the `notebooks` directory.
