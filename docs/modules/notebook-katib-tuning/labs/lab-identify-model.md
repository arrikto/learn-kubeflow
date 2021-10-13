# Lab: Identify "ideal" Model for Hyperparameter Tuning
The notebook you executed evaluates three models in parallel. You must now select the ideal model for hyperparameter tuning. 

## Requirements 
To identify the ideal model evalaute all available outputs for model accuracy. 
Please review the remaining models to meet the following requirements:

1. The model accuracy for all three proposed models is known.
2. The ideal model has been selected. 

As a reminder for each of the metrics displayed

- r squared: generally a higher value indicates a better model fit
- mean squared error: generally a lower value indicates a better model fit
- mean squared logarithmic error: generally a lower value indicates a better model fit

## Solution

??? success 

      Keeping in mind that these are algorithmic models numerical output may not always be the same.
      Generally after reviewing all three models via the same method presented in the prior activity we can identify 
      that the xgb type has the best scores in each of the metric areas, therefore we will proceed with this model. 
