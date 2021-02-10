# HTTP mirroring

```sh
wget -nv -o logfile --mirror -L --limit-rate=rate --http-user=username --http-passwd=password url
```

# FTP mirroring

```sh
wget -nv --mirror -L ftp://user:password@host/
```
