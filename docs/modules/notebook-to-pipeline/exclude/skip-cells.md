# Skip Cells Not Used in a Step

In their current form, our `read_data` and `clean_data` steps both contain a 
number of lines of code that generate diagnostic output or do other work that
is not core to the work of those steps. For pipeline runs, we don’t want to
include this code, because it will add unnecessary compute cycles and
execution time.

![read data step](images/read_data.png)
{: style="display: block; margin: auto; width:80%"}

We can keep this code in our notebook where it will be of use as we continue
to develop our models, but explicitly exclude it from pipeline steps. To do
this, we need to make sure that all the statements to be excluded are in
separate cells from the code that is core to pipeline steps. Then, we can
apply the *Skip Cell* annotation to these cells.

!!! important "Follow Along"
    Please follow along in your own copy of our notebook as we annotate skip cells.

For the `read_data` step, we’ll want to skip the calls to `df.auto.head()` and
`df.auto.describe()`. To do this, edit each cell and select *Skip Cell* from the
*Cell type* pull down menu.

When you’ve done this successfully, your `read_data` step will look something
like the figure below.

![read data step with skips](images/read_data-skips.png)
{: style="display: block; margin: auto; width:80%"}

