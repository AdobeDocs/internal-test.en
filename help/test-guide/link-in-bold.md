---
title: Link wrapped in bold
description: UGP-11630 link in bold have problems
exl-id: 2008a43a-5bca-4509-a52f-6ffd79c49c1c
---
# Link wrapped in bold

Problem syntax

`1. Navigate to the [**Sites** console](highlight.md).`

When rendered, only "console" is a hyperlink.

Rendered

1. Navigate to the [**Sites** console](highlight.md).

## Other example

Syntax:

```
_prefix text ![AdobeAnalytics](assets/package.png) suffix test_

**prefix text ![AdobeAnalytics](assets/package.png) suffix test**
```

Rendered:

_prefix text ![AdobeAnalytics](assets/package.png) suffix test_

**prefix text ![AdobeAnalytics](assets/package.png) suffix test**

## Bonus - Image wrapped in bold

`Not bold ok **Click the Adobe logo ![bluff](assets/package.png) to activate your subscription** not bold again`

Not bold ok **Click the Adobe logo ![bluff](assets/package.png) to activate your subscription** not bold again
