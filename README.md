# Driver-Stress-Prediction-Using-GSR-values-and-Machine-Learning-Algorithms
AIM: to predict driver workload using GSR values and their corresponding Anxiety scores.
INTRODUCTION
The data set consisted of total 14 participants and had a total of 24 tasks for each participant. There were two types of workload
1) STATIC
2) DYNAMIC
And there were two types of vehicles that were used in the experiment.
1) MARUTI SUZUKI CRETA
2) GLOSTER
We have considered the dynamic data for the vehicle Maruti Suzuki CRETA for a total of 13 participants.Participant 14’s data was not considered due to incomplete or missing values.
INPUT AND OUTPUT FEATURES

For the Input variable(X) we have calculated Normalized GSR.
NORMALIZED GSR= EXPERIMENTAL GSR – BASELINE GSR

For the output variable(y) we have calculated Anxiety score.(0 or 1)

Anxiety score was premeditated by calculating the standard deviation value for each participant and taking the mean of these values for all the participants. If the value was smaller than the mean it was scored as low anxiety.(0) and if the value was higher than the overall mean ,then it was scored as high anxiety(1).
MODELS USED FOR TRAINING
We have used for models for training the dataset. They are
1. KNN Classifier(K neighbours)
2. Adaboost
3. RandomForest
4. LGBM Classifier


We Achieved the maximum accuracy rate with Knn classifier which is 0.84

The other models predicted the accuracy rates as 0.73,0.73 and 0.79 for Adaboost, Random forest and LGBM classifier respectively.

In the end I have also used the SHAP model to show the importance of input feature over the predicted values.

For Knn classifier: Accuracy : 0.84 precision: 0.89 recall: 0.68 F1.0-score: 0.77

For LGBM Classifier: Accuracy: 0.79 precision: 0.83 recall: 0.6 F1.0-score: 0.69

For Random forest classifier and Adaboost model : Accuracy: 0.73 precision: 0.83 recall: 0.4 F1.0-score: 0.54

AUC curve was calculated using Logistic Regression: AUC: 0.65

Feature importance using SHAP model was calculated using Random Forest classifier: Feature: Normalised GSR, Importance: [0.69032051]
