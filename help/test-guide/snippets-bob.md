---
title: Bob's snippets test
description: Dunno what to say {{__meta_homepage}}
homepage: /help/test-guide/toc-overview.md
---
# {{__meta_title}}

## Include example

`{{$include /help/test-guide/bob-includes.md}}`

{{$include /help/test-guide/bob-includes.md}}

## Snippets

**Metadata references**

`The home page is [here]({{__meta_homepage}})`

The home page is [here]({{__meta_homepage}})

`{{__meta_description}}`

{{__meta_description}}

**Snippets references**

These link to snippets.md file in root repo.

`{{long}}`

{{long}}

`{{audience}}`

{{audience}}

`{{#obsidion}}`

{{#obsidion}}

## Snippets in comments and code blocks

<!--
This is {{__meta_description}}
-->

```
img dev ref
{{__meta_description}}
var=numbot
```
