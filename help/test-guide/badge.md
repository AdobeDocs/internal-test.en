---
title: badges
description: This is the article overview.
badgeWeb: label="Campaign Web" url="https://www.example.com" type="Positive"
badge3: label="Premium" url="https://www.example.com" type="Neutral"
exl-id: 2d2c9c46-9338-4ef6-accf-77b8bb918af2
---
# Combining sprockets and widgets

Matt

In order to fancify a gizmo, you can combine the power of sprockets with the functionality of widgets.

## Badge with URL that opens in new window

[!BADGE Open in new tab]{type=Negative url="https://www.adobe.com newtab=true" tooltip="Open beta.md"}

## Examples

```
|Type|Badge|
|---|---|
|Informative (default)|[!BADGE Beta]{type=Informative url="https://www.example.com"}|
|Positive|[!BADGE New Feature]{type=Positive url="https://www.example.com" tooltip="Go to example.com"}|
|Negative|[!BADGE Discontinued]{type=Negative tooltip="This feature is now end of life"}|
|Neutral|[!BADGE Maybe]{type=Neutral tooltip="A rider fell off his horse..."}|
|Caution|[!BADGE Attention]{type=Caution} tooltip="Yellow status"|
```

|Type|Badge|
|---|---|
|Informative (default)|[!BADGE Beta]{type=Informative url="https://www.example.com"}|
|Positive|[!BADGE New Feature]{type=Positive url="https://www.example.com" tooltip="Go to example.com"}|
|Negative|[!BADGE Discontinued]{type=negative tooltip="This feature is now end of life"}|
|Neutral|[!BADGE Maybe]{type=Neutral tooltip="A rider fell off his horse..."}|
|Caution|[!BADGE Attention]{type=Caution tooltip="Yellow status"}|

## [!BADGE Beta]{type=Positive tooltip="Beta content"} More testing

The above heading should have a "Beta content" badge.

[!BADGE Open in new tab]{type=Negative url="https://www.adobe.com newtab=true" tooltip="Open adobe.com"}

|Label|Badge|
|---|---|
|Unreleased|[!BADGE Unreleased]{type=Negative url="https://www.example.com"}|
|Sunset|[!BADGE End-of-life]{type=Positive url="https://www.example.com" tooltip="Example!"}|
|Discontinued|[!BADGE Discontinued]{type=Negative tooltip="foo"}|
|Current|[!BADGE Latest Version]{type=Informative}|
|Inline badge with text in table|[!BADGE Inline table]{type=Informative} Stay tuned for more|

[!BADGE Inline paragraph]{type=Informative} Badges aren't really intended to be inline, but we should support it.

## Link testing

[!BADGE Relative link]{type=Negative url="beta.md newtab=true" tooltip="Open beta.md"}

[!BADGE Open in new tab]{type=Negative url="/help/test-guide/example-boxtext.md" tooltip="Open example boxtext"}

## SCCM Markdown

[!BADGE Neutral]{type=Neutral} [!BADGE Informative]{type=Informative} [!BADGE Positive]{type=Positive} [!BADGE Negative]{type=Negative}

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


## Understanding sprockets

[!BADGE Premium]{type=Informative url="https://www.example.com"}

In 1843, Eli McWilloughby was carrying piping hot metal from his forge. Thinking he was dipping the piece of metal into water in order to quench the steel, he instead dipped the flaming metal into a vat of acid.
