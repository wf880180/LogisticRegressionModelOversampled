# Logistic_Regression_Model-Oversampled
use the original dataset, and resample the data by using the RandomOverSampler module from the imbalanced-learn library.

## Overview of the Analysis

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

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

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.