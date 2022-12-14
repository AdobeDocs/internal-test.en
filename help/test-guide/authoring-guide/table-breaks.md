---
title: Table breaks
description: Test of different table breaks
exl-id: 85c8e8c6-5333-4a94-b5d6-1bf018bbd3ce
---
# Table breaks 

## Standard markdown table with `<br>`

**FIXED `Green<br>Red<br>Blue`**

|  | Number | Colors |
|---|---|---|
| Juanya | 17 | Green<br>Red<br>Blue |
| Maria | 23 | Yellow<br>Brown |

{style="table-layout:fixed"}

**AUTO `Green<br>Red<br>Blue`**

|  | Number | Colors |
|---|---|---|
| Juanya | 17 | Green<br>Red<br>Blue |
| Maria | 23 | Yellow<br>Brown |

{style="table-layout:auto"}

## Markdown table with double `<br>`s

**FIXED `Green<br><br>Red<br><br>Blue`**

|  | Number | Colors |
|---|---|---|
| Juanya | 17 | Green<br><br>Red<br><br>Blue |
| Maria | 23 | Yellow<br><br>Brown |

{style="table-layout:fixed"}

**AUTO `Green<br><br>Red<br><br>Blue`**

|  | Number | Colors |
|---|---|---|
| Juanya | 17 | Green<br><br>Red<br><br>Blue |
| Maria | 23 | Yellow<br><br>Brown |

{style="table-layout:auto"}

## Markdown table with `<p>`

**FIXED `Green<p>Red<p>Blue`**

|  | Number | Colors |
|---|---|---|
| Juanya | 17 | Green<p>Red<p>Blue |
| Maria | 23 | Yellow<p>Brown |

{style="table-layout:fixed"}

**AUTO `Green<p>Red<p>Blue`**

|  | Number | Colors |
|---|---|---|
| Juanya | 17 | Green<p>Red<p>Blue |
| Maria | 23 | Yellow<p>Brown |

{style="table-layout:auto"}

|  | Number | Colors |
|---|---|---|
| Juanya | 17 | This is the color **green** and it is meant to wrap to a different line as a matter and or means of testing aforesaid paragraph breaks. <p>This is the color **red** and it is meant to wrap to a different line as a matter and or means of testing aforesaid paragraph breaks. <p>This is the color **blue** and it is meant to wrap to a different line as a matter and or means of testing aforesaid paragraph breaks.  |
| Maria | 23 | Yellow<p>Brown |

{style="table-layout:fixed"}

|  | Number | Colors |
|---|---|---|
| Juanya | 17 | This is the color **green** and it is meant to wrap to a different line as a matter and or means of testing aforesaid paragraph breaks. <p>This is the color **red** and it is meant to wrap to a different line as a matter and or means of testing aforesaid paragraph breaks. <p>This is the color **blue** and it is meant to wrap to a different line as a matter and or means of testing aforesaid paragraph breaks.  |
| Maria | 23 | Yellow<p>Brown |

{style="table-layout:auto"}
