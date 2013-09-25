# Python

This document cover good practices in Python.

## Syntax

Syntax good-practices.

### Flake8

Ever run flake8 in your code to check for bad syntax, anti-patterns, cyclomatic
complexity. To run flake8 in your project run:

```
flake8 .
```

### Too long line

A line is too long when has more than 119 characters. To check for this using
flake8 run this:

```
flake8 . --max-line-length=120
```

### Escaping new line

Never use '\' to escape newline. If you accidently add a space between escape
character and newline, you will waste a few hours to find why your code is broken.

```python
from foo import bar, \
foobar
```

Group all imports with paratheses

```python
from foo import (
    bar,
    foobar
)
```
