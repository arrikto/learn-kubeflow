# Gather Imports in One Cell

## Why?

In general, though convenient, it’s usually not a good idea to scatter imports
throughout your code. It almost always leads to errors caused by references to
modules that you end up using before the location where you had imported them
originally.

When building pipelines with Kale, it’s essential that you organize your
imports together in one or two cells and then annotate those cells using the
*Imports* label. This will avoid pipeline execution errors due to missing
modules and enable Kale to configure the execution environment for each
pipeline step correctly.

## How Kale uses Imports cells
Kale prepends the code in every cell annotated with *Imports* to the code in
the cells you’ve annotated with *Pipeline Step*. Kale executes each pipeline
step as if it were a notebook composed of all *Imports* cells in your notebook
followed by the cells annotated with *Pipeline Step* for the specific step in
question. Therefore all imports, variable declarations and setup statements
included in each *Imports* cell will execute before the core code for the
pipeline step.

Organizing imports together and annotating those cells as Imports ensures that
Kale can organize the code for each step and set up its execution environment
correctly.
