---
title: Markdown preview issues
description: Markdown preview issues
---
# Markdown preview issues in VSC extension

## Strings without blank lines around are merged into single string

When you view this in preview, lines not separated by blank spaces are united into the same line. When rendered, each line remains separate. (I believe this rendering rule has been modified; it's hard to tell, since the guidance has always been to add blank lines between entities.)

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

## Badges in inline code blocks rendered in HTML

Specify the badge information on its own line or in a heading, table, or other page element. 

Here's the syntax for an inline badge with a beta label, blue color, URL, and tooltip:

`[!BADGE Beta]{type=Informative url="https://www.example.com" tooltip="Go to example.com"}`

