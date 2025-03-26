# Titanic Survival Prediction

Project Overview: This project aims to develop a machine learning model to predict whether a passenger survived the Titanic disaster. The dataset includes various features such as age, gender, ticket class, fare, cabin information, and more. The goal is to preprocess the data effectively and build a classification model to achieve high prediction accuracy.

Dataset: 
  The dataset used contains:
      Numerical Features: Age, Fare, SibSp (Siblings/Spouses Aboard), Parch (Parents/Children Aboard), Pclass (Ticket Class)
      Categorical Features: Sex, Embarked (Port of Embarkation)
      Target Variable: Survived (0 = No, 1 = Yes)
      
Data Preprocessing: 
  Handling Missing Values:Age and Fare: 
    Imputed using median values.
    Cabin: Dropped due to high missing values.
    Categorical columns: Encoded numerically.
  Feature Encoding: Converted categorical variables like Sex and Embarked using Label Encoding.
  Feature Scaling: Applied StandardScaler to normalize Age and Fare.
  
Model Selection: 
  Random Forest Classifier was used due to its robustness and high accuracy.
  Cross-validation was applied to ensure generalization.
  
Model Evaluation: 
  Accuracy: Measures overall correctness.
  Precision: Measures how many predicted positives were actually positive.
  Recall: Measures how many actual positives were correctly identified.
  F1-score: Harmonic mean of precision and recall.
  
Results: 
  The model achieved 100% accuracy, precision, recall, and F1-score, indicating potential data leakage or an extremely structured dataset.
