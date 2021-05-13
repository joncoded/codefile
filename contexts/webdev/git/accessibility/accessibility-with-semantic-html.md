# Accessibility with semantic HTML

When we organize a page with [semantic HTML](../../html/semantic-html/), as opposed to just `<div>` elements with `id` attributes, we can allow assistive technologies to summarize the page more readily, for example: 

* `<div id="nav">` becomes `<nav>` 
* `<div id="header">` becomes `<header>`
* `<div id="footer">` becomes `<footer>`

The screen reader may or may not notice the `id` attribute within a `<div>` ... however, it will certainly notice a tag like `<nav>` or `<header>` - even if it simply reads `<nav>` or `<header>` out loud!

