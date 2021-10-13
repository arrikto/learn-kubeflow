# HyperParameter Tuning

## HyperParameters
Hyperparameters are the variables that control the model training process. Data Scientists frequently perform hyperparameter tuning to optimize the hyperparameter values to maximize the predictive accuracy of their models. 

## HyperParameter Tuning 
Automated hyperparameter tuning, offered by Arrikto, focuses on optimizing a target objective that you specify. A common metric is the model’s accuracy in the validation pass of the training job (validation-accuracy) or the model quality metric you are focused on. You can specify
whether you want the hyperparameter tuning job to maximize or minimize the metric. Katib will run several trial and each trial tests a different set of hyperparameter configurations. At the end of the experiment, Katib outputs the optimized values for the hyperparameters. 

## Post HyperParameter Tuning
Once you have produced the ideal set of hyperparameters you are prepared to serve the most ideal version of your model into production.
