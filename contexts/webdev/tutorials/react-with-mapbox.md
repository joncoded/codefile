---
description: Placing a non-Google digital map on your React site
---

# React with Mapbox

[Mapbox](https://www.mapbox.com) allows us to display a customized map on our own websites \(provided we stay within limits\) - to do so, we need:

### Prerequisites

* [Mapbox access token](https://account.mapbox.com/) 
* [Mapbox GL](https://docs.mapbox.com/mapbox-gl-js/api/) Javascript library
* Node.js with npm installed
* Some React and JavaScript experience

### Setup

In your project folder:

* Create a `package.json` file at the root
* Create a `public` folder for the final product and create the files:
  * `index.html` where the final product will display
  * `index.css` to house the styles for index.html
* Create an `src` folder and create the files to compile:
  * `app.js`  for all the React logic

#### Setting up `package.json`

Copy and paste this into `package.json` while changing any text that includes the \(bracketed text\): 

{% code title="package.json" %}
```javascript
{
    "name": "(project name)", 
    "description": "(the map project's description)",
    "version": "1.0.0",
    "main": "src/app.js",
    "dependencies": {
        "mapbox-gl": "^2.1.1",
        "react": "^17.0.0",
        "react-dom": "^17.0.0",
        "react-scripts": "^4.0.1",
        "worker-loader": "^3.0.7"
    },
    "scripts": {
        "start": "react-scripts start"
    },
    "browserslist": [
        "defaults"
    ],
    "author": "(your name)",
    "license": "MIT",
    "homepage": "(where you will upload this to)"
}
```
{% endcode %}

Note:

*  the `dependencies` version values may require updating in future days

### Deployment

In Terminal \(or any command line\): 

* `$ git init` if not already 

