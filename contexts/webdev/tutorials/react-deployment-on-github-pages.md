# React deployment on GitHub pages

### Connecting the local repository with the remote

In Terminal \(or any command line\) - if we have not yet already: 

* `$ git init` 
* `$ git remote origin add (remote url on github)`
* `$ git add -A`
* `$ git commit -m "pushing initial map"`
* `$ git push origin master`

### Installing the gh-pages utility

Then, let's set up the gh-pages package as a "dev dependency":

* `$ npm install gh-pages --save-dev`

### Editing package.json for deployment

* Add this property to the `package.json` file, replacing `yourname` and `yourrepo` with the obvious:

```text
"homepage" : "https://yourname.github.io/yourrrepo"
```

* Then, within the `scripts` property:

```text
"scripts" : {
    "predeploy" : "npm run build", 
    "deploy" : gh-pages -d build",
    ...
}
```

Overall, the `package.json` file should look something like: 

```text
{
  "homepage": "https://joncoded.github.io/whatever", 
  "name": "reactetc",
  "description": "some react stuff",
  "version": "1.0.0",
  "main": "src/index.js",
  "dependencies": {
    "react": "^17.0.0",
    "react-dom": "^17.0.0",
    "react-scripts": "^4.0.1",
  },
  "scripts": {
    "predeploy" : "npm run build", 
    "deploy" : gh-pages -d build",
    "start": "react-scripts start",
    "build": "react-scripts build"
  },
  "browserslist": [
    "defaults"
  ],
  "author": "joncoded",
  "license": "MIT"
}
```

### Deploying

* One line: 

`$ npm run deploy`

### Setting up the remote repository for GitHub pages

On GitHub:

* Create a new remote repository \(and note down its URL\)
* Go into the repository's **Settings**
  * Go to the section **GitHub Pages**
  * Under **Source**
    * Pick **"Branch: gh-pages" \(**
      * leave the folder at ****/\(root\)
    * Save

Wait a few seconds or a few minutes to see the page live on: 

https://**yourname**.github.io/**yourrepo**

