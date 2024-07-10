# Customer Churn Prediction

This project aims to build a machine learning model for predicting customer churn and identifying the most relevant features contributing to churn. The dataset used for this project is sourced from Kaggle and can be found [here](https://www.kaggle.com/datasets/ylchang/telco-customer-churn-1113). Detailed information about the dataset can be accessed [here](https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113).

The dataset file is named `df_merged.csv`.

## Code and Libraries Used

The code for this project is written in Python 3.10.12. The following libraries and tools were used:
- pandas 2.0.3
- numpy 1.25.2
- PyCaret 3.3.2
- Matplotlib 3.7.1
- SciPy 1.11.4
- scikit-learn (sklearn) 1.2.2
- Seaborn 0.13.1
- CatBoost 1.2.5
- LightGBM 4.1.0

## Workflow

1. **Data Cleaning and Exploratory Data Analysis (EDA)**:
   - Perform data cleaning and exploratory data analysis.
   - Encode categorical features as necessary.

2. **Outlier Detection**:
   - Implement outlier detection techniques to identify and possibly remove outliers (not yet implemented).

3. **Naive Model Building using PyCaret**:
   - Utilize PyCaret to quickly build initial models and establish a baseline for prediction.

4. **Model Fine-tuning using scikit-learn**:
   - Fine-tune the best performing models using scikit-learn to improve prediction accuracy.

5. **Visual Assessment of Best Performing Model**:
   - Evaluate the performance of the best performing model visually using confusion matrix and ROC curve.

6. **Identify Feature Importance**:
   - Determine the importance of features in predicting customer churn.

## Evaluation Metric: Recall

We use **recall** as the evaluation metric for this project. Recall is crucial in the context of customer churn prediction as it measures the ability of a model to correctly identify churn cases (true positives) out of all actual churn cases (true positives + false negatives). Maximizing recall helps in reducing the number of customers who churn but are incorrectly predicted as non-churners, thus minimizing potential revenue loss.

## Implementation in Jupyter Notebook

All tasks mentioned above are implemented in the Jupyter Notebook `customer_prediction.ipynb`. This notebook contains detailed code and explanations for each step of the workflow.

## TODO & Next Steps

1. **Address Class Imbalance Issue**:
   - Implement techniques to handle class imbalance in the dataset.

2. **Implement Outlier Detection and Removal**:
   - Integrate outlier detection and removal methods.

3. **One-hot Encode "contract" Feature**:
   - Perform one-hot encoding on the "contract" feature to enhance model performance.