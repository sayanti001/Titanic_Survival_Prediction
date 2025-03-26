```markdown
# Titanic Survival Prediction

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the required dependencies.

```bash
pip install -r requirements.txt
```

## Usage

```python
# Run the Python script to train the model
python titanic_survival_prediction.ipynb
```

## Project Overview

This project aims to develop a machine learning model to predict whether a passenger survived the Titanic disaster. The dataset includes various features such as age, gender, ticket class, fare, cabin information, and more. The goal is to preprocess the data effectively and build a classification model to achieve high prediction accuracy.

## Dataset

The dataset used contains:

- **Numerical Features**: Age, Fare, SibSp (Siblings/Spouses Aboard), Parch (Parents/Children Aboard), Pclass (Ticket Class)
- **Categorical Features**: Sex, Embarked (Port of Embarkation)
- **Target Variable**: Survived (0 = No, 1 = Yes)

## Data Preprocessing

1. **Handling Missing Values**:
   - Age and Fare: Imputed using median values.
   - Cabin: Dropped due to high missing values.
   - Categorical columns: Encoded numerically.
2. **Feature Encoding**:
   - Converted categorical variables like Sex and Embarked using Label Encoding.
3. **Feature Scaling**:
   - Applied StandardScaler to normalize Age and Fare.

## Model Selection

- **Random Forest Classifier** was used due to its robustness and high accuracy.
- Cross-validation was applied to ensure generalization.

## Model Evaluation

The trained model was evaluated using:

- **Accuracy**: Measures overall correctness.
- **Precision**: Measures how many predicted positives were actually positive.
- **Recall**: Measures how many actual positives were correctly identified.
- **F1-score**: Harmonic mean of precision and recall.

### Results

The model achieved **100% accuracy, precision, recall, and F1-score**, indicating potential data leakage or an extremely structured dataset.

## Repository Structure

```
📂 titanic-survival-prediction
├── 📄 titanic_survival.py  # Main script for training and evaluation
├── 📄 README.md            # Project documentation
├── 📄 requirements.txt     # Dependencies
└── 📄 tested.csv           # Dataset
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Future Improvements

- Investigate potential **data leakage** causing perfect accuracy.
- Experiment with other classification models such as Logistic Regression and XGBoost.
- Implement hyperparameter tuning to optimize model performance.

## License

[MIT](https://choosealicense.com/licenses/mit/)
```
