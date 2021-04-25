# Tensorflow/Keras examples

`01-cifar-10.ipynb` - Transfer learning ResNet architecture using the cifar10 data set. This notebook requires a GPU. When running on Open Data Hub the Jupyter notebook
persistent volume may need to be increased above 2GB. I'm still testing this. The notebook should take about 9 minutes to run on an nvidia T4 GPU. 

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