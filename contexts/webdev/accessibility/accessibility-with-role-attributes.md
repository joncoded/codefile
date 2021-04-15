# Accessibility with role attributes

The `role` attribute helps guide assistive technologies in a few different ways: 

### `complementary`

Helps a screen reader user understand that the information in the `<div>` relates to a main section \(but remains meaningful when separated from it\):

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



