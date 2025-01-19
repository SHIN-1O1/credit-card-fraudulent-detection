# credit-card-fraudulent-detection
## Overview

This project aims to detect fraudulent credit card transactions using machine learning techniques. It is crucial to identify fraudulent transactions effectively to prevent financial losses and ensure the security of customers' credit card information. The dataset used in this project contains anonymized credit card transaction data, with features such as transaction time, amount, and 28 principal components derived from PCA.

## Dataset

The dataset used for this project is publicly available and contains the following key features:

Time: The time in seconds elapsed between this transaction and the first transaction in the dataset.

Amount: The transaction amount.

Class: The target variable, where 1 indicates a fraudulent transaction and 0 indicates a normal transaction.

## Libraries Used

The project uses the following Python libraries:

pandas for data manipulation.

numpy for numerical computations.

matplotlib and seaborn for data visualization.

scikit-learn for machine learning algorithms.

imblearn for handling imbalanced datasets.

## Steps Performed

1. Data Loading and Exploration

Loaded the dataset using Pandas.

Explored the dataset to understand its structure, dimensions, and distribution of the Class variable.

2. Data Preprocessing

Checked for missing values and found none.

Standardized the Amount and Time columns using StandardScaler.

Split the data into fraud and normal subsets for separate analysis.

3. Data Visualization

Visualized the distribution of fraud and normal transactions using:

Scatter plots for Time vs Amount by class.

Correlation heatmaps to analyze relationships among features.

4. Handling Class Imbalance

The dataset is highly imbalanced, with fraudulent transactions accounting for a small fraction of the data.

Used techniques such as oversampling (SMOTE) and undersampling to balance the dataset.

5. Model Training

Implemented the following machine learning algorithms to detect fraudulent transactions:

Isolation Forest: Anomaly detection algorithm to identify outliers.

Local Outlier Factor (LOF): Identifies the local deviation of a data point with respect to its neighbors.

One-Class SVM: SVM-based model for anomaly detection.

6. Model Evaluation

Evaluated models using metrics such as:

Accuracy: 0.9967170750718908 %

Precision

Recall

F1-Score

Created confusion matrices to visualize the performance of models.

## Results

The models were evaluated, and the following results were observed:

Isolation Forest:

High precision in detecting fraudulent transactions.

Lower recall due to some false negatives.

Local Outlier Factor:

Balanced performance in identifying fraud and normal transactions.

One-Class SVM:

Struggled with accuracy due to dataset complexity and imbalances.

## Visualizations

Key visualizations generated during the project include:

Scatter plots showing the distribution of Time vs Amount for fraud and normal transactions.

Heatmaps illustrating the correlation between different features.

Confusion matrices for model performance evaluation.

## Tools and Environment

Python (3.12)

Jupyter Notebook/Google Colab

Anaconda for package management

##How to Run

Clone this repository.

Install the required dependencies using:

pip install -r requirements.txt

Run the Jupyter Notebook or Python script to train and evaluate models.

## Conclusion

The project successfully demonstrated the application of machine learning techniques to detect fraudulent credit card transactions. While models like Isolation Forest and LOF performed well, further optimization and additional data preprocessing can enhance their performance.

##Future Work

Explore deep learning techniques such as Autoencoders for anomaly detection.

Use additional features or external datasets to improve the model's robustness.

Deploy the model in a real-time system for live transaction monitoring.

## Acknowledgments

Special thanks to the open-source community for providing the dataset and libraries used in this project.
