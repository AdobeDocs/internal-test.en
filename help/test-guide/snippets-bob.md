---
title: Bob's snippets test
description: Dunno what to say {{__meta_homepage}}
homepage: /help/test-guide/toc-overview.md
color: Purple
exl-id: fd3ca9be-734d-4a5d-a423-60b9538af424
---
# {{__meta_title}}

## Include example

`{{$include /help/_includes/bob-includes.md}}`

Above rendered:

{{$include /help/_includes/bob-includes.md}}

## Snippets

**Metadata references**

`The home page is [here]({{__meta_homepage}})`

Above rendered:

The home page is [here]({{__meta_homepage}})

`{{__meta_description}}`

Above rendered:

{{__meta_description}}

**Snippets references**

These link to snippets.md file in root repo.

`{{long}}`

Above rendered:

{{long}}

`{{audience}}`

Above rendered:

{{audience}}

`{{obsidion}}`

Above rendered:

{{obsidion}}

`{{image}}`

Above rendered:

{{image}}

`{{color}}`

Above rendered:

{{color}}

`{{bigblock}}`

Above rendered:

{{bigblock}}

`{{html}}`

Above rendered:

{{html}}

## Snippets in comments and code blocks

<!--
This is {{__meta_description}}
-->

```
img dev ref
{{__meta_description}}
var=numbot
```
