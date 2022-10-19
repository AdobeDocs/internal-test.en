---
title: Code block highlighting
description: Testing code blocks with numbering and highlighting
---
# Code blocks

Testing highlighting within code blocks.

## Different start line

`js line-numbers="true" start-line="6"`

```js line-numbers="true" start-line="6"  
  line 1, the first
  line 2
  line 3
  line 4
  line 5
  line 6
  line 7
  line 8
  line 9
  line 10
  line 11
  line 12
  line 13
  line 14
  line 15
  line 16
  line 17
  line 18
  line 19
  line 20
```

## Highlighting only

`js line-numbers="true" highlight="4-10, 16"`

```js line-numbers="true" highlight="4-10, 16"  
  line 1, the first
  line 2
  line 3
  line 4
  line 5
  line 6
  line 7
  line 8
  line 9
  line 10
  line 11
  line 12
  line 13
  line 14
  line 15
  line 16
  line 17
  line 18
  line 19
  line 20
```

## Highlighting and start line (good)

`js line-numbers="true" start-line="3" highlight="4-10, 16"`

```js line-numbers="true" start-line="3" highlight="4-10, 16"  
  line 1, the first
  line 2
  line 3
  line 4
  line 5
  line 6
  line 7
  line 8
  line 9
  line 10
  line 11
  line 12
  line 13
  line 14
  line 15
  line 16
  line 17
  line 18
  line 19
  line 20
```

## Highlighting and start line (overshoot)

`js line-numbers="true" start-line="7" highlight="9-14, 26"`

```js line-numbers="true" start-line="7" highlight="9-14, 26"  
  line 1, the first
  line 2
  line 3
  line 4
  line 5
  line 6
  line 7
  line 8
  line 9
  line 10
  line 11
  line 12
  line 13
  line 14
  line 15
  line 16
  line 17
  line 18
  line 19
  line 20
```

## Standard test

```python line-numbers="true"
# Python code to demonstrate the working of
# random() and seed()
 
# importing "random" for random operations
import random
 
# using random() to generate a random number
# between 0 and 1
print("A random number between 0 and 1 is : ", end="")
print(random.random())
 
# using seed() to seed a random number
random.seed(5)
 
# printing mapped random number
print("The mapped random number with 5 is : ", end="")
print(random.random())
 
# using seed() to seed different random number
random.seed(7)
 
# printing mapped random number
print("The mapped random number with 7 is : ", end="")
print(random.random())
 
# using seed() to seed to 5 again
random.seed(5)
 
# printing mapped random number
print("The mapped random number with 5 is : ", end="")
print(random.random())
 
# using seed() to seed to 7 again
random.seed(7)
 
# printing mapped random number
print("The mapped random number with 7 is : ", end="")
print(random.random())
```
