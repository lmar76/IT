# Python 3.9 in RedHat Enterprise Linux 8.x

Install `python39`:

```sh
dnf install python39
```

Update `alternatives`:

```sh
alternatives --set python3 /usr/bin/python3.9
```

Check `python3` entry in the `alternatives`:

```sh
alternatives --list
```
