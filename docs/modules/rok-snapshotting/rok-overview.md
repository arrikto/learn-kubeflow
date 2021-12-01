# Rok Overview
Rok is an incredibly powerful technology which addresses several enterprise MLOps and Data Science use cases. Before we begin our technical education make sure you understand all the ways that Rok can be used and all the use cases that it can address.

## Environment Reproducibility
<div style="padding:75% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/649555197?h=1b39afd014&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Rok Use Cases - Environment Repro.mov"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

Much of the data being used for Machine Learning and Data Science training, testing, validation and production forecasting resides in a data lake. Unfortunately these are often cycling data and after a long period of time the data may morph or change. As a result you may not be able to come back to the environment and reproduce a specific execution data or data load. Being able to recreate an immutable snapshot is really important for a variety of industries that need this ability to "go back in time". For example a healthcare AI algorithm may turn down someone and an audit to confirm the model is per policy may require looking at the data that the model was trained on. If this model is several years old, then restoring all the data may be challenging, or impossible. With Rok however snapshots can quickly be loaded to reproduce the exact scenario, including the configuration of the containers and Pods, under which the model was trained. Additionally a company may have new data scientists join and others depart. Having reproducibility allows new hires to see the exact scenario under which prior data scientists did their modeling. This reproducibility is also critical for debuggability since you can quickly load the training scenario for the model and its artifacts. This reproducibility is powerful and necessary to maintain business stability.

## Model Portability w/ Authentication
<div style="padding:75% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/649556861?h=0e65c9a537&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Rok Use Cases - Portability.mov"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

Model development can occur on a local machine, on a virtual machine or in some other type of development environment. The many different environments that model development can take place in do not have consistent or shared data storage. In fact data storage is often in silos. With Rok and Rok Registry you can move models across environments with the relevant data. You can even subscribe to the models of your colleagues or have them subscribe to yours. Rok Registry subscriptions have access controls so that management or access to models is dependent on authentication.

## Functionality & Performance Improvements
<div style="padding:75% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/649558608?h=6b34601124&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Rok Use Cases - Functionality &amp;amp; Performance.mov"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

You can take advantage of the Rok Storage Class and use it for Kubeflow to take advantage of streamlined ML workflows along with significant performance and cost infrastructure benefits. This includes easy Pod restarts across availability zones in AWS / GCP. Additionally with Kale and Rok and the Multiple Read Write volumes you can run multiple steps on multiple different nodes and distribute the whole training and workload across the nodes and can maintain dependencies across these steps and nodes. This is also backed by pipeline step caching which further improves performance and reduces cost.

## Additional Exploration
Additional areas to explore once you complete your Rok 101 education are:

- Streamlined ML Pipeline building with automatic versioning 
- Kale & Rok with hyperparameter tuning
- Kale & Rok automate and deploy model inference server faster
- Integrated Data Management for the complete DS environment.
- Ability to deploy a TensorBoard server from a Rok-backed artifact
- AutoML made easy with Kale & Rok
