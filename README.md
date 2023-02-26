# Logistic_Regression_Model-Oversampled
use the original dataset, and resample the data by using the RandomOverSampler module from the imbalanced-learn library.

## Overview of the Analysis

 Purpose of the analysis:
	Credit risk poses a classification problem that’s inherently imbalanced. Using various techniques to train and evaluate modes with imbalances classes, and build a model that can identify the cerditworthiness of borrowers from the historical dataset.
* Based on the data set, I set the "loan_status" as a factor and train model. Predict the person is going to pay back the load or not base on each condiction.
* The model 1 value_counts is [0 : 75036, 1 : 2500] based on "loan_status". The model 2 after oversampled the value_counts is [0 : 56271, 1 : 56271] based on "loan_status".
* The stages of the machine learning process:
	- Split the Data into Training and Testing Sets
		- Step 1: Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
		- Step 2: Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
		- Step 3: Check the balance of the labels variable (y) by using the value_counts function.
		- Step 4: Split the data into training and testing datasets by using train_test_split.
	- Create a Logistic Regression Model with the Original Data
		- Step 1: Fit a logistic regression model by using the training data (X_train and y_train).
		- Step 2: Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model.
		- Step 3: Evaluate the model’s performance by Calculate the accuracy score of the model, Generate a confusion matrix, and Print the classification report.
	- Predict a Logistic Regression Model with Resampled Training Data
		- Step 1: Use the RandomOverSampler module from the imbalanced-learn library to resample the data. Be sure to confirm that the labels have an equal number of data points.
		- Step 2: Use the LogisticRegression classifier and the resampled data to fit the model and make predictions.
		- Step 3: Evaluate the model’s performance by Calculate the accuracy score of the model, Generate a confusion matrix, and Print the classification report.

* Method:
	- LogisticRegression
	- RandomOverSampler

## Results

* Machine Learning Model 1:

	- Model 1 confusion Matrix </br>
	![alt text](https://github.com/wf880180/LogisticRegressionModelOversampled/blob/main/Image/Model1Matrix.png)
	- Model 1 Result</br>
	![alt text](https://github.com/wf880180/LogisticRegressionModelOversampled/blob/main/Image/Model1Result.png)

	* The accuracy is 99 percent. (18663+563) / (18663 + 102 + 56 + 563) = 0.9918
	* The precision is 99 percent. 18663 / (18663 + 18716) = 0.9971
	* The recall is 99 percent. 18663 / (18663 + 102) = 0.9945


* Machine Learning Model 2:
	- Model 2 confusion Matrix </br>
	![alt text](https://github.com/wf880180/LogisticRegressionModelOversampled/blob/main/Image/Model2Matrix.png)
	- Model 2 Result</br>
	![alt text](https://github.com/wf880180/LogisticRegressionModelOversampled/blob/main/Image/Model2Result.png)

	* The accuracy is 99 percent. (18649+615) / (18649 + 116 + 4 + 615) = 0.9938
	* The precision is 99 percent. 18649 / (18649 + 56) = 0.9970
	* The recall is 99 percent. 18649 / (18649 + 116) = 0.9938

## Summary

* Which one seems to perform best? How do you know it performs best?
	- Model 2 is doing better because Model 2's balance is higher and most rate is higher than Model 1.

* Does performance depend on the problem we are trying to solve?  (For example, is it more important to predict the 1's, or predict the 0's? )
	- Yes, in this case we want more accuracy of people pay back the loan, so we'll more focus on the status pay back.