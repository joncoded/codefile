# Accessibility with role attributes

The `role` attribute helps guide assistive technologies in a few different ways: 

### `complementary`

The `complementary` role helps a screen reader user understand that the information in the `<div>` relates to a main section \(but remains meaningful when separated from it\):

```markup
<main>
    <h2>An article about accessibility</h2>
    ...
</main>

<div role="complementary">
    <h3>Other articles you may like</h3>
    ...
</div>
```

### `main`

The `main` role helps a screen reader user know the location of the main element of a webpage - as such, it can appear only once per page \(just like an `<h1>` tag\): 

```markup
<div role="main">

    <h1>Article title</h1>
    
    <h2>Subsection</h2>
    
    <p>...</p>
    
    <h2>Subsection 2</h2>
    
    <p>...</p>    
    
</div>

<aside>
    ...
</aside>
```

Since semantic HTML has the `<main>` tag, we should opt to use that tag and only reserve the `role="main"` for certain occasions:

```markup
<main>
<!-- this is content on the site unique to this page -->

    <h1>Article title</h1>
    
    <h2>Subsection</h2>
    
    <p>...</p>
    
    <h2>Subsection 2</h2>
    
    <p>...</p>    
    
</main>

<footer>
<!-- this content could appear on other pages -->
    ...
</footer>
```

### `presentation`

When we prefer that the screen reader does not read out the element, e.g. "ordered list" in a list that obviously lists items numerically: 

```markup
<ol role="presentation">
    <li>Do this now</li>
    <li>Do this later</li>
    <li>Do this much later</li>
</ol>
```

Or, when we have to do some hack in HTML \(perhaps because of a client who demanded an unconventional layout\): 

```markup
<section role="presentation" class="padding-100">
    <!-- some blank section with 100px padding -->
</section>

<section>
    <!-- a normal section that allows content 
    (such as an image) to overlap the above section -->
</section>
```

{% hint style="danger" %}
Ensure that the element with this role _does not have any meaningful content_ that the screen reader _cannot_ read! 
{% endhint %}

### Other `role` values

Many more roles exist to improve the screen reader experience and we can find them in this following list on Mozilla: 

{% embed url="https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA\_Techniques" %}



