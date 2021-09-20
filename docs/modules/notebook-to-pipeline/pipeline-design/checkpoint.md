# Checkpoint: Pipeline Design

Having completed the lessons in this module, you should now be able to do the
following comfortably:

1. Identify code in a notebook that implements a discrete step in a machine
learning workflow and annotate that cell as a *Pipeline Step*.
2. Identify the data that one step produces as output and the step or steps
that depend on that data as input. 
3. Specify single-step and multi-step dependency relationships between
Kubeflow pipeline steps using the Depends on parameter of the *Pipeline Step*
annotation.
4. Create pipeline branches that can run in parallel using the *Depends on*
parameter of the *Pipeline Step* annotation.
5. Organize the Python statements that import modules your pipeline steps need
into a small number of cells and mark those cells using the Imports annotation.
6. Identify cells in a notebook that should be excluded from pipeline runs and
annotate them as Skip Cells.
7. Organize and annotate Functions cells.

