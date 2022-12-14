# Kernels

## Create a new Python kernel

Activate the environment:

```
conda activate myenv
```

Create the new Python kernel:

```
python -m ipykernel install --name <name> --display-name "<long name>" --sys-prefix
```

## List and manage kernels

Activate the base environment:

```
conda activate base
```

Listing and managing kernels:

```
$ jupyter kernelspec command [args]
```


