---
title: badges
description: This is the article overview.
badge: "Beta Content"
badge-before-title: true
badge-color: negative
badge-url: https://www.adobe.com
badge-tooltip: Yes!
---
# We don't need no ***REMOVED***in' badges!


[!BADGE Unreleased]{type=Negative}


|Label|Badge|
|---|---|
|Unreleased|[!BADGE Unreleased]{type=Negative url="https://www.example.com"}|
|Sunset|[!BADGE End-of-life]{type=Positive url="https://www.example.com" tooltip="Example!"}|
|Discontinued|[!BADGE Discontinued]{type=Negative tooltip="foo"}|
|Current|[!BADGE Latest Version]{type=Informative}|


## SCCM Markdown

[!BADGE Neutral]{type=Neutral} [!BADGE Informative]{type=Informative} [!BADGE Positive]{type=Positive} [!BADGE Negative]{type=Negative}

## Bob Documentation

```
|Type|Badge|
|---|---|
|Informative (default)|[!BADGE Beta]{type=Informative url="https://www.example.com"}|
|Positive|[!BADGE New Feature]{type=Positive url="https://www.example.com" tooltip="Go to example.com"}|
|Negative|[!BADGE Discontinued]{type=Negative tooltip="This feature is now end of life"}|
|Neutral|[!BADGE Note]{type=Informative tooltip="This information is neither good nor bad."}|
|Caution|[!BADGE Attention]{type=Caution} tooltip="Yellow status"|
```

|Type|Badge|
|---|---|
|Informative (default)|[!BADGE Beta]{type=Informative url="https://www.example.com"}|
|Positive|[!BADGE New Feature]{type=Positive url="https://www.example.com" tooltip="Go to example.com"}|
|Negative|[!BADGE Discontinued]{type=Negative tooltip="This feature is now end of life"}|
|Neutral|[!BADGE Note]{type=Informative tooltip="This information is neither good nor bad."}|
|Caution|[!BADGE Attention]{type=Caution tooltip="Yellow status"}|

## [!BADGE Heading]{type=Positive tooltip="Badge in heading"} Badge in heading

I added `## [!BADGE Heading]{type=Positive tooltip="Badge in heading"} Badge in heading` as a heading. Test.

## Spectrum HTML


From spectrum docs:

<div style="display: flex; gap: var(--spectrum-global-dimension-size-50);">
    <sp-badge variant="neutral">Neutral</sp-badge>
    <sp-badge variant="informative">Informative</sp-badge>
    <sp-badge variant="positive">Positive</sp-badge>
    <sp-badge variant="negative">Negative</sp-badge>
</div>

Markdown source for this page:

```markdown
---
title: badges
description: This is the article overview.
badge: "Beta Content"
badge-before-title: false
badge-type: negative
badge-url: https://www.adobe.com
badge-tooltip: Yes!
badge2: "Alpha Content"
badge2-before-title: false
badge2-type: positive
badge2-url: https://www.example.com
badge2-tooltip: no!
---
# We don't need no ***REMOVED***in' badges!


[!BADGE Unreleased]{type=Negative}


|Label|Badge|
|---|---|
|Unreleased|[!BADGE Unreleased]{type=Negative url="https://www.example.com"}|
|Sunset|[!BADGE End-of-life]{type=Positive url="https://www.example.com" tooltip="Example!"}|
|Discontinued|[!BADGE Discontinued]{type=Negative tooltip="foo"}|
|Current|[!BADGE Latest Version]{type=Informative}|


## SCCM Markdown

[!BADGE Neutral]{type=Neutral} [!BADGE Informative]{type=Informative} [!BADGE Positive]{type=Positive} [!BADGE Negative]{type=Negative}

## Spectrum HTML


From spectrum docs:

<div style="display: flex; gap: var(--spectrum-global-dimension-size-50);">
    <sp-badge variant="neutral">Neutral</sp-badge>
    <sp-badge variant="informative">Informative</sp-badge>
    <sp-badge variant="positive">Positive</sp-badge>
    <sp-badge variant="negative">Negative</sp-badge>
</div>
```