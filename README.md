# Employee Attrition and Department Prediction

This project aims to develop a neural network model that predicts whether employees are likely to leave the company (attrition) and identifies the department that best fits each employee. The model uses a branched neural network architecture to predict these two outcomes simultaneously.

## Table of Contents
- [Background](#background)
- [Dataset](#dataset)
- [Preprocessing](#preprocessing)
- [Model Architecture](#model-architecture)
- [Training the Model](#training-the-model)
- [Evaluation](#evaluation)
- [Improvements](#improvements)
- [Sources](#Sources)

## Background
Human Resources (HR) departments can benefit from predictive models that help in understanding employee attrition and suitability for various departments. Such models can assist in proactive measures to retain talent and optimize employee placement.

## Dataset
The dataset used in this project contains information about employees, including demographics, job satisfaction, performance ratings, and more. The dataset can be found [here](https://static.bc-edx.com/ai/ail-v-1-0/m19/lms/datasets/attrition.csv).

## Preprocessing
Preprocessing steps include:
1. Importing necessary libraries.
2. Reading the dataset.
3. Creating target variables (`Attrition` and `Department`).
4. Selecting relevant features for the model.
5. Encoding categorical variables using one-hot encoding.
6. Standardizing numeric features.
7. Splitting the dataset into training and testing sets.

## Model Architecture
The model uses a branched neural network architecture:
- Shared layers: Two hidden layers shared by both branches.
- Department branch: A hidden layer followed by an output layer with softmax activation.
- Attrition branch: A hidden layer followed by an output layer with softmax activation.

## Training the Model
The model is compiled using the Adam optimizer, with categorical cross-entropy loss for the department branch and binary cross-entropy loss for the attrition branch. The model is trained for 50 epochs with a batch size of 32.

## Evaluation
The model's performance is evaluated using accuracy metrics for both department prediction and attrition prediction.

## Improvements
Several potential improvements include:
- Feature engineering and selection.
- Hyperparameter tuning.
- Regularization techniques.
- Data augmentation for imbalanced classes.
- Cross-validation.
- Ensemble methods.
- Advanced neural network architectures.
- Transfer learning.
- Improved data quality and handling.

## Sources
- Tutors
- Google Colab
- Chat GPT
- Classmates