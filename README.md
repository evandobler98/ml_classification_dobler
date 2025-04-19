# 🍄 Mushroom Classification Project

## Overview

This project focuses on classifying mushrooms as edible or poisonous using machine learning techniques. The dataset, sourced from the UCI Machine Learning Repository, contains various categorical features describing mushroom characteristics.

## Dataset

- **Source**: [UCI Mushroom Dataset](https://archive.ics.uci.edu/ml/datasets/Mushroom)
- **Features**: 22 categorical attributes (e.g., cap shape, odor, gill color)
- **Target**: Edibility (`e` for edible, `p` for poisonous)

## Methodology

1. **Data Preprocessing**:
   - Loaded the dataset and assigned appropriate column names.
   - Handled missing values and encoded categorical features using one-hot encoding.

2. **Feature Selection**:
   - Selected features based on domain knowledge and exploratory data analysis.
   - Focused on attributes like odor, gill color, and spore print color, which showed significant correlation with the target variable.

3. **Model Training**:
   - Implemented two classification models:
     - Decision Tree Classifier
     - Random Forest Classifier
   - Split the dataset into training and testing sets (70% training, 30% testing).

4. **Evaluation**:
   - Assessed model performance using accuracy, confusion matrix, and classification report.
   - Both models achieved high accuracy, with the Decision Tree slightly outperforming the Random Forest.

## Results

- **Decision Tree Classifier**:
  - Accuracy: 99.5%
  - Confusion Matrix:
    ```
    [[1263    0]
     [  12 1163]]
    ```

- **Random Forest Classifier**:
  - Accuracy: 99.4%
  - Confusion Matrix:
    ```
    [[1263    0]
     [  13 1162]]
    ```

## Conclusion

The models effectively classified mushrooms with high accuracy. The Decision Tree model performed slightly better, likely due to the dataset's simplicity and the categorical nature of the features.

## Future Work

- Explore additional classification algorithms (e.g., Logistic Regression, SVM).
- Perform hyperparameter tuning to optimize model performance.
- Implement cross-validation for more robust evaluation.
- Visualize decision boundaries and feature importances for better interpretability.

## Repository

- [Project Notebook](https://github.com/evandobler98/ml_classification_dobler/blob/main/classification_dobler.ipynb)
