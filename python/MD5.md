# Calculate MD5 sum of a file

```python
def md5sum(filename, bufsize=4096):
    with open(filename, 'rb') as f:
        m = hashlib.md5()
        while True:
            buffer = f.read(bufsize)
            if not buffer:
                break
            m.update(buffer)
    return  m.hexdigest()
```
