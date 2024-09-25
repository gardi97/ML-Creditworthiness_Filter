# Credit Reliability Classifier

## Introduction
This project aims to create a classifier capable of predicting the credit reliability of potential clients based on historical application and credit data. Various machine learning models were evaluated to select the most appropriate one for this task.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Data Analysis](#data-analysis)
- [Models](#models)
- [Evaluation](#evaluation)
- [Conclusions](#conclusions)



## Installation
To run this project, you will need the following libraries:

```bash
pip install pandas numpy scikit-learn seaborn matplotlib
```

You may also need to configure access to the dataset files, which are expected to be named `application_record.csv` and `credit_record.csv`.

## Usage
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/credit-reliability-classifier.git
    ```
2. Place the dataset files (`application_record.csv` and `credit_record.csv`) in the correct directory.
3. Run the Jupyter notebook to train and evaluate the models:
    ```bash
    jupyter notebook Progetto_Affidabilità_Creditizia_v3.ipynb
    ```

## Features
- Data preprocessing of client application and credit record data.
- Implementation of various machine learning models:
  - Support Vector Machine (SVM)
  - K-Nearest Neighbors (KNN)
  - Naive Bayes (ComplementNB)
- Comparison of model performance using precision, recall, and F1-score.
- Visualizations: Confusion matrices, Precision-Recall curves.

## Data Analysis
The dataset consists of two files:
- `application_record.csv`: Contains 438,557 client application records.
- `credit_record.csv`: Contains the monthly credit status of clients.

Key variables:
- **Status**: Credit status can take values like C (regular payments), 0 (minor delay), etc.
- **Target**: Classification of credit reliability based on client history.

## Models
Multiple models were trained and compared:
- **Support Vector Machines**: Gaussian and polynomial kernels were tested with and without oversampling.
- **K-Nearest Neighbors (KNN)**: Optimized using different numbers of neighbors.
- **Naive Bayes**: ComplementNB was selected for the task.

## Evaluation
The models were evaluated based on precision, recall, and F1-score. The best-performing models were:
- SVM with Gaussian kernel
- KNN with optimized hyperparameters

## Conclusions
Despite the numerous models evaluated, it was not possible to identify a satisfactory one 

## Contributors
- [Francesco Gardini](https://github.com/gardi97)
