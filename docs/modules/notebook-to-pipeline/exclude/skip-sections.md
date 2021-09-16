# Skip Sections Not Used in Pipelines

The Visualize Data section of this notebook informs how we build models. It
is what we used to identify the significant independent variables in this
dataset as reflected in this portion of the notebook.

![significant variables](images/sig_col.png)
{: style="display: block; margin: auto; width:80%"}

We use the outcome of our analysis to define the list `sig_col` near the top of
the *Modeling* section. We don’t need to run the cells in the *Visualize Data*
section as part of our pipeline, though we should keep this section in the
notebook because, as is the case with most projects of this nature, we will
likely need to refine our models further and want to return to a visualization
and analysis phase in a future iteration.