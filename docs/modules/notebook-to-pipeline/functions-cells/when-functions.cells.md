# When to use *Functions* Cells

One annotation we’ve not yet discussed is the *Functions* cell type. Kale
provides this cell type to enable you to identify blocks of code containing:

- Functions used later in your machine learning pipeline.
- Global variable definitions (other than pipeline parameters) and code that
  initializes lists, dictionaries, objects, and other values used throughout
  your pipeline.

*Functions* cells help Kale identify all dependencies for pipeline steps. As
you know, Kale prepends the code in every cell annotated with *Imports* to the
code in the cells you’ve annotated with *Pipeline Step*. In addition, Kale also
prepends the code in every *Functions* cell as part of this process.

Kale executes each pipeline step as if it were a notebook composed of all
*Imports* cells in your notebook followed by all *Functions* cells, and then
followed by the cells annotated with *Pipeline Step* for the specific step in
question. Therefore all imports, variable declarations and setup statements
included in each *Imports* cell and all functions and other declarations found
in all *Functions* cells will execute before the core code for the pipeline
step.

Organizing functions together and annotating those cells with the *Functions*
label ensures that Kale can organize the code for each step and set up its
execution environment correctly.

