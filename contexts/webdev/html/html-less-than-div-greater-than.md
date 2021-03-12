---
description: dividing up a webpage
---

# 🚧 HTML &lt;div&gt;

Within an HTML page, inside the  `<body>` tag, one may `div`ide up the content in terms of `<div>` tags:

```markup
<html>

    <head>
        ...
    </head>
    
    <body>
    
        <div id="header">
        
            <h1>Page title</h1>
        
        </div>
        
        <div id="main">
        
            <div id="intro">            
                
                <h2>Welcome</h2>
                
                <img src="...">
                
            </div>
            
            <div id="outro">
                
                <h2>Bye!</h2>
                
                <p>Hope to see you soon!
                
            </div>
        
        </div>
        
        <div id="footer">
        
            <p>Copylight (current year)</p>
        
        </div>
    
    </body>
    
</html>
```

While this works fine on simple pages, things may get cluttered with `<div>` tags and we would soon replace `<div>` with other more meaningful tags such as `<section>`, `<header>`, `<footer>` and so on; we call these tags of **syntactic sugar** or, more specifically in this context, **semantic HTML:**

```markup
<html>

    <head>
        ...
    </head>
    
    <body>
    
        <header>
            
            <h1>Page title</h1>
        
        </header>
        
        <main>
        
            <section id="intro">                            
                
                <h2>Welcome</h2>
                
                <img src="...">
                
            </section>
            
            <section id="outro">
                
                <h2>Bye!</h2>
                
                <p>Hope to see you soon!
                
            </section>
        
        </main>
        
        <footer>
        
            <p>Copylight (current year)</p>
        
        </footer>
    
    </body>
    
</html>
```

Comparing the two, we see the second one has tags which make it that much more readable than the first one with just mostly `<div>` tags!

We will look more at semantic HTML in the next page ➡️

