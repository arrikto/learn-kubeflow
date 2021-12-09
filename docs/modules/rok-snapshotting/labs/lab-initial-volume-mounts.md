# Lab: Initial Volume Mounts
Before the Kubeflow Pipeline run starts, Rok takes a snapshot of the workspace
and data volume. Then, it clones these snapshots to create new volumes that the
pipeline steps will use. The initial clones of the workspace volume and data
volume are mounted to each of the containers that are created to process the
Kubeflow pipeline steps.

## Requirements
You can identify where these volumes are mounted by reviewing the pipeline steps.

Review the pipeline step `clean_data` to identify where the volumes are mounted. 

## Solution

??? success "View Solution"

      The volumes will be mounted to the /home/jovyan directory, with sub directories created for the data volumes. 
