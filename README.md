# titanic-survival-prediction


This repository contains an exercise from Kaggle focused on predicting the survival of passengers aboard the Titanic. The goal of this exercise is to build basic machine learning models to predict whether or not a passenger survived based on various attributes, such as their age, sex, passenger class, where they embarked, and more.

## Objective

The objective of this project is to develop a model that can predict the survival of Titanic passengers using a range of features. The key attributes used in this prediction include:

- **Age**: The age of the passenger.
- **Sex**: The gender of the passenger.
- **Passenger Class**: The class of travel (1st, 2nd, 3rd).
- **Embarked**: The port where the passenger boarded the Titanic.
- **Fare**: The fare paid by the passenger.
- **Siblings/Spouses Aboard**: The number of siblings or spouses traveling with the passenger.
- **Parents/Children Aboard**: The number of parents or children traveling with the passenger.
- And other relevant attributes.

## Dataset

The dataset used in this project is the **Titanic: Machine Learning from Disaster** dataset available on Kaggle. It contains two primary CSV files:

1. **train.csv**: The training data, which includes the passenger information along with their survival status (0 for did not survive, 1 for survived).
2. **test.csv**: The test data, which includes passenger information without survival labels, used for making predictions.

Additionally, any data files or outputs generated during the process are stored in the `dataset` folder.

## Model Approach

In this project, basic machine learning models such as **Random Forest Classifier**, and **Support Vector Classifier (SVC)** were implemented. The process includes:

- **Data Preprocessing**: Handling missing values, converting categorical variables into numerical ones (using One-Hot Encoding), and scaling numerical features.
- **Model Training**: Using different machine learning models to predict survival.
- **Model Evaluation**: Using cross-validation to assess model performance and tuning hyperparameters for optimal results.


## Results

The models were evaluated using **cross-validation** with a 10-fold split to assess the performance of each model. The following machine learning models were tested:

- **Random Forest Classifier**
- **Support Vector Classifier (SVC)**

After evaluating the models, the following observations were made:

- **Random Forest Classifier** achieved a very high score on one of the 10 folds, but its overall mean score was lower than that of the **SVM Classifier**, with a larger spread in scores across the folds. This suggests that while the Random Forest model can perform well under certain conditions, it may be less consistent and is more prone to overfitting on specific folds.
  
- **Support Vector Classifier (SVC)** showed a more stable performance across all folds, resulting in a higher mean score and less variation in the results. This suggests that the SVM model is more likely to generalize well to new, unseen data.


## License

This project is for educational purposes as part of a Kaggle exercise. Feel free to use or modify the code for learning and personal use.