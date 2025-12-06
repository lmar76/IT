# WGET usage examples

## Download data from explicit FTPS server

```sh
wget --ftp-user USER --ask-password ftps://HOST/PATH
```

## Download data from implicit FTPS server

```sh
wget --ftp-user USER --ask-password --ftps-implicit ftps://HOST/PATH
```

## HTTP mirroring

```sh
wget --http-user=USER nv -o LOGFILE --mirror -L --limit-rate=<rate> --http-user=USER --http-passwd=<password> <url>
```

## FTP mirroring

```sh
wget --ftp-user USER --ask-password -nv -nH -m ftp://OST/PATH
```
