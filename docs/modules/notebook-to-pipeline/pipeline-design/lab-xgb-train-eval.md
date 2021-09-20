# Lab: XGB train and eval steps

Following a process similar to what we did for the LGBM and RF regression
models above, reorganize the code and apply the appropriate annotations for
the XGB model. For this lab, the code you will work with is found in this cell.

![xgb step](images/xgb-step.png)
{: style="display: block; margin: auto; width:80%"}

## Requirements 

Reorganize and annotate the code for the XGB model to meet the following
requirements:

1. Create a new pipeline step called `train_xgb` to train the XGB model.
2. Create a new pipeline step called `eval_xgb` to evaluate the XGB model.
3. Specify the correct dependency relationships for both steps. **Note that
   the `train_xgb` step begins a branch in our pipeline. This branch can run
   in parallel with the branches for the LGBM and RF models.**
4. For each step, include only cells that contain code that is core to the
   step.
5. Exclude cells that are not core to one step or the other using the
   *Skip Cell* annotation.

## Solution

When you are finished, compare your notebook to the
[solution](lab-xgb-train-eval-solution.md) and make any necessary changes so
that your notebook matches the solution.

