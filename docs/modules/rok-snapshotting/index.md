# **Rok 101**: Snapshotting and Restoring Kubeflow Pipelines

## Course Summary
When deploying Kubeflow production environments, you will want to snapshot your
notebooks, pipelines, and volumes so that you can rapidly restore environments
or specific Kubeflow pipeline steps. We’ll teach you how Rok takes snapshots,
how to restore snapshots, and how to manage the volumes in the Kubernetes Pods.
Because it’s the simplest way to get started, we will use MiniKF as our
Kubeflow environment.

We are assuming that you know how to organize and annotate cells in a Jupyter
Notebook to define a Kubeflow pipeline that will run on a Kubernetes cluster. If
you need a refresher on these skills, please review our [Kale 101
course](modules/notebook-to-pipeline/).

We are also assuming that you know how to use Katib to perform hyperparameter
tuning with Kubeflow Pipelines. If you need a refresher on these skills please
review our [Katib 101 course](modules/notebook-katib-tuning).
