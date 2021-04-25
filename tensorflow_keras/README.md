# Tensorflow/Keras examples

[Tensor Flow Examples](https://github.com/tensorflow/docs.git)

=> docs/site/en/tutorials/keras/classification.ipynb

=> docs/site/en/tutorials/quickstart/beginner.ipynb

=> docs/site/en/tutorials/quickstart/advanced.ipynb

[Jason Dudash's Tensorflow demos](https://github.com/dudash/jupyter-gpu-examples)

Demos in this repo.

`01-cifar-10.ipynb` - Transfer learning ResNet architecture using the cifar10 data set. This notebook requires a GPU or it will take forever to run. When running on Open Data Hub the Jupyter notebook persistent volume may need to be increased above 2GB. The notebook should take about 9 minutes to run on an nvidia T4 GPU. 

#### OpenDataHub configuration

- Run Jupyter hub with a GPU.
- Choose the largest cpu/memory combo available based on the worker nodes.
- Storage for Jupyter hub defaults to 2Gi which may not suffice for many demos. There may be 2 ways to change this.
     - Change the config map and delete the old pvc.
       - Scale down the `jupyterhub` deployment config to 0 replicas. 
       - Edit the `jupyterhub-cfg` config map and increase the pvc size. 
       - Delete the `jupyterhub-nb-user-pvc` pvc.
       - Scale up `jupyterhub` deployment config. It should create a new pvc. 
    - Set the `SINGLEUSER_PVC_SIZE` environment variable when launching jupyter hub (not tested)