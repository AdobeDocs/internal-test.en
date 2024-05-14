---
title: Markdown extension issues
description: Markdown extension issues
---
# Mardown extension issues

## Strings without blank lines around are merged into single string

Syntax:

>[!NOTE]
>
>Escaping characters in the metadata section requires a different approach than escaping markdown syntax. The metadata section at the top of the document uses YAML format, which has different rules.
>
>As a rule of thumb, if you add special characters such as a colon or a `[` at the start of the value, add parentheses around the metadata value like this:
>
>`---`
>`title: "Processing rules: A new beginning"`
>`---`

string1
string2
string3

`[!NOTE]`
`[!TIP]`
`[!IMPORTANT]`
`[!WARNING]`
`[!CAUTION]`
`[!ADMIN]`
`[!AVAILABILITY]`
`[!PREREQUISITES]`
`[!INFO]`
`[!ERROR]`
`[!SUCCESS]`
`[!MORELIKETHIS]`


