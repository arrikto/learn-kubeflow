# Solution - Lab: Create `split_data` Step

In the *Build Models* subsection of the *Modeling* section, we split data for
training and evaluation and then build and evaluate three regression models.
In this lab, we’ll define a pipeline step for the data splitting portion of our
workflow.

## Requirements 

Annotate one or more cells in the *Build Models* section of our notebook to
meet the following requirements:

1. Annotate one or more cells in our notebook to create a pipeline step named
   `split_data` that splits our dataset for use in later training and
   evaluation steps.
2. Specify the correct dependency relationship for `split_data`.

## Solution

Requirement 1: We accomplish splitting the data in just one cell. Annotate this
cell as depicted below to create the `split_data` pipeline step.

![split_data done](images/split_data-done.png)
{: style="display: block; margin: auto; width:80%"}

Requirement 2: The `split_data` step depends on the output of `prep_data` which
selects just the significant columns in our dataset and transforms categorical
columns for training.

Our pipeline can now be depicted as:

![pipeline with split_data](images/pipeline-split_data.png)
{: style="display: block; margin: auto; width:80%"}

