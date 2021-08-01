---
description: allowing the user to input one line of plain text
---

# HTML inputs

### HTML input: text

**Plain text** inputs allow the user to input a single line:

```markup
<label for="firstName">First name</label>
<input type="text" id="firstName" name="firstName">
```

The `placeholder` attribute displays a suggested value for the input field \(but the form will not include the value by default when the user submits the form\)

```markup
<label for="firstName">First name</label>
<input type="text" id="firstName" name="firstName" placeholder="e.g. Jon">
```

### HTML input: radio

**Radio** inputs appear when the user needs to make _**one choice out of two or more possible choices**_: 

```markup
<p>Select a language:</p>

<div>
    <input type="radio" id="language-en" name="language">
    <label for="language-en">English</label>
</div>

<div>
    <input type="radio" id="language-fr" name="language">
    <label for="language-fr">Français</label>
</div>

<div>
    <input type="radio" id="language-tw" name="language">
    <label for="language-tw">繁體中文</label>
</div>
```

Note that `id` attributes must be unique, while all related fields share the same `name` attribute!

### HTML input: checkbox

**Checkbox** inputs appear when the user can make _**one or more choice ... out of one choice or more possible choices**_:

```markup
<p>Select your preferred language(s):</p>

<div>
    <input type="checkbox" id="language-en" name="language" checked>
    <label for="language-en">English</label>
</div>

<div>
    <input type="checkbox" id="language-fr" name="language">
    <label for="language-fr">Français</label>
</div>

<div>
    <input type="checkbox" id="language-tw" name="language">
    <label for="language-tw">繁體中文</label>
</div>
```

{% hint style="success" %}
Using the `checked` attribute on a `checkbox` makes it checked by default ☑️
{% endhint %}

As with radio, `id` attributes must all be unique, while all related fields share the same `name` attribute!

\(Note how only the `type` attribute in each field changed versus the radio input type!\)

### HTML input: password

**Passwords** allow the user to type into a field with the characters obscured:

![](../../../../.gitbook/assets/html-password.png)

```markup
<label for="password">Password:</label>
<input type="password" id="password" name="password">
```

### HTML input: number

### HTML input: c

