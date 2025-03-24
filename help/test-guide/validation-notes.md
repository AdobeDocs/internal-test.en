---
title: Validation issues between steps
description: Validation issues between steps UGP-11842
solution: Campaign, Campaign v8
version: Campaign v8
exl-id: 2ff03088-7692-44f4-8aee-017d589420f1
---
# Validation for extra lines between steps

**No blank lines before/after note**

1. This is step 1.
   >[!NOTE]
   >
   >This is a note.
1. This is step 2.
1. This is step 3.

**Yes blank lines before/after note**

1. This is step 1.

   >[!NOTE]
   >
   >This is a note.

1. This is step 2.
1. This is step 3.

**No blank lines before/after image**

1. This is step 1.
   ![image](assets/android.png)
1. This is step 2.
1. This is step 3.

**Yes blank lines before/after image**

1. This is step 1.

   ![image](assets/android.png)

1. This is step 2.
1. This is step 3.

**No blank lines before/after bullet list**

1. This is step 1.
   * Bullet 1
   * Bullet 2
   * Bullet 3
1. This is step 2.
1. This is step 3.

**Yes blank lines before/after bullet list**

1. This is step 1.

   * Bullet 1
   * Bullet 2
   * Bullet 3

1. This is step 2.
1. This is step 3.

<!--
**No blank lines before/after shade box**

1. This is step 1.
   >[!BEGINSHADEBOX]

   There should be a shadebox component here

   >[!ENDSHADEBOX]
1. This is step 2.
1. This is step 3.

**Yes blank lines before/after shade box**

1. This is step 1.

   >[!BEGINSHADEBOX]

   There should be a shadebox component here

   >[!ENDSHADEBOX]

1. This is step 2.
1. This is step 3.
-->
