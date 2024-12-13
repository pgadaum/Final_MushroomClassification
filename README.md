# Mushroom Classification Project
![](UTA-DataScience-Logo.png)

## Project Overview
This project focuses on classifying mushrooms as either edible (safe for consumption) or poisonous using machine learning techniques. The dataset used for this classification task is the **Mushroom Classification Dataset** from Kaggle, which provides information about various physical characteristics of mushrooms. Our best model, a Random Forest model, achieved an accuracy of 100% on the validation dataset. This performance indicates a highly effective classification of mushrooms into edible or poisonous categories.

## Dataset Details
- **Source:** [Kaggle Mushroom Classification Dataset](https://www.kaggle.com/datasets/uciml/mushroom-classification)
- **License:** CC0-1.0
- **Number of Rows:** 8,124
- **Number of Features:** 23
- **Target Column:** `class`
  - Edible: `0`
  - Poisonous: `1`

## Project Workflow

### 1. Data Loading and Exploration
- The dataset was downloaded using the Kaggle API.
- The data was inspected to understand its structure and contents.
- Key initial checks included counting rows and features, checking for missing values, and assessing class balance.

### 2. Data Analysis
- **Class Balance:** The dataset is balanced with 4,208 edible mushrooms and 3,916 poisonous mushrooms.
- **Target Encoding:** The `class` column was encoded as `0` (Edible) and `1` (Poisonous).
- Histograms and count plots were generated to visualize feature distributions and their relationships with the target variable.

### 3. Data Cleaning and Preparation
- Checked and removed any duplicated rows (none found).
- One-hot encoding was applied to categorical features to prepare the dataset for machine learning models.
- Split the dataset into training, validation, and test sets with a 60-20-20 ratio.

### 4. Machine Learning Model Development
Three machine learning models were implemented and evaluated:

#### Random Forest Classifier
- **Validation Accuracy:** 1.0000
- **Test Accuracy:** 1.0000

#### Decision Tree Classifier
- **Validation Accuracy:** 1.0000
- **Test Accuracy:** 1.0000

#### Gradient Boosting Classifier
- **Validation Accuracy:** 0.9982
- **Test Accuracy:** 1.0000

### 5. Model Evaluation and Submission
- Validation and test sets were used to evaluate model performance using metrics such as accuracy and classification reports.
- Submission files were generated for the Kaggle competition using predictions from the trained models.

## How to Run the Code
1. Install required libraries:
   ```bash
   pip install pandas scikit-learn matplotlib seaborn kaggle
   ```
2. Set up Kaggle API credentials as described in the code.
3. Run the notebook to:
   - Load and preprocess the data.
   - Train machine learning models.
   - Evaluate and generate predictions.

## File Descriptions
- **Final_MushroomClassification.ipynb:** Jupyter Notebook containing the full implementation.
- **mushrooms.csv:** Original dataset (downloaded from Kaggle).
- **submission.csv:** Submission file containing predictions from the Random Forest model.
- **submission_gbc.csv:** Submission file containing predictions from the Gradient Boosting model.

## Key Results
- All models achieved near-perfect accuracy on the validation and test datasets, demonstrating the effectiveness of machine learning techniques on this dataset.
- The Random Forest and Decision Tree models achieved a test accuracy of 1.0000, making them ideal for this classification task.

## Future Work
- Explore hyperparameter tuning to further optimize the models.
- Investigate feature importance to identify the most influential mushroom characteristics.
- Experiment with additional algorithms such as Support Vector Machines or Neural Networks.

## Acknowledgements
This project uses the Mushroom Classification Dataset from UCI Machine Learning Repository, made available on Kaggle. The dataset is publicly available under the CC0 license.
