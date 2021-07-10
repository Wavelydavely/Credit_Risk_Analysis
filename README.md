# Credit_Risk_Analysis

Overview of the analysis:

FastLending would like to begin using machine learning to weed through their loan applications. We know that fraudulent applications are vastly outnumbered by legitimate applications, so it will be a challenge to measure each target equally. In this exercise, we will be using six different models to process the data available to us, at which time we will choose the best model.

Results: 

	-Oversampling:
		Balanced accuracy score = 0.6398437216722869
		Precision = .01
		Recall = 0.59
	-SMOTE:
		Balanced accuracy score = 0.6216172933512213
		Precision = .01
		Recall = 0.59
	-Undersampling:
		Balanced accuracy score = 0.5160196365189295
		Precision = .01
		Recall = 0.60
	-Combination:
		Balanced accuracy score = 0.6357786318898034
		Precision = .01
		Recall = 0.69
	-Balanced Random Forest Classifier:
		Balanced accuracy score = 0.7877672625306695
		Precision = .04
		Recall = 0.67
	-Easy Ensemble:
		Balanced accuracy score = 0.925427358175101
		Precision = .07
		Recall = 0.91

Summary: 

	No method is highly precise, meaning we will always have a substantial number of false positives. With our goal to weed out fraudulent applications though, this is fairly acceptable. It is far more important for us to prioritize sensitivity, even at the expense of precision. The Easy Ensemble AdaBoost Classifier is flagging 91% of fraudulent applications, while only 7% of the flagged applications are actually fraudulent. This model surpasses all other models, with the next best being the Balanced Random Forest Classifier flagging 67% of fraudulent application. We might like to increase the precision of our model, but we would recommend moving forward with the Easy Ensemble AdaBoost Classifier.