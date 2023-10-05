# Download data from FTPS server

```
whet --user <username> --ask-password ftps://<host>/<path>
```

# HTTP mirroring

```
wget -nv -o <logfile> --mirror -L --limit-rate=<rate> --http-user=<username> --http-passwd=<password> <url>
```

# FTP mirroring

```sh
wget -nv --mirror -L ftp://<user>:<password>@<host>/
```
