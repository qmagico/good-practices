===============
Escaping new line
===============

Never use '\' to escape newline. If you accidently add a space between escape character and newline, you will waste a few hours to find why your code is broken.

```
from foo import bar, \
foobar
```

Group all imports with paratheses

```
from foo import (
    bar,
    foobar
)
```
