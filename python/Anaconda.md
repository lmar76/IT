# Environments

## Creating an environment from an environment.yml file

Run:

```
conda env create -f environment.yml
```

See [Creating an environment from an environment.yml file](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file).

## Exporting the environment.yml file

Activate the environment:

```
conda activate myenv
```

Export the environment:

```
conda env export -f environment.yml
```

The file will contain all the packages in the environment. To create the file with only the requested packages, run:

```
conda env export --from-history -f environment.yml
```

Use the `-c` option to add additional channels:

```
conda env export --from-history -c conda-forge -f environment.yml
```

See [Exporting the environment.yml file](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#exporting-the-environment-yml-file)

## Updating Anaconda environments

```
conda info --envs | awk '{ if ($1 != "#" && $1 != "") { print $1 } }' | while read env ; do conda update -n $env -y --all ; done
```

# Troubleshooting

## Installation

```
conda.exe: error while loading shared libraries: libz.so.1
```

See: https://stackoverflow.com/questions/60106630/conda-exe-error-while-loading-shared-libraries-libz-so-1

Usually the problem is due to the `noexec` flag set on `/tmp` in `/etc/fstab`. In this case:

```
mkdir /users/$USER/tmpconda
TMPDIR=/users/$USER/tmpconda bash Miniconda2-latest-Linux-x86_64.sh
```

