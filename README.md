# Bike-sharing-demand-project
AWS Machine Learning nanodegree

This project is part of the submission for AWS Machine Learning nanodegree Project 1 due on May 24, 2025.
This Report targets to answer questions indicated in the strater code.

Describe the `predictions` series to see if there are any negative values.
During the first trail the minimum value from predictions.describe() is found to be 3.013077
Hence, there are no negative predictions.

## Add nw features
Some of the features are changed to be categorical and year, month, day and hour columns are generated from the datetime column for the second trial.

The minimum value of predictor in the second trial is 2.454035. Hence, no negative values.

The kaggle submission is accepted and the result is summerized below;
fileName                     date                        description           status                     publicScore  privateScore  
---------------------------  --------------------------  --------------------  -------------------------  -----------  ------------  
submission_new_features.csv  2025-05-25 18:32:44.883000  new features          SubmissionStatus.COMPLETE  0.60985      0.60985       
submission.csv               2025-05-25 16:59:55.580000  first raw submission  SubmissionStatus.COMPLETE  1.80136      1.80136   


## Change hyperparameters
The following hyperparameters are changed to he values below;
hyperparameters={
        'RF': {'n_estimators': 300, 'max_depth': 15},
        'XGB': {'learning_rate': 0.05, 'max_depth': 8},
        'CAT': {'iterations': 1000, 'learning_rate': 0.03},
        'NN_TORCH': {'num_epochs': 20},
    }

    In the hyperparameter case the minimum prediction values are found to be -11.0125
    Hence, negative predictions are corrected to be zero.

fileName                   date                      description                      status                 publicScore  privateScore  
----------------------  --------------------------  -----------------------------  -----------------------  -----------  ------------  
submission_new_hpo.csv    2025-05-25 19:13:47.703000  new features with hyperparameters  SubmissionStatus.COMPLETE  0.51037      0.51037       
submission_new_features.csv  2025-05-25 18:32:44.883000  new features                   SubmissionStatus.COMPLETE  0.60985      0.60985       
submission.csv               2025-05-25 16:59:55.580000  first raw submission          SubmissionStatus.COMPLETE  1.80136      1.80136       
