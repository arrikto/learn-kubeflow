# Lab: Create `prep_data` step

In the *Prep Data* section of our notebook, we are performing two operations:

1. Selecting the significant independent variables (columns) that we will
   use as features for our regression models and only including these columns
   in our data frame.
2. Encoding categorical variables so that they can be used by our models. 

## Requirements

To incorporate the *Prep Data* section as a step in our Kubeflow pipeline,
please modify your copy of our notebook to meet the following requirements:

1. Create a new pipeline step.
2. Set the step name to `prep_data`.
3. Specify the correct step on which `prep_data` depends as the *Depends on*
   parameter.
4. As part of this annotation, include all cells that contain code that is core
   to the step `prep_data`.
5. Exclude cells in the *Prep Data* section that are **not** core to the
   functionality of this step.

## Solution

When you are finished, compare your notebook to the
[solution](lab-prep_data-solution.md) and make any necessary changes so that
your notebook matches the solution.
