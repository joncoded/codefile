---
description: writing notes while coding webpages
---

# HTML commenting and doctype

**HTML comments** allow us to enter notes in an HTML file and they won't directly affect the run time of a page: 

```markup
<!-- this is a comment -->

<!-- here is another comment -->

<!-- 2020-12-31 : TODO don't forget to finish this -->
```

In general: 

```text
<!-- (some one line message) -->
```

Comments can also have multiple lines:

```text
<!--

this 
will
work 
too

-->
```

### DOCTYPE?

The **HTML doctype** may look like a comment but it actually informs the browser that the document really uses a specific version of HTML, in this case, HTML 5:

```markup
<!DOCTYPE html>
```

Older versions of HTML had more arcane doctypes, such as HTML 4.01: 

```markup
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" 
"http://www.w3.org/TR/html4/loose.dtd">
```

...which we no longer use but may see when we "View Source" into some older pages ;\)

