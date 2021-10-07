# Lab: Set Up Katib Job

Setting up the Katib Job takes place within the Kale UI either within MiniKF or Enterprise KubeFlow deployment with Arrikto. 
By setting up the job from within the Kale UI you are ensuring that Katib can take advantage of the KubeFlow Pipelines and the Rok Snapshotting.
The preparation done in advance ensures that when you go to configure a Katib Job all the options will be prepopulated or will be based on
what has been defined in the notebook cells. 

## Requirements 
To configure the hyperparameter tuning job you will need to configure each of the below:

### Search Space Parameters 
All hyperparameters are to be considered with the following details:
- NUM_ESTIMATORS should start at 400 and go to 600 at intervals of 10.
- MAX_DEPTH should be between 1 and 5 at intervals of 1.
- LEARNING_RATE should be between 0 and 1 at intervals of 0.1.

### Search Algorithm
This should be Grid Search.

### Search Objective
You are trying to maximize the value of r squared. 

### Run Parameters
You should do at last 3 trials, at most 12 and stop after 3 failed attempts. 

Please configure the Katib Job to meet the above requirements. 

## Solution

??? success
    
    The solution is displayed in the screenshots below: 
    ![set up katib job answers](images/set-up-katib-job-answers.png)
    {: style="display: block; margin: auto; width:80%"}

## Next Steps
Once you have confirmed that your solution is consistent with what is expected click COMPILE AND RUN to begin execution. 
