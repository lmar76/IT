# Kernels

## Create a new Python kernel

Requirements for the specific environment:
```
ipykernel
```

Activate the environment:

```
conda activate myenv
```

Create the new Python kernel:

```
python -m ipykernel install --name <name> --display-name "<long name>" --sys-prefix
```

## List and manage kernels

Activate the environment for which you want to manahe kernels, e.g. the one used to start JupyterLab:

```
conda activate jupyter
```

Listing and managing kernels:

```
jupyter kernelspec command [args]
```


