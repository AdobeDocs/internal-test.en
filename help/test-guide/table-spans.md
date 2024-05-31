---
title: Virushi table spans
description: Use HTML tables to create complex table with joined rows and columns
---
# Virushi table spans

We can use column spans and row spans to combine cells. However, we cannot nest tables within tables. We have limited abilities to add or remove borders within tables.

**Source table wiki**

<https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=tve&title=Logout+API+%7C+SRS+%7C+Services#253894408078fb027eacf84649b17c34958de93ba5>

## HTML table with spans

*Response*

The successful response is a list of objects described by the following table

<table>
<thead>
  <tr>
    <th>headers</th>
    <th></th>
    <th></th>
    <th></th>
    <th></th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td><strong>status</strong></td>
    <td colspan="4">200</td>
    <td>mandatory</td>
  </tr>
  <tr>
    <td><strong>Content-Type</strong></td>
    <td colspan="4">application/json</td>
    <td>mandatory</td>
  </tr>
  <tr>
    <td rowspan="6"><strong>body</strong><br></td>
  </tr>
  <tr>
    <td rowspan="6"><strong>mvpdLogouts</strong><br></td>
    <td colspan="4">JSON containing a list of elements, each element having the following fields:</td>
    <td rowspan="6">mandatory<br></td>
  </tr>
  <tr>
    <td><strong>actionName</strong></td>
    <td>
       <p>The action to be performed in a user-agent.</p>
       <p>The possible values are:</p>
       <ul>
        <li><strong>logout</strong> - The client application needs to load the URL indicated by the "url" field to perform logout with the MVPD. (MVPD authenticated profile exist)</li>
        <li><strong>complete</strong> - The client application is not required to perform any subsequent action with the MVPD (e.g. Temp Pass, Degradation, dummy logout endpoint).</li>
        <li><strong>invalid</strong> - The client application is not required to perform any subsequent action with the MVPD (e.g. MVPD authenticated profile does NOT exist).</li>
       </ul>
    </td>
    <td>mandatory</td>
  </tr>
  <tr>
    <td><strong>actionType</strong></td>
    <td>
       <p>The type of interaction the client application must perform in order to continue the flow with the action specified by the parameter "actionName".</p>
       <p>The possible values are:</p>
       <ul>
        <li><strong>interactive</strong> - This corresponds to an <i>actionName=logout</i> when the logout flow must continue with the navigation to the URL specified in the "url" response field.</li>
        <li><strong>none</strong> - This corresponds to an actionName=complete or <i>actionName=unsupported</i>.</li>
       </ul>
    </td>
    <td>mandatory</td>
  </tr>
  <tr>
    <td><strong>mvpd</strong></td>
    <td>The internal unique identifier associated with an Identity Provider during on-boarding process.</td>
    <td>mandatory</td>
  </tr>
  <tr>
    <td><strong>url</strong></td>
    <td>
      <p>The logout URL used to perform logout flow with the MVPD endpoint.</p><br>
      <p>Not present for: actionName - complete + invalid / actionType - none</p>
    </td>
    <td>mandatory&ast;</td>
  </tr>
  <tr>
    <td>&ast; these fields are present, but only in some specific business flows</td>
    <td></td>
    <td></td>
  </tr>
</tbody>
</table>

## Row spans example

<table>
<thead>
  <tr>
    <th></th>
    <th></th>
    <th>Online Support</th>
    <th>Business Support</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td></td>
    <td></td>
    <td></td>
    <td>Paid Support ($)</td>
  </tr>
  <tr>
    <td rowspan="3">Assigned Experts<br></td>
    <td>Account Support Lead</td>
    <td></td>
    <td>✔</td>
  </tr>
  <tr>
    <td>Named Support Engineer</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Technical Account Manager</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="12">Support Services</td>
    <td>Online Support</td>
    <td>Business hours</td>
    <td>Business hours</td>
  </tr>
  <tr>
    <td>24x7x365 P1 Issue Support</td>
    <td>✔</td>
    <td>✔</td>
  </tr>
  <tr>
    <td>Named Support Contacts (per product)</td>
    <td>4</td>
    <td>6</td>
  </tr>
  <tr>
    <td>Live Telephone Support</td>
    <td></td>
    <td>✔</td>
  </tr>
  <tr>
    <td>Escalation Management</td>
    <td></td>
    <td>✔</td>
  </tr>
  <tr>
    <td>Service Reviews per Year</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Expert Sessions per Year</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Case Reviews</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Event Management</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Environment Review, Maintenance &amp; Monitoring</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Release, Migration, Upgrade &amp; Product Roadmap Review</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Cloud Support Activities – Experience Manager as Cloud</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Field Services</td>
    <td>Launch Advisory Services – First Year of new solution</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Field Service Activities</td>
    <td></td>
    <td></td>
  </tr>
</tbody>
</table>

## Column spans

<table>
<thead>
  <tr>
    <th>Americas</th>
    <th>Europe, Middle East & Africa</th>
    <th>Asia Pacific</th>
    <th>Japan<sup>1</sup></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>6 am – 5:30 pm</td>
    <td>9 am – 5 pm</td>
    <td>9 am – 5 pm</td>
    <td>9 am – 5:30 pm</td>
  </tr>
  <tr>
    <td colspan="4">
      <p><sup>1</sup><i>Language support is available only in English and Japanese.</i></p>
      <p><i>Adobe Commerce excludes Japanese language support.</i></p>
      <p><i>P2, P3, P4 cases are limited to business hours only in Japan.</i></p>
    </td>
  </tr>
</tbody>
</table>
