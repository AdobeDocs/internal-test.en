---
title: Beta tags change 2
description: Description
exl-id: 2d7aa048-b36e-4b31-a566-ed0270246a35
---
# Beta Tags

Matt was here

## Line Numbers in Code Blocks

```markdown
'''python{line-numbers}
<code here>
'''
```

```python{line-numbers}
    # first process codeblocks
    for idx, line in enumerate(mdlines):
        if line.count('<!--') > 0 and not incodeblock:
            incomment = not incomment
        if line.count('-->') > 0 and not incodeblock:
            incomment = not incomment
            leavingcomment = True

        if line.count('&#96;&#96;&#96;') == 1:  # on a fence
            incodeblock = not incodeblock
            if not incodeblock:
                leavingcodeblock = True
            onfence = True
        else:
            onfence = False

        # open fence: &#96;&#96;&#96;language{option option}

        if onfence and not leavingcodeblock:
            language = line.strip('`').split('{')[0]
            options = line.replace('&#96;&#96;&#96;' + language, '').replace('{', '').replace('}', '').split()
            prismopts = ''
            mdlines[idx] = '&#96;&#96;&#96;' + language
            for option in options:
                opt = option.strip().split('=')[0]
                if opt == 'line-numbers':
                    prismopts = 'class="line-numbers"'
                    needenddivcode = True
            if prismopts:
                mdlines[idx] = '<style>\npre {\n  line-height: 1 !important;\n}\n</style>\n' + mdlines[idx]
            print(':', idx, line, language, options, 'div' in mdlines[idx])

```


<!-- </div> -->

## CTA

```
This is the [!__BETA_CTA CTA Test](https://www.adobe.com)
```

Foo


## Tabs

Anim aute ex elit qui duis qui et pariatur cillum nisi Lorem fugiat amet. Aliquip duis ut laborum tempor. Cupidatat velit est dolor fugiat Lorem ipsum velit ex velit mollit. Ut laborum cupidatat mollit eiusmod in sunt reprehenderit quis sunt irure consectetur et ex Lorem. Lorem anim laboris mollit id labore dolore.

### Hello World in different languages

Simple one-liner:

```javascript
console.log('Hello World!')
```

>[!NOTE]
>Easy Peasy!

```python{line-numbers    wrap }
print('Hello World\n')
```
