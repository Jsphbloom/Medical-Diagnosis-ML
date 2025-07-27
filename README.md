# Medical-Diagnosis-ML
Much time, effort and money is spent on diagnosing illnesses in patients. This takes up much of a doctor’s time, time that could be used elsewhere had the doctor utilized an accurate machine learning model to predict diagnoses of various illnesses based on collected health information. This model aims to do exactly that. The dataset I’m using has a binary 'at risk' feature for strokes. This machine learning tool is meant to help identify those at risk of strokes based on provided data.

The aim of this model is to reduce analysis times for individual patients, as an aid for doctors to accurately identify illnesses based on potentially hidden correlations. This will benefit the doctors as they will have more time to dedicate towards direct patient care, hospital management and stakeholders as more patients will be taken care of in a more efficient manner, and the patients themselves, as hospital wait times would reduce, and they receive a more accurate diagnosis of their illnesses.

False negatives are costly for the patient in this scenario. A missed diagnosis, especially if the model is heavily relied upon, could be detrimental to the patient’s health, and in turn, the hospital’s credibility. A false positive will warrant further inspection, and ultimately, the real cost is the time of review and rejection of a doctor. However, a false negative can mean the illness can go overlooked in the patient longer than it should, and incur more severe health and financial burdens. This will lead me to tune primarily for Recall, as false negatives are more costly using this approach. Success will be measured by the accuracy of the model, and how much time is saved by the doctors when using it to help review patient notes.




















Data Acquisition and Understanding

The dataset will be obtained from Kaggle. This dataset will be analyzed for null values and outliers, and basic visualizations of the data will be made before further exploration, to provide a starting point.

	Data Preparation and Feature Engineering

The data will be cleaned, features separated, values normalized, and prepared for model fitting. The target value will be dropped (condition), the data will be split into testing and training sets, and the features will be standardized using a scaler.

	Modeling Strategy

First and foremost, we’ll use a logistic regression model for a fast and simple baseline model. From there, we’ll use a Random Forest model, and then test XGBoost. We’ll calculate the cross validation score using the results from these models, and select the best one. That final model we will train with the best parameters on the entire training set.

	Results Interpretation and Communication

The results will demonstrate the accuracy of the model and its ability to predict conditions based on potentially unseen correlative factors. This will be pontificated upon in regards to potential business insights. There will be a visual component used to represent the results of the data processing.
