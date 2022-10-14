---
title: Tabs test
description: Testing the new tabs feature on dev
---
# Tabs test

## Page tabs

A tab is a clickable area at the top of a section that shows different content. When a tab is clicked, the tab's contents are shown, and the contents of other tabs is hidden. You can add multiple sets of tabs within a page. Note that users cannot use in-page search (Ctrl+F/Cmd+F) to locate content within tabs that are not displayed.

**Tab syntax**

```
>[!TABS START]

>[!TAB iOS]

This content appears in the iOS tab.

>[!TAB iOS]

This content appears in the Android tab.

>[!TAB Windows]

This content appears in the Windows tab.

>[!TAB MacOS]

This content appears in the MacOS tab.

>[!TAB Linux]

This content appears in the Linux tab.

>[!TABS END]
```

**Rendered**

>[!TABS START]

>[!TAB iOS]

This content appears in the iOS tab.

>[!TAB iOS]

This content appears in the Android tab.

>[!TAB Windows]

This content appears in the Windows tab.

>[!TAB MacOS]

This content appears in the MacOS tab.

>[!TAB Linux]

This content appears in the Linux tab.

>[!TABS END]

## Objectives

* Create Content Fragment Models.
* Add tab placeholders, date and time, JSON objects, fragment references, and content references to the models.
* Add validation to content references.
