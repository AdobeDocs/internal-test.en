---
title: Overview
description: This is the article overview.
---
# Code Highlighting a line

## ```python {line-numbers="true" start-line="20" highlight="24-27,31"}```

* `line-numbers="true"`: Turn on line numbers
* `start-line="20"`: Start line numbers with 20 (not 1).  Can be negative: `-5`
* `highlight="24-27,31"`: High light lines 24, 25, 26, 27, 31 based on `start-line` offset.

```python {line-numbers="true" start-line="20" highlight="24-27,31"}
foo = 12

print(f'foo is {foo}'

def fun():
    # This is a function definition

    print('Hello from Fun!')

# This is global again

foo = foo + 12

print(f'foo is now {foo}.')
```
