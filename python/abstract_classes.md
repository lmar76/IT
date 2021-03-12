# Creation of abstract classes

## Creation of abstract classes using `abc`

```python
import abc

class BaseClass(abc.ABC):
    """Base class."""

    def __init__(self, value):
        self.value = value
    
    @abc.abstractmethod
    def meth(self):
        pass
```

`BaseClass` cannot be instantiated. E.g.:

```
> c = BaseClass(10)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: Can't instantiate abstract class BaseClass with abstract methods meth
```

`BaseClass` subclass:

```python
class DerivedClass(BaseClass):
    """Derived class."""

    def meth(self):
        return self.value ** 2
```

`DerivedClass` *can* be instantiated because implements abstract method `meth`. E.g.:

```
> c = DerivedClass(10)
> c.meth()
100
```
