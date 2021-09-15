# Working Example

## Scenario

Throughout the rest of this module, we’ll be working with a prediction use
case. This type of challenge is common in data science work, but regardless
of your use case, working through this example will teach you what you need
to know to adapt your own code for orchestration as a Kubeflow pipeline in a
Kubernetes cluster. 

We’ve adapted our example from the Car Price Prediction dataset on Kaggle.

We’ll take on the role of a data scientist consulting with a Chinese automobile
company called Geely Auto. Geely aspires to enter the US market by setting up a
manufacturing unit in the US and producing cars locally to be able to compete
with US and European auto manufacturers.

Geely has contracted with our consulting company to understand the factors on
which the pricing of cars depends. Specifically, they want to understand the
factors affecting the pricing of cars in the American market, since those may be
very different from the Chinese market. The company wants to know:

- Which variables are significant in predicting the price of a car?
- How well those variables describe the price of a car?

We are required to model the price of cars with the available independent
variables. 

This will be used by Geely’s management to understand how exactly the prices
vary with the independent variables. 

They can accordingly design cars and the business strategy etc. to meet certain
price levels. 

Further, the model will be a good way for management to understand the pricing
dynamics of a new market.

Based on various market surveys, our hypothetical consulting firm has gathered
a dataset of different types of cars across the US market. The dataset includes
over 200 cars, their prices, and 24 automobile features that we will analyze as
independent variables.

See the [handouts](/assets/learn_kubeflow_pipelines_handouts.zip) for a data
dictionary listing the automobile features and their descriptions.

## Main sections in our notebook

Our example notebook follows a common workflow for prediction and other types
of data science problems. The main sections are as follows.

### Read and clean data

First we find sections on reading and cleaning data.

![reading and cleaning data sections](/images/image61.png){: style="display: block; margin: auto; width:80%"}

Most data science workflows will include these steps. Depending on your dataset
and use case they might be complex, relatively simple, or somewhere in between.
Think of these sections in this notebook as representative of read and clean
steps for any workflow.


### Visualize and analyze data

Following the cleaning section, there is a fairly long section of data analysis
looking at a few distributions and how the independent variables are correlated
with price.

As with reading and cleaning data, such sections are common to most data
science notebooks. Again, think of these as representative of analysis steps
for any workflow.

![visualize engine variables](/images/image52.png){: style="display: block; margin: auto; width:80%"}

### Prepare data, build models, and evaluate

Finally, as we move toward the end of our example notebook, we see sections for
data preparation, model building, and model evaluation. 

![visualize engine variables](/images/image44.png){: style="display: block; margin: auto; width:80%"}

In this notebook, the model building and evaluation run together in the same
cells as they often do when one is developing a model.

![build models](/images/image64.png){: style="display: block; margin: auto; width:80%"}

