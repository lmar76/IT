# Connect to a FTP server using SSL

```
curl -v -u user --ssl-reqd ftp://hostname/
```

In case of self-signed certificate, add option `-k` or `--insecure` to not check the certificate.
