# Solution - Lab: Skip Cells

## Requirements
1. Update the cells in the *Clean Data* section of our notebook so that cells
not necessary for cleaning data will be excluded from the `clean_data` pipeline
step. Here’s what `clean_data` looks like as you begin this exercise. 

![clean data step](images/clean_data.png)
{: style="display: block; margin: auto; width:80%"}

## Solution

We definitely need the first cell in the *Clean Data* section so no changes
are required here.

![clean_data first cell](images/clean_data-firstcell.png)
{: style="display: block; margin: auto; width:80%"}

This step, however, displays the data types for fields in this data set. We
use the output to identify the fact that we need to change the data type for
the ‘symboling’ column to ‘str’. However, we do not need to execute the cell
on each run of the pipeline we’re building.

![df_auto.dtypes()](images/df_auto-dtypes.png)
{: style="display: block; margin: auto; width:80%"}

The first two cells in the block below work together to fix some misspellings
and ensure that we are using the same label for ‘CarName’ across all rows.

![standardize car names](images/standardize-car-names.png)
{: style="display: block; margin: auto; width:80%"}

The cell below is diagnostic. It turns out that we don’t have any duplicates
in this data set, but even if we did, we do not need to run this cell as part
of the `clean_data` step or any pipeline step. We would only run cells that
dealt with duplicates. 

![df_auto.loc()](images/df_auto-loc.png)
{: style="display: block; margin: auto; width:80%"}

This cell is just a means of getting a quick peek at the data. It doesn’t do
any data cleaning.

![df_auto.head()](images/df_auto-head.png)
{: style="display: block; margin: auto; width:80%"}

!!! important "Follow Along
    Before continuing, please ensure the `clean_data` step in your notebook
    matches the solution above.