# Interview-Status-Prediction
Interview Status Prediction by Machine Learning

By: Eng. Anwar Hashem (PhD Student). 
 
Introduction:
The hiring entity or a specific service provider relies heavily on the personal interview in making employment or providing services decisions, as the interviewer tests the candidate’s analytical skills, and thus can select candidates suitable for the organization’s needs. But with the expansion of services and its conditions and the large number of applicants, the process becomes very cumbersome, and requires the use of machine learning to predict the results of the interview.
Machine learning algorithms have shown significant promise in accurately predicting interview-related outcomes. Various studies have explored the application of machine learning in predicting interview attendance.
This project focuses on predicting the status of job interviews using machine learning techniques. The goal is to create models that effectively determine whether a candidate would be considered, might be considered, or wouldn't be considered post an interview.

The Project Objective:
The "Interview Status Prediction" project focuses on building a predictive model to determine the status of job interviews, i.e. predict whether a candidate will pass or fail an interview. The goal is to create models that effectively determine whether a candidate would be considered, might be considered, or wouldn’t be considered post an interview.


Data Description: 
The dataset for the interview status prediction project consists of three CSV files as the following:
1-	Train: to train the machine learning model (learn patterns and relationships relevant to predicting interview outcomes). https://fastupload.io/6c39710a81864f69
2-	Test: to evaluate the performance of the trained model (predicts outcomes on this unseen data) https://fastupload.io/d1408114e1a38d33
3-	Result: to store the predictions made by the model on the test set. https://fastupload.io/b6d9f28a70ae2722
These files provide the necessary data for training, validating, and testing a predictive model for interview outcomes. 

Methodology: 
The steps taken during data preprocessing, EDA, and feature engineering. Include justifications for the methods used.
a-	Data Preprocessing:
1.	Data Cleaning: 
i.	Removed missing values or filled nulls using mode/mean.
ii.	dropped redundant columns.
iii.	
2.	Exploratory Data Analysis (EDA):
i.	Explored data distribution.
ii.	Identified outliers
iii.	Checked correlations between features.
b-	Feature Engineering:
1.	Label Encoding: Converted categorical variables into numerical representations for model compatibility.
2.	Feature Selection: Selected relevant features for training the models based on their impact on interview status prediction.

Explored data distribution for Categorical columns:

Identified outliers for Numerical columns:

We found that Interview duration: 
-	Mean: 37.3 minutes 
-	Standard deviation: 13.2 minutes.
-	Shortest interview: 15 minutes 
-	Longest Interview: 60 minutes.

Checked correlations between features:

We found that five columns in training data are important for the target column status.

Modeling: 
Decision Tree: A decision tree is a flowchart-like tree structure where an internal node represents feature (or attribute), the branch represents a decision rule, and each leaf node represents the outcome.

Random Forest: An ensemble method (based on the divide-and-conquer approach) of decision trees generated on a randomly split dataset. This collection of decision tree classifiers is also known as the forest.

AdaBoost: Mainly used for classification, and the base learner (the machine learning algorithm that is boosted) is usually a decision tree with only one level, also called as stumps. It makes use of weighted errors to build a strong classifier from a series of weak classifiers.


Gradient Boosting: Based on boosting in a functional space, where the target is pseudo-residuals rather than the typical residuals used in traditional boosting. It gives a prediction model in the form of an ensemble of weak prediction models, i.e., models that make very few assumptions about the data, which are typically simple decision trees.



Results and Evaluation: 
The visualizing of data:

The evaluation metrics for each model:
The detail of evaluation metrics for each model is shown in attached code file. 
As the details in attached report, the result shows that AdaBoost algorithm performed the best among the tested models for interview status prediction. 

Conclusion: 
-	There is no noticeable difference when removing the null values and when processing them with the mean and median due the dataset contains a small number of missing values
-	AdaBoost algorithm performed the best for interview status prediction. 
-	This tool can be highly valuable for recruitment processes, helping HR professionals streamline their efforts and make data-driven decisions. This method helps avoid biases, saves time for recruiters, and ensures fair hiring.


Attached files:
interview_status_prediction_by_ml:
https://colab.research.google.com/drive/1xgwAt0L6EBOlwe8AZ3wC2jHWMG4OVu-t#scrollTo=IoLhHh0_Fd4F

