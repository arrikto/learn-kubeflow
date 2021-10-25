# Lab: Identify "ideal" Model for Hyperparameter Tuning
The notebook you executed evaluates three models in parallel. 
You must now select the ideal model for hyperparameter tuning. 

## Requirements 
To identify the ideal model, evaluate all available outputs for model accuracy. 
In the prior section you looked at the quality metrics for one model.
Now you must review the quality metrics for the remaining models.
Once you have reviewed all three models you will be able to pick the 
best performing model. This is the model you will use for hyperparameter tuning. 

As a reminder for each of the metrics displayed

- r squared: generally a higher value indicates a better model fit
- mean squared error: generally a lower value indicates a better model fit
- mean squared logarithmic error: generally a lower value indicates a better model fit

The ideal model is the model with the best quality metrics
per the descriptions above. 

## Solution

??? success "View Solution"

      Keeping in mind that these are algorithmic models numerical output may not always be the same.
      Generally after reviewing all three models via the same method presented in the prior activity we can identify 
      that the **xgb** type has the best scores in each of the metric areas, therefore we will proceed with this model. 
      In the next section you will isolate this model in the notebook and skip the other models
      so that your hyperparameter tuning focuses only on one model. At this point your Notebook 
      should not be changed you should only have the ideal model identified. Please proceed to the next section. 
