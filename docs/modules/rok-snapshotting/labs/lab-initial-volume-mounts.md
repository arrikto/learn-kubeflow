# Lab: Initial Volume Mounts
Before the Kubeflow Pipeline run starts, Rok takes a snapshot of the workspace
and data volume. Then, it clones these snapshots to create new volumes that the
pipeline steps will use. The initial clones of the workspace volume and data
volume are mounted to each of the containers that are created to process the
Kubeflow pipeline steps.

## Requirements
You can identify where these volumes are mounted by reviewing the pipeline steps.

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
