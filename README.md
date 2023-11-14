# deep-learning-challenge
HW16

# Alphabet Soup Deep Learning Model Analysis Report

## Overview of the Analysis

The analysis aimed to create a predictive model for Alphabet Soup using deep learning techniques. The objective was to develop a model capable of predicting successful outcomes for funding based on certain features provided in the dataset.

## Results

### Data Preprocessing

- **Target Variable:** The target variable for the model was 'IS_SUCCESSFUL', indicating the success or failure of funding.
- **Features:** Features included 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', and 'SPECIAL_CONSIDERATIONS'.
- **Removal of Variables:** Columns 'EIN' and 'NAME' were removed as they did not contribute to the model's predictive power.

### Compiling, Training, and Evaluating the Model

- **Model Configuration:**
  - The neural network model consisted of two hidden layers, with 80 and 30 neurons respectively, using ReLU activation functions. The output layer had a single neuron employing a sigmoid activation function for binary classification.
  - The choice of architecture was to strike a balance between complexity and computational cost.

- **Model Performance:**
  - Initially achieved an accuracy of approximately 72%.
  - Attempted optimization strategies included varying the number of neurons, layers, activation functions, and epochs in an effort to exceed the 75% target accuracy.

### Summary

The deep learning model, although initially promising, fell short of the target accuracy of 75%. To address this, a different approach using an SVM model was attempted.

## Recommendation for a Different Model

An alternative solution could involve utilizing a Support Vector Machine (SVM) for the classification problem. SVMs can be effective in handling high-dimensional data and are known for their capability to handle non-linear relationships in data. Their kernel trick allows for better classification in high-dimensional spaces. Moreover, feature scaling and proper tuning of hyperparameters can often yield improved results.

The SVM model could potentially overcome the limitations encountered with the neural network model and might provide better accuracy, especially after meticulous hyperparameter tuning.

In an attempt to improve the accuracy, the SVM model underwent hyperparameter optimization through GridSearchCV to systematically search through a parameter grid. The optimization process aimed to fine-tune the SVM model by exploring different combinations of hyperparameters, including 'C', 'gamma', and 'kernel'. After optimization, the SVM model achieved an improved accuracy. The best parameters identified were utilized to predict and evaluate the model on the test set. This optimization process represents an iterative approach to refining the SVM model's performance for more accurate pr

## Conclusion

In conclusion, while the deep learning model showed promise, it fell short of the target accuracy. Exploring alternative models such as SVMs, RNNs, Random Forests, and Decision Trees could be a viable strategies to enhance prediction accuracy for Alphabet Soup's funding outcomes.
