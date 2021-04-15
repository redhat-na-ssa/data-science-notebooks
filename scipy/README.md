# SciPy Examples

## Requirments

A Python 3.6 environment

```
$ python3 -m venv scipy-demos
$ source scipy-demos/bin/activate
$ pip install pip --upgrade
$ pip install -r requirements.txt
```

### Running the notebook server.

```
$ jupyter nbextension enable --py widgetsnbextension
$ jupyter lab --ip=0.0.0.0
```

If running on OpenShift, the Jupyter notebook image needs to
be configured the same as above.

