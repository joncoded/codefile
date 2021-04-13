# Accessibility with hierarchies

**Hierarchies** not only allow screen-reader users to tap into a summary list of sections of a webpage, but also provide some organization in the document for non-users:

### Heading hierarchies

```markup
<h1>Article title</h1>

<h2>Chapter 1</h2>

<h3>Introduction</h3>

<p>...</p>

<h3>Continuing</h3>

<p>...</p>

<h2>Chapter 2</h2>

<h3>Moving along</h3>

<p>...</p>

<h2>Chapter 3</h2>

<p>...</p>
```

In HTML, we have a couple of rules about how headings should appear in a document:

* `<h1>` must appear on every page
* `<h2>` must appear after `<h1>` \(i.e. no `<h1>` then `<h3>`\)
  * in general, `<hX>` must appear after `<hX-1>`

Note that while we cannot "skip downwards" in the hierarchy, we could still "skip upwards" \(an `<hX>` after an `<hX+Y>`, such as an `<h2>` after an `<h4>`\) 

```markup
<h1>Article title</h1>

<h2>Chapter 1</h2>

<h3>Introduction</h3>

<h4>The introduction for the introduction</h4>

<!-- no h3 required here -->

<h2>Chapter 2</h2>
```

### List hierarchies

Ensure to properly __markup any **nested lists**, i.e. _lists within lists:_

```markup
<ul>
    <li>List level 1 item 1</li>
    <li>List level 1 item 2 <!-- no closing li tag yet -->
        <ul>
            <li>List level 2 item 1</li>
            <li>List level 2 item 2</li>
            <li>List level 2 item 3</li>            
        </ul> <!-- close the nested list -->
    </li> <!-- now close "List level 1 item 2" -->
</ul>
```

Think of the nested list the same as text - mere content of a list item in the parent list!

