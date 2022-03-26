# Moder Project from scratch with React

## the React entry point

The index.html in the public folder

## Supporting ES6

[Instructor] So we're going to be writing our React code using ES6 syntax and we're also going to need to add support for JSX, React's special HTML-like syntax for defining page layouts. And in order to do all this, we're going to start off by opening up a terminal inside our directory and running
`
npm install --save-dev @babel/core @babel/cli @babel/preset-env @babel/preset-react`

And then we're going to hit enter. And that might take a little while to run. But once it does, the next thing we need to do is create a .babelrc file. This file will tell the Babel transpiler what presets and plugins to use to transpile our code. So let's create this .babelrc file in the root of our directory. Call it .babelrc. Don't forget the dot before it. And inside this file, we're going to define a JSON object. And this object will have a property presets that will be an array of two strings. The first one's going to be babel/present-env, which handles the transformation of ES6 into common JS, and @babel/preset-react, which knows how to deal with JSX properly. Babel will use both of these presets to transform our code into something a browser can run, although just as a side note, most modern browsers now support ES6 syntax so this isn't as necessary as it once was. And that's it for now. Let's make sure to save this file and we'll see later on how to actually use Babel to transpile our code using the presets we've defined here.