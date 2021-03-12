---
description: the metadata part of a webpage
---

# HTML &lt;head&gt;

As the `<html>` tag usually contains two top-level child tags: `<head>` and `<body>` we know that while the `<body>` contains the main content, the `<head>` contains "content about the content", also known as **metadata**:

```markup
<html>

    <head>
    
        <!-- content about the content, e.g. -->

        <title>MySite 2.0</title>
    
    </head>
    
    <body>
    
        <!-- main content goes here -->
        
    </body>
    
</html>
```

As with the `<body>` any and all tags in `<head>` are really optional but typically include:

* `<title>` = the title which appears on the tab \(or browser bar\)
  * not to be confused with **heading** like `<h1>`, `<h2>`, etc. 
  * search engines will use this as a webpage's title
* `<meta>` = page metadata for search engines to use
* `<link>` = references to other external scripts such as [CSS stylesheets](../../css/)

### `<meta>` tags

A well-developed page typically has about a dozen of these self-closing tags for search engine \(SEO\) and social media optimization \(SMO?\) purposes, the most important of which are:

#### description

* the description of the web page

```markup
<meta name="description" content="A page that shows you how to use meta tags">
```

#### keywords

* basically a description in terms of single words or phrases

```markup
<meta name="keywords" content="meta tags, html, web development">
```

#### viewport

* more relevant in recent times, this makes the page more readable in mobile phone screens

```markup
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### `<link>` tags

The most common use of the `<link>` tag is to include, or relate \(hence `rel`\), a [CSS](../../css/) stylesheet file:

```markup
<link rel="stylesheet" href="style.css">
```

