# SciPy Examples

## Different ways to deploy

### 1) Run on Binder or Google Collab

[01-py-slicer](01-py-slicer.ipynb) - A NumPy tutorial that works with medical images.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/redhat-naps-da/data-science-notebooks/main?filepath=scipy%2F01-py-slicer.ipynb)
[![Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/bkoz/6c70b79a6c5bce2044379a682d8e32b6/slider.ipynb)

### 2) A local Python 3.8 environment

```
$ python3 -m venv scipy-demos
$ source scipy-demos/bin/activate
$ pip install pip --upgrade
$ pip install -r requirements.txt
```

Configure and run the Jupyter notebook server.

```
$ jupyter nbextension enable --py widgetsnbextension
$ jupyter lab --ip=0.0.0.0
```

### 3) On an OpenShift cluster

If running on OpenShift, the Jupyter notebook image needs to
be configured the same as above.


