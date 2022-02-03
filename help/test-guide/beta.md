---
title: Beta tags
description: Description
exl-id: 747ade98-26f9-40b8-80b0-354e516a6231
---
# Beta Tags

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

This is the [!__BETA_CTA CTA Test](https://www.adobe.com).  And  [!__BETA_CTA CTA Test](https://www.adobe.com)

```
This is the [!__BETA_CTA CTA Test](https://www.adobe.com)
```

Foo

## Accordion POC

>[!__BETA_ACCORDIAN Fluffer]
>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula
>eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient
>montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque
>eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
>fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut,
>imperdiet a, venenatis vitae, justo. Nullam dictum felis eu pede mollis pretium.
>Integer **tincidunt**. Cras dapibus. Vivamus elementum semper nisi. Aenean vulputate
>eleifend tellus. Aenean leo ligula, porttitor eu, consequat vitae, eleifend ac,
>enim. Aliquam ante, dapibus in, viverra quis, feugiat a, tellus. Phaselus>viverra nulla ut metus varius laoreet. Quisque rutrum. Aenean imperdiet. Etiam
>ultricies nisi vel augue. Curabitur ullamcorper ultricies nisi. Nam eget dui.
>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula


>[!__BETA_ACCORDIAN Poof!]
>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula
>eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient
>montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque


## Tabs

Anim aute ex elit qui duis qui et pariatur cillum nisi Lorem fugiat amet. Aliquip duis ut laborum tempor. Cupidatat velit est dolor fugiat Lorem ipsum velit ex velit mollit. Ut laborum cupidatat mollit eiusmod in sunt reprehenderit quis sunt irure consectetur et ex Lorem. Lorem anim laboris mollit id labore dolore.

### Hello World in different languages

>[!__BETA_TABS START]

>[!__BETA_TAB Javascript]

Simple one-liner:

```javascript
console.log('Hello World!')
```

>[!__BETA_TAB Python]

>[!NOTE]
>Easy Peasy!

```python{line-numbers    wrap }
print('Hello World\n')
```

>[!__BETA_TABS END]
