# 👍 Accessibility

### Definitions

**Accessible web content** deals with the availability of web content to as many people as possible, if not to everyone, via suitable alternatives, e.g.:

* hyperlinks with keyboard or other non-mouse methods
* audio content has a text-based equivalent
* video content has text-based captions
* images have alternate text accessible by a screen-reader
* text customization for font size, high-contrast, etc.

**Disability** refers to either a permanent or non-permanent, an inherent or acquired, a physical or non-physical \(e.g. cognitive\), impediment that prevents one from accessing something, e.g.:

* a temporary broken bone that prevent precise mouse usage
* a permanent blindness either from birth or a recent accident 
  * blindness as a complex topic
* an inability, like most people, to understand specialized jargon or choice of words

### Principles

The four "POUR" principles and questions to ask when determining the accessibility of anything:

* **perception** \(can more than one sense access it?\)
* **operability** \(can one navigate it using alternative input devices?\)
* **understandability** \(does it have legibility and consistency?\)
* **robustness** \(can one access it via different platforms?\)

### Issues

#### Alternatives

* giving an object some metadata that one can access via other means, e.g.
  * screen reader-readable **labels** in sections, forms and so on
  * **alternative \(alt\) text** for images that contain meaningful content

#### Focus

* a change in appearance of an input item on the screen that shows that it will currently receive input from an input hardware, e.g.
  * **focus ring**, the highlighted border of a text box
  * **text decoration**, the underline of a hyperlink
* if not specified via `tabindex`, non-interactive elements will not have **focus**, e.g.:
  * headings
  * paragraphs
  * images
* the order of elements matters, i.e.:
  * [right-floated](https://developer.mozilla.org/en-US/docs/Web/CSS/float) elements will still focus first

#### Organization

* keeping a document or system organized via: 
  * **heading** hierarchies
  * **list** hierarchies
  * sectional **dividers**
* providing an **alternative to using color** to differentiate objects
  * ensuring decent **color contrast**

