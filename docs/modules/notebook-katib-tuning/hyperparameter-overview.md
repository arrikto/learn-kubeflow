# Hyperparameter Tuning

## Hyperparameters
Hyperparameters are variables that control the model training process. You can use hyperparameter tuning to maximize the predictive accuracy of your models.


## Hyperparameter Tuning 
Automated hyperparameter tuning optimizes a target objective that you specify. A common metric is the model’s accuracy in the validation pass of the training job (validation-accuracy) or the model quality metric you are focused on. You can specify
whether you want the hyperparameter tuning job to maximize or minimize the metric. Katib will run several trials. Each trial tests a different set of values for your hyperparameters. At the end of the experiment, Katib outputs the optimized values for the hyperparameters.

## Post Hyperparameter Tuning
Once you have produced the ideal set of hyperparameters you are prepared to serve the most ideal version of your model into production.
