# Checkpoint: Kale Fundamentals

At this point, we’ve covered the *Pipeline Step*, *Imports*, and *Skip Cell*
annotations. With a little review here and there you should now be able to
recall how to do the following:

1. Identify code in a notebook that implements a discrete step in a machine
learning workflow and annotate that cell as a Pipeline Step.
2. Identify the data that one step produces as output and the step or steps
that depend on that data as input. 
3. Specify dependency relationships between Kubeflow pipeline steps using the
Depends on parameter of the Pipeline Step annotation.
4. Organize the Python statements that import modules your pipeline steps need
into a small number of cells and mark those cells using the Imports annotation.
5. Identify cells in a notebook that should be excluded from pipeline runs and
annotate them as Skip Cells.
