# Diabetes-Machine-Learning

<img width="275" height="183" alt="image" src="https://github.com/user-attachments/assets/363973ce-7cbc-4e03-b462-d62850bf7820" />



## Table of Contents
-[Project Objective] (#project-objective)

-[Data Source]

-[Exploratory Data Analysis] (#Exploratory-Data Analysis)

-[Data Preprocessing] (#Data-Preprocessing)

-[Machine Learning Model] (#Machine-Learning-Model)

-[Evaluation Metrics] (#Evaluation-metrics)

-[Key insights] (#Key-insights)

-[Conclusions] (#Conclusions)




## Project Objective.
The goal is to predict the likelihood of diabetes onset, allowing for timely and targeted preventive measures.
This initiative will empower Stark Health Clinic to enhance patient outcomes, reduce the burden on healthcare resources, and play a proactive role in combating the diabetes epidemic.

## Data Source
10Alytics provided the Datasets used in this project, which contain features like "Gender, Age, Smoking history, BMI, heart disease, hypertension, and other relevant information.

## Exploratory Data Analysis.
EDA was performed to uncover different patterns in the datasets. Univariate, Bivariate, and multivariate analyses were performed, and outliers were identified and handled.

## Data Preprocessing.
During Data Preprocessing, the Target variable was noticed to have high class imbalance, which was later handled. All Categorical variables were encoded, while scaling was performed on the numerical variables to ensure uniformity in the numerical features(columns).

## Machine Learning.
Logistic Regression was used as our baseline model, where the Recall on both classes were class 0 was 0.99 and class 1 was 0.62. The false Negative is 655, which is a very high variable to be accepted. Several other models like, "LogisticRegression, SGDClassifier, SVC, KNeighborsClassifier, DecisionTreeClassifier, and Ensemble Classifiers" were all trained by adding a "class_weights = {0:1, 1:4}" to improve the model performance. Sticking to LogisticRegression, the recall on Class 1 was 0.77571 and False Negative reduced to 386. 
 
SMOTE technique was applied to the Target Variable, by over_sampling the minority variable to have equal class balance and retraining all the models. Random Forest WAS selected as the Model to be Recommended and deployed as the False Negatve is 87, recall for class 0 was 0.99 and class 1 was 0.95. Feature Importances can be further done.

## Evaluation Metrics.
Precision, Recall, Accuracy and (False Negative)  were evaluation metrics considered before selecting Random ForestClassifier as our Model. 

Accuracy - Classification tasks that measure the percentage of correctly predicted classes out of al the predictions made.
Precision - Proportion of true positive predictions among all the positive predictions.
Recall - Proportion of true positive predictions among all actual positive instances.

## Key Insights
The model built was able to corrected predict the True Negative 17398, 
True Negative was 1634.
False Negative 87. 
False Positive was 111.

The RandomForest performance which was selected as our model, looked into Key Insights about the performance of the model and its evaluation metrics before selected. 

## Conclusion
The model choosen after advanced model building by applying different advanced machine learning techniques showed that the model can be recommended and deployed by Stark Healthcare, which can help in early detection of Diabetes and also reduce the burden on healthcare resources and improve effficiency, productivity and play a proactive role in combating Diabetes.






