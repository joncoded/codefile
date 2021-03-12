---
description: the metadata part of a webpage
---

# 🚧 HTML head

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
* `<meta>` = page metadata such as description or keywords for search engines to use
* `<link>` = references to other external scripts such as [CSS stylesheets](../../css/)

### `<meta>` tags

A well-developed page typically has about a dozen of these for search engine \(SEO\) and social media optimization \(SMO?\)

