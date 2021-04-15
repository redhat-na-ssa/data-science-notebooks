# SciPy Examples

## Requirements

### A local Python 3.6 environment

```
$ python3 -m venv scipy-demos
$ source scipy-demos/bin/activate
$ pip install pip --upgrade
$ pip install -r requirements.txt
```

#### Configuring and running the Jupyter notebook server.

```
$ jupyter nbextension enable --py widgetsnbextension
$ jupyter lab --ip=0.0.0.0
```

### OpenShift

If running on OpenShift, the Jupyter notebook image needs to
be configured the same as above.

### Run examples on Binder or Google Collab

[01-py-slicer](01-py-slicer.ipynb)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/redhat-naps-da/data-science-notebooks/main?filepath=scipy%2F01-py-slicer.ipynb)
[![Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/bkoz/52eaba19295bd4b96ea0daeeb062a607/slider.ipynb)

