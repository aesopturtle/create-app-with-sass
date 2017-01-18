# create-app-with-sass

This repo is forked from [rickharrison/create-react-app-sass](https://github.com/rickharrison/create-react-app-sass).
The main purpose is to add [Sass](http://sass-lang.com/) support not just for [create-react-app](https://github.com/facebookincubator/create-react-app), 
but also for [create-inferno-app](https://github.com/infernojs/create-inferno-app) (and probably other similar app creators).

### Installation

```
npm install create-app-with-sass --save-dev
```

### Usage

Replace your `start` and `build` scripts in your `package.json`

##### For React
```
"scripts": {
  "start": "craete-app-with-sass react-scripts start",
  "build": "craete-app-with-sass react-scripts build"
},
```
##### For Inferno
```
"scripts": {
    "start": "craete-app-with-sass inferno-scripts start",
    "build": "craete-app-with-sass inferno-scripts build"
},
```

Your `src` directory will automatically re-compile any `.scss` file into a `.css` file with the same name in the same location. 
Then you can `import` the `.css` file in your components the same way as before using `create-react-app` or `create-inferno-app`. 
You will also need to add `*.css` to your `.gitignore` file as they are now just a build artifact and your `.scss` is the true source.
