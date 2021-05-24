# CSS selectors

The following types of **selectors** exist in ****_most of_ CSS:

* **element** - selects HTML elements like `<div>` and `<p>`
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
* **pseudo-element** - helper keywords that deal with specific parts or states of elements
  * `:focus` - when the cursor focuses on some element
  * `:hover` - when the cursor points to some element
  * `::after` - dealing with content after some selector
  * `::before` - dealing with content before some selector

### **Hierarchy of elements**

Operators that sub-select elements based on their hierarchy in the HTML:

* "and" comma  
  * `selector1, selector2`
    * use the CSS in all instances of `selector1` and `selector2`
* "within the class" period 
  * `selector1.selector2`
    * use the CSS in `selector1` elements with a class of `selector2`
* "inside" space 
  * `selector1 selector2`
    * use the CSS in all instances of `selector2` that are inside `selector1`
* "parent" bracket
  * `selector1 > selector2`
    * use the CSS in all instances of `selector2` that is a direct child of `selector1`
* "younger sibling" plus
  * `selector1 + selector2` 
    * use the CSS in all instances of `selector2` that lie after `selector1`
* "elder sibling" tilde
  * `selector1 ~ selector2`
    * use the CSS in all instances of `selector1` that lie after `selector2`

