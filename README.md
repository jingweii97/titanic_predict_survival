# Titanic Survival Prediction
This repository contains my approach to the Titanic: Machine Learning from Disaster challenge on Kaggle. The goal of this project is to predict passenger survival using machine learning techniques.

Outcome: Scored 0.78468 at kaggle competition, which ranks ~top 10%.

## Project Overview

The Titanic dataset provides information on passengers, such as age, gender, ticket class, and other relevant features. The objective is to train a model that accurately predicts whether a passenger survived or not.

## Dataset
Train Data: InData/train.csv (Used for model training and validation)  
Test Data: InData/test.csv (Unknown data for final predictions)

## Workflow
Overview of the workflow is shown in the following:

1. Data Collection and Loading:  
  Import and read train and test data from Kaggle.

3. Exploratory Data Analysis (EDA):  
  - EDA Part I: To analyze the overall data structure and characteristics of the available feature, in order to have a basic understanding of the provided data.
  - EDA Part II: Based on the outcome of EDA Part I, selected relevant features will be analyzed to understand the correlation between features and target.
     
4. Data Preprocessing:  
  - Feature Engineering: Feature Creation (create new feature highlighting the relevant features), Feature Selection (select only relevant features) and Feature Transformation (handle missing data, scaling and encoding)
  - Building Pipeline: To automate and bundle the process of feature engineering and modelling, to reuse in later stage for test data set.
    
5. Model Evaluation:  
  - Various metrics have been used as evaluation basis, e.g. confusion matrix, classification matric, ROC-AUC, log-loss etc.
  - Tested with various model, starting with base model using Logistic Regression, and eventually Random Forest. Hyperparameter tuning has been performed using GridSearchCV.

6. Test Data Prediction:
  - With the fine-tuned model, prediction is made for test data and exported to destination.
    
7. First Test Data Submission Review:
  - Submission results showed that the model scored 0.78468 (~top 10%).



## Repository Structure

```
|-- InData/               # Contains the dataset files
|-- OutData/              # Destination folder for prediction result
|-- TitanicMachineLearning_score_78468_final            # Jupyter notebook for analysis & modeling
|-- archive/              # Archived jupyter notebook
|-- README.md             # Project documentation
```

## Future Improvements

- Exploring other feature engineering techniques.
- Trying different ensemble methods to improve performance.

## Acknowledgments

This project is based on Kaggle's Titanic competition dataset. Special thanks to the Kaggle community for their insights and contributions.

---

Feel free to contribute or suggest improvements!

