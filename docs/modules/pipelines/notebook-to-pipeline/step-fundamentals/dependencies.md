# Dependencies Between Pipeline Steps

In order to define a pipeline you need to identify not just the code that makes
up the step, but also specify the order in which the steps of your pipeline
should execute. To do this, select which step (or steps) should immediately
precede the step you are annotating by using the Depends on pull-down menu.

!!! important "Follow Along"
    Please follow along in your own copy of our notebook as we add a dependency
    for clean_data.

The step `clean_data` relies on `read_data` to read our dataset into a `pandas`
data frame (`df_auto`) so we need to define that relationship and establish the
sequence in which these two steps should execute.

![clean_data dependency](images/image59.png){: style="display: block; margin: auto; width:80%"}

With the work we’ve done so far, we now have a two-step pipeline that we can
summarize as follows.

!!! important "Make sure you understand your data dependencies"
    When considering how to organize your notebook into a Kubeflow pipeline it
    is essential that you assess the data dependencies between steps and ensure
    that values you’ve set for the Depends on field for each step reflect these
    dependencies.