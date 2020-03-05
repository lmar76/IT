# `unittest.mock`

## Mocking `os.walk`

Example:

```python
import os
from unittest import mock


def other_function(start):
	for root, dirs, files in os.walk(start):
		print((root, dirs, files))


with mock.patch('os.walk') as mock_os_walk:
	mock_os_walk.return_value = ((1, 2, 3), (4, 5, 6), (7, 8, 9))
	other_function('.')
```
