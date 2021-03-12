---
description: displaying data in cells on an HTML page
---

# HTML tables

As part of semantic HTML, **tables** allow us to make "two-dimensional lists" with headers, rows, columns and footers:

```markup
<table>
    <caption>Explaining the table for accessibility</caption>
    <thead>
        <tr>
            <th>Column 1 Header</th>
            <th>Column 2 Header</th>
            <th>Column 3 Header</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Row 1, Column 1</td>
            <td>Row 1, Column 2</td>
            <td>Row 1, Column 3</td>
        </tr>
        <tr>
            <td>Row 2, Column 1</td>
            <td>Row 2, Column 2</td>
            <td>Row 2, Column 3</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td>Total, Column 1</td>
            <td>Total, Column 2</td>
            <td>Total, Column 3</td>
        </tr>
    </tfoot>
</table>    
```

A table with this structure should appear \(although, of course, styling will differ\): 

| Column 1 Header | Column 2 Header | Column 3 Header |
| :--- | :--- | :--- |
| Row 1, Column 1 | Row 1, Column 2 | Row 1, Column 3 |
| Row 2, Column 1 | Row 2, Column 2 | Row 2, Column 3 |
| **Total, Column 1** | **Total, Column 2** | **Total, Column 3** |

### Table parts

The HTML `<table>` and its child elements make up one very well-defined set of semantic HTML tags: 

* `<table>` = a **table**
  * `<caption>` = the table's description \(for accessibility purposes\)
  * `<thead>` = the **table header**
    * `<tr>`  = a **table row** 
    * `<th>` = a **table heading** column
  *  `<tbody>` = the **table body** that usually covers most of the table's data 
    * `<tr>` = a **table row** \(similar to the one in `<thead>`\)
      * `<td>` = a table cell within a table row
  * `<tfoot>` = the **table footer** that usually has the last row of the table

\(Note that the `<tfoot>` typically has the same `<tr>` and `<td>` child elements as the `<tbody>`\)

{% hint style="warning" %}
Tables were so well-defined that, in the early days of the Internet, many people once used them to _build webpage layouts_ 😮

However, for many reasons beyond the scope of this page \(including accessibility\), we should **not** adopt this practice...

...as much as possible, tables should contain only brief amounts of text in each `<td>` cell, much like a chart that displays statistics!
{% endhint %}

