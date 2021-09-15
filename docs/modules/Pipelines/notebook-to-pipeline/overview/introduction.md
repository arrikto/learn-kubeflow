# Introduction

When first learning to use Kubeflow, you will probably want to adapt one or
more existing Python scripts or Jupyter notebooks so that they can be deployed
as a Kubeflow pipeline. In this module we will prepare you to define Kubeflow
pipelines based on existing code or from scratch as you develop new models.

Because it’s the simplest way to get started, we will use MiniKF as our
Kubeflow environment. We’ll teach you how to organize and annotate cells in a
Jupyter Notebook to define a Kubeflow pipeline that will run on a Kubernetes
cluster. This does not require any specialized knowledge of Kubernetes.
Instead, we’ll use the open-source Kale JupyterLab extension.