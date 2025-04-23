# Titanic Survival Modeling - Final Project

This project explores the Titanic dataset to build a predictive model for passenger survival. The work was completed collaboratively as a final project for my Analytics Models course and involves extensive feature engineering, model training, evaluation, and comparison.

## Files
- `MAT 340 Final Project.ipynb`: Full code with documentation and outputs
- `Titanic Analytics Models Final Presentation.pptx`: PowerPoint slides used for the final presentation
- `README.md`: Project overview and explanations


## Project Overview

Using the Titanic dataset from Kaggle, we explored multiple classification models to predict whether a passenger survived. We:
- Cleaned and merged the dataset
- Selected meaningful features
- Trained and evaluated three models:
  - Logistic Regression
  - K-Nearest Neighbors (KNN)
  - Random Forest Classifier (final model)


## Data Preparation

- Merged `train.csv` and `test.csv` using `PassengerId`
- Converted categorical variables (`Sex`) to numeric
- Filled missing `Age` and `Fare` values with the **median**
- Final features used: `Sex`, `Age`, `SibSp`, `Parch`, `Fare`


## Models Used

### 1. Logistic Regression
- Accuracy: **78%**
- Survivor Recall: **69%**
- Pros: Simple, interpretable
- Cons: Limited in capturing non-linear patterns

### 2. K-Nearest Neighbors (KNN)
- Accuracy: **70%**
- Survivor Recall: **53%**
- Pros: Intuitive and non-parametric
- Cons: Sensitive to feature scaling, lower performance

### 3. Random Forest (Tuned) Final Model
- Accuracy: **81%**
- Survivor Recall: **72%**
- Non-Survivor Recall: **88%**
- Tuned Parameters: `n_estimators=20`, `max_depth=200`, `max_leaf_nodes=100`
- Pros: Strong performance, interpretability via feature importance

## Evaluation Metrics

We used:
- Confusion Matrix
- Accuracy
- Precision
- Recall
- F1-Score
- Feature Importance Visualization
- Decision Tree Graph


## Final Model Decision

We selected the tuned Random Forest Classifier due to its superior performance in accuracy, recall, and interpretability. It provided both predictive power and valuable feature insights, making it the best choice for our survival prediction task.


## Tools Used

- Python (Pandas, Scikit-Learn, Matplotlib, Seaborn)
- Google Colab
- GitHub


## Authors

- Omari Emmanuel  
- Hanna Nguyen
- Chris Smith

Queens University of Charlotte  
Spring 2025

## Resources
- [Colab Notebook Link](https://colab.research.google.com/drive/1qYUmOyqNNzVBlotFbG-1BPgfh4OFjr9S)

## GitHub Repository
All project-related code and detailed documentation are available in this repository.

Feel free to explore the project, review the analysis, and reach out with any feedback!

