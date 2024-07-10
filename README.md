# Customer Churn Prediction

The aim of this project was to build a ML model for predicting customer churn and to identify the most relevant features contributing to customer churn. The dataset used for this project is sourced from Kaggle and can be found [here](https://www.kaggle.com/datasets/ylchang/telco-customer-churn-1113). Detailed information about the dataset can be accessed [here](https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113).

The dataset file is named `df_merged.csv`.

## Workflow

1. **Data Cleaning and EDA**:
   - Perform data cleaning and exploratory data analysis.
   - Encode categorical features as necessary.

2. **Outlier Detection**:
   - Implement outlier detection techniques to identify and possibly remove outliers (not yet implemented).

3. **Naive Model Building using PyCaret**:
   - Utilize PyCaret to quickly build initial models and establish a baseline for prediction.

4. **Model Fine-tuning using sklearn**:
   - Fine-tune the best performing models using `sklearn` to improve prediction accuracy.

5. **Visual Assessment of Best Performing Model**:
   - Evaluate the performance of the best perfoming model visually using confusion matrix and ROC curve.

6. **Identify Feature Importance**:
   - Determine the importance of features in predicting customer churn.

## Evaluation Metric: Recall

For this project we use **recall** as the evaluation metric. Recall is particularly important in the current context of customer churn prediction because it measures the ability of a model to correctly identify churn cases (true positives) out of all actual churn cases (true positives + false negatives). Maximizing recall helps in reducing the number of customers who churn but are incorrectly predicted as non-churners, thus minimizing potential revenue loss.

## Implementation in Jupyter Notebook

All tasks mentioned above are implemented in the Jupyter Notebook `customer_prediction.ipynb`. This notebook contains detailed code and explanations for each step of the workflow.

## TODO & Next Steps

1. **Tackle Class Imbalance Issue**:

2. **Implement Outlier Detection and Removal**:

3. **One-hot Encode "contract" Feature**:

---