# Diabetes Prediction Using Supervised Learning techniques.

# Project/Goals
The ultimate goal of the project is to gain insights from the data sets and communicate these insights to stakeholders using appropriate visualizations and metrics to make informed decisions based on the business questions asked.
Questions asked:
- Are there any missing values in the dataset?
- How are the predictor variables related to the outcome variable?
- What is the correlation between the predictor variables?
- What is the distribution of each predictor variable?
- Are there any outliers in the predictor variables?
- How are the predictor variables related to each other?
- Is there any interaction effect between the predictor variables?
- What is the average age of the individuals in the dataset?
- What is the average glucose level for individuals with diabetes and without diabetes?
- What is the average BMI for individuals with diabetes and without diabetes?
- How does the distribution of the predictor variables differ for individuals with diabetes and without diabetes?

# Process
Step 1: Obtaining data
This dataset is originally from the National Institute of Diabetes and Digestive and Kidney
Diseases. The objective of the dataset is to diagnostically predict whether a patient has diabetes,
based on certain diagnostic measurements included in the dataset. 
[Kaggle Dataset](https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset)

Step 2: Loading and understanding the dataset.
- Working with diabetes.cvs data to understand  each predictor variables included in the dataset.
- Having a general understanding and information about the relationship between various features that contribute to the target variable (outcome).

Step 3:EDA.exploratory data analysis, 
- Create a displot, histplot, scatterplot and pairplot to look at the distributions of different predictor variables and their correlation.
- Learn the trend and detect outlier or possible factor that can affect the statistical model.
- Create heatmap to take a closer look at the corellation.

Step 4: preprocessing and feature engineering.
- Detect and handle outliers.
- Structure the data for efficient analysis.
- Split the into training and testing for appropriate training .
- Scale the data 

Step 5:Building a  Logistic regression model.
Since the dataset contains continuous numerical data and  a binary data, a Logistic regression model was built to prediction model whether a patient has diabetes or not.
An ensemble  which is RaandomForest Classifier  was also built for proper performance comparism between the two models.

step 6:Evaluation metrics: Appropriate evaluation metrics such as accuracy, precision, recall, F1-score, and ROC-AUC, confusion matrix and Classification Report were included to futher evaluate our models.

step 7: Hypertuning and Cross-validation were performed to get a more robust estimate of the model's performance.

# Results
- Average glucose level for individuals with diabetes are 141.257 and without diabetes  are 109.980.
- Average BMI for individuals with diabetes 35.1425 are and without diabetes are 30.304
- Average age of individuals in the dataset is 33 years.
- Based on a correlation of 0.47, Glucose is the most strongly correlated feature with the Outcome which suggests that higher glucose levels could be a significant indicator of diabetes.BMI can be also important factor in diabetes.
- Based on the evaluation metrics,the Random Forest Classifier model has a slightly higher accuracy(0.7316) compared to the Logistic Regression model(0.7272).
- In terms of precision,the Logistic Regression model has slightly higher precision than the Random Forest Classifier, which indicates that it makes fewer false positive predictions however, the Random Forest Classifier has a slightly higher ROC-AUC score (0.7065) compared to the Logistic Regression model (0.6885). 
- Additionally, the Random Forest Classifier has slightly higher F1 Score and recall values.
- In summary, the Random Forest Classifier model has higher accuracy,recall,F1 score and ROC-AUC than the Logistic Regression model. The Random Forest Classifier model could be preferred based on these evaluation metrics.
 # conclusion
 -Random Forest Classifier appear to have a better accuracy than Logistic regression model in predicting  whether a patient have Diabetes or not.
- Cross validation gave more robust estimate of the model performances  with increased Mean CV Accuracy: 0.7820 and Mean CV Precision: 0.7229
- Glucose level is the most important feature in predicting whether a patient have Diabetes or not.
- The least important feature that doesn’t really affect the prediction is Skin thickness.


