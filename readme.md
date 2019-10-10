# React Boilerplate

#### Basic stuff:
```
$npm init -y 
$npm install --save-dev webpack webpack-cli
```

#### Instead of running $node_modules/.bin/webpack, run the following:
```
$npm run build
```
#### It runs by default in production mode, making the output bundle minified (or set it at webpack.config.js). Otherwise:
```
$npm run build -- --mode development
```
#### Or configure the mode in the webpack.config.js

#### To see what our code does at the terminal:
```
$node dist/app.bundle.js
```

#### Install babel:
```
$npm i -D @babel/core @babel/cli @babel/preset-env
```

#### How to run babel:
```
$node_modules/.bin/babel <js-file>
$(npm bin)/babel <js-file>
$(npm bin)/babel <js-file> --presets=@babel/preset-env
```

#### weback --> to bundle our JavaScript
#### babel --> to compile our JavaScript in JS that will run in down level browsers
#### until now they are not configured to work together
#### so to work together, we install the babel-loader and configure accordingly the webpack.config.js
```
npm i -D babel-loader
```

#### Install React (-S: to save as runtime dependencies)
```
npm i -S react react-dom prop-types
```

#### Configure babel for React with preset-react
```
npm i -D @babel/preset-react
```
