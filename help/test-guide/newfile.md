---
title: New file
description: Description
cloud: nimbus
exl-id: a9476bf9-2b3a-4d5c-ab1c-cd5ffc71a43b
---

# New file

## Testing deep link

[Deep link explicit anchor](newfile.md#command-line)

[Deep link derived anchor](newfile.md#deep-link-from-bob)

testing webook

| A | B | C |
| ---  | --- | --- |
| 1 | 2 | 3 |


[Link to redirected page](https://experienceleague.adobe.com/docs/experience-manager-core-components/using/developing/developing.html)

```
Don't use <https://> for links..
```

## Command line {#command-line}

<table>
 <tbody>
  <tr>
   <th>Adaptive Form component</th>
   <th>Corresponding XFA component</th>
   <th>Included by default in Document of Record Template?</th>
   <th>Notes</th>
  </tr>
  <tr>
   <td>Button</td>
   <td>Button</td>
   <td>false</td>
   <td> </td>
  </tr>
  <tr>
   <td>Check box</td>
   <td>Check Box</td>
   <td>true</td>
   <td> </td>
  </tr>
  <tr>
   <td>Date picker</td>
   <td>Date/Time Field</td>
   <td>true</td>
   <td> </td>
  </tr>
  <tr>
   <td>Drop-down list</td>
   <td>Drop-down List</td>
   <td>true</td>
   <td> </td>
  </tr>
  <tr>
   <td>Scribble Signature</td>
   <td>Signature Scribble</td>
   <td>true</td>
   <td> </td>
  </tr>
  <tr>
   <td>Numeric box</td>
   <td>Numeric Field</td>
   <td>true</td>
   <td> </td>
  </tr>
  <tr>
   <td>Password box</td>
   <td>Password Field</td>
   <td>false</td>
   <td> </td>
  </tr>
  <tr>
   <td>Radio Button</td>
   <td>Radio Button</td>
   <td>true</td>
   <td> </td>
  </tr>
  <tr>
   <td>Text box</td>
   <td>Text Field</td>
   <td>true</td>
   <td> </td>
  </tr>
  <tr>
   <td>Reset button</td>
   <td>Reset Button</td>
   <td>false</td>
   <td> </td>
  </tr>
  <tr>
   <td>Submit button</td>
   <td><p>Email Submit Button</p> <p>HTTP Submit Button</p> </td>
   <td>false</td>
   <td> </td>
  </tr>
  <tr>
   <td>Terms and conditions</td>
   <td> </td>
   <td>true</td>
   <td> </td>
  </tr>
  <tr>
   <td>File Attachment</td>
   <td> </td>
   <td>false</td>
   <td>Not available in Document of Record template. Only Available in Document of Record through attachments.</td>
  </tr>
 </tbody>
</table>

## Containers {#containers}

<table>
 <tbody>
  <tr>
   <th>Adaptive Form component</th>
   <th>Corresponding XFA component</th>
   <th>Notes</th>
  </tr>
  <tr>
   <td>Panel<br /> </td>
   <td>Subform<br /> </td>
   <td>Repeatable panel maps to repeatable subform.</td>
  </tr>
 </tbody>
</table>


1. Based on whether you select a default or a custom template, some or all of the following properties appear in the Document of Record tab. Specify these appropriately:

    * **Logo Image**: You can either choose to use the logo image from the Adaptive Form, choose one from DAM, or upload one from your computer.
    * **Form Title**
    * **Header Text**
    * **Disclaimer Label**
    * **Disclaimer**
    * **Disclaimer Text**
    * **Accent Color**: The color in which header text and separator lines are rendered in the document or record PDF
    * **Font Family**: Font family of the text in the Document of Record PDF
    * **For Check Box and Radio Button components, show only the selected values**
    * **Separator for multiple selected value(s)**
    * **Include form objects that are not bound to data model**
    * **Exclude hidden fields from the Document of Record**
    * **Hide description of panels**

   >[!NOTE]
   >
   >If you are using an Adaptive Form template created with a verision of Designer prior to 6.3, for Accent Color and Font Family properties to work, ensure that the following is present in your Adaptive Form template under the root subform:

   ```xml
   <proto>
   <font typeface="Arial"/>
   <fill>
   <color value="4,166,203"/>
   </fill>
   <edge>
   <color value="4,166,203"/>
   </edge>
   </proto>
   ```

1. To save the branding changes, tap Done.

| Adaptive Form component |Corresponding XFA component |Notes |
|---|---|---|
| Image |Image |The TextDraw and Image components, whether bound or unbound, always appear in the Document of Record for an XSD-based Adaptive Form, unless excluded using the Document of Record settings. |
| Text |Text |

Foo

## Deep link from Bob
