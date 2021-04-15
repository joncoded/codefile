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

