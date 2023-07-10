---
title: Highlight test
description: Highlight test
---

# Highlight test

This has span only, not div, which renders badly.

## Paragraph and sentence

<span class="preview">This entire paragraph should be highlighted. The way we currently highlight text is to add tags. This word is **bold**. And this is just the last sentence.</span>

This entire paragraph should NOT be highlighted. <span class="preview"> This word is **bold** inside a highlighted sentence.</span> And this is just the last sentence.

## Block of paragraphs (div)

<div class="preview">This entire set of paragraphs should be highlighted. 

The way we currently highlight text is to add tags. This word is **bold**. 

And this is just the last sentence.</div>

## Block of components (div)

Ok, so this sentence is not part of highlighting.

<div class="preview">

Highlighting begins here.

![image](assets/adobe-logo-old.png)
![image](assets/adobe—logo.png)

That was an image. Let's try a table.

|  | Number | Colors |
|---|---|---|
| Juanya | 17 | Green<br>Red<br>Blue |
| Maria | 23 | Yellow<br>Brown |

And now a note.

>[!NOTE]
>
>This is a note.

Last paragraph in highlighting.

</div>

Text outside the section.

## Highlighting that includes a heading


<div class="preview">

### Highlighting begins above this line

This is a paragraph.

</div>

Highlighting ends above this line

## Tables

<table style="table-layout:auto">
<tbody> 
  <tr> 
  <td>Data structure name</td> 
  <td> <p> Enter a name for the new data structure.</p> </td> 
  </tr> 
  <tr> 
  <td> <p>Specification</p> </td> 
  <td> <p>Do one of the following to set up your data store's columns.</p> 
    <ul> 
    <li> <p>Click <strong>Add item</strong> to specify the properties of one column manually.</p> <p>Enter the <strong>Name</strong> and <strong>Type</strong> for the data store column and define corresponding properties.</p> </li> 
    <li> <p>Click <strong>Generator</strong> to determine the columns from the sample data you provide.</p> 
    <div class="preview">
     <b>Example: </b> 
      <p>For example, the following JSON sample data creates three columns: name, age, and phone number. Phone number is a collection of mobile and landline phone numbers.</p> 
      <p><code>{</code> </p> 
      <p><code>"name":"John",</code> </p> 
      <p><code>"age":30,</code> </p> 
      <p><code>"phone number": {</code> </p> 
      <p><code>"mobile":"987654321",</code> </p> 
      <p><code>"landline":"123456789"</code> </p> 
      <p><code>}</code> </p> 
      <p><code>}</code> </p> 
      <p>The empty columns in the data store view:</p> 
      <p>You can then add values to the data store manually or by using the Workfront Fusion data store modules.</p> 
    </div> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
  <td>Strict </td> 
  <td> <p>Enable this option to ensure that the payload matches the data structures. Payloads that contain extra items not specified in the data structure are rejected.</p> </td> 
  </tr> 
  </tbody> 
</table>

## Highlighting in notes

>[!CAUTION]
>
><div class="preview">**This object is hot.**
>
>Very hot.</div>
