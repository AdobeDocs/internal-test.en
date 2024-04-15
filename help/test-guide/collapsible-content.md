---
title: collapsible
description: Test of collapsible syntax
exl-id: 74319765-a930-44ef-b88d-a102d3a1d3c0
---
# Collapsible content

I'm tired and I just can't go on...

Let's start with a simple accordion.

> Play an accordian, go to jail.
>   - Starving Musician, Santa Cruz

+++Click me
Boo!
+++

## FAQ Use Case

+++What is collapsible content?
When a page is loaded, collapsible sections are hidden. The user can click the collapsible title to expand the section.
 +++

+++What's the difference between collapsible content and accordions?
According to the strict definition of the tools we're using, accordions can have only one section expanded at a time, whereas users can control collapsible content individually. But really, accordions and collapsible sections are interchangeable.
+++

+++When should collapsible content be used?
Examples:

* In a long list of Frequently Asked Questions, you might want to display only the questions to make it easier for users to scan the page. Then they can click the title of any question they're interested in.
* If a long procedure includes multiple sub-procedures, the set of steps can be unwieldy. You can hide these sub-procedures with something like a **Details** or **Steps** title that users can see. For example, if Step 3 is "Provide Maintainer access to the user," you could add a **Details** section that would give specific steps for assigning permissions.
* With inline images. Click a little inline image to display a different image. This might be a bad idea. I'm spitballing here.
+++

+++Are there drawbacks to using collapsible content?
In the past, page search (Ctrl/Cmd+F) failed to find hidden content, so collapsing an entire FAQ page for example might make it difficult for users to find what they're looking for.

While this page search problem still applies to Safari, Chrome users can find content within a page.

Page search is something to consider.
+++

+++What should I look out for with collapsible sections?

* Make sure that you add open and close syntax for each collapsible section. If you forget to close a section, validation won't catch it.
* While it's possible to include headings inside a collapsible section, it's not recommended.
* Make sure that images and notes inside a collapsible section include blank lines before and after. Validation DOES catch these errors.
+++

## Collapser with markdown

**Bullet list and image**

This is a bullet list.

* Bullet one
* Bullet two
  * two point five
* Bullet three

+++Click me
This is a bullet list.

* Bullet one
* Bullet two
  * two point five
* Bullet three

![logo](assets/adobe-logo-old.png)
+++

**Note**

+++Click me
This is text.

>[!NOTE]
>
>This is a simple note.

+++

## Numbered list

1. Do this.
1. Do that.

   +++Details
   Doing that requires the following:

   * Jello
   * Carrots
   * Pineapple
   +++

1. Do more.

## Nested in collapser

+++Details
Do the following:

1. Understand this.
1. Do this:

   +++Secret
   Life is short.
   +++

1. Last step.
+++

## Nested in note

>[!NOTE]
>
>This is a bad idea.
>
>+++Click me!
>I'm inside a note.
>+++

## Should not be rendered inside code block

```
copy con autoexec.bat
ren config.sys config.exe
+++Click here!
Let's hope I'm not collapsed.
+++
format c:
```

## Code block inside collapser

+++Click here...

Try this commands.

```
copy con autoexec.bat
ren config.sys config.exe
format c:
```

And scene.
+++

## Heading inside collapser

+++Important Section

## This is a heading

This is paragraph text.

+++
