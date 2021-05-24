# 🚧  CSS selectors

The following types of **selectors** exist in ****_most of_ CSS:

* **elements** - selects HTML elements like `<div>` and `<p>`
  * CSS: `div` and `p`
* **id** - selects any id attribute within an HTML element
  * CSS: `#some-id`
* **class -** any class attribute within an HTML element
  * CSS: `.some-class`
* **attribute** - any attribute within an HTML element
  * CSS: `[some-attribute]`
    * value that equals: `[some-attribute="some-value"]`
    * value starting with prefix: `[some-attribute^="prefix"]`
    * value ending with suffix: `[some-attribute$="suffix"]`
    * value that contains: `[some-attribute*="infix"]`
* **pseudo-elements** - helper keywords that deal with specific parts or states of elements
  * `:focus` - when the cursor focuses on some element
  * `:hover` - when the cursor points to some element
  * `::after` - dealing with content after some selector
  * `::before` - dealing with content before some selector

\*\*\*\*



