# Lab: Create a train_rf and eval_rf steps

Following a process similar to what we did for the LGBM regression model in the
previous section, reorganize the code and apply the appropriate annotations for
the RandomForest (RF) model. For this lab, the code you will work with is found
in this cell.

![rf cell](images/rf-cell.png)
{: style="display: block; margin: auto; width:80%"}

## Requirements 

Reorganize and annotate the code for the RF model to meet the following
requirements:

1. Create a new pipeline step called `train_rf` to train the RF model.
2. Create a new pipeline step called `eval_rf` to evaluate the RF model.
3. Specify the correct dependency relationships for both steps. **Note that
   the `train_rf` step begins a branch in our pipeline. This branch can run in
   parallel with the branch for the LGBM model.**
5. For each step, include only cells that contain code that is core to the step.
6. Exclude cells that are not core to one step or the other using the *Skip Cell*
   annotation.

## Solution

When you are finished, compare your notebook to the
[solution](lab-rf-train-eval-solution.md) and make any necessary changes so
that your notebook matches the solution.
