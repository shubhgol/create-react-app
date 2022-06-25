# create-react-app
 setup React application without the Create-React-App CLI
 
 SetUp
 
 1) install react library
       react , react-dom
2) install webpack library
     webpack --- which include all core webpack functionality
     webpack-cli --- enable running webpack from the command line
     webpack-dev-server --- this development server automatically rerun webpack when our file is changed

     //The core function of webpack is that it takes a bunch of JavaScript files we write in our project and turns them into a single, minified file, so that it will be quick to serve. Starting from webpack 4, we aren’t required to write a configuration file at all to use it, but in this tutorial we will write one so that we can understand it better.


3) configuring Babel
   //Babel is a toolchain that is mainly used to convert ECMAScript 2015+ code into a backwards compatible version of JavaScript in current and older browsers or environments.

   @babel/core --- is the main dependency that includes babel transform script.

   @babel/preset-env --- is the default Babel preset used to transform ES6+ into valid ES5 code. Optionally configures browser polyfills automatically.

   @babel/present-react --- is used for transforming JSX and React class syntax into valid JavaScript code.

   babel-loader ---- is a webpack loader that hooks Babel into webpack. We will run Babel from webpack with this package.
   
   
#   webpack config setup
   
   mode: env whether its running in dev or prod env
   entry: path of main js file
   output : {
      path: directory name,
      filename: file name
   }
   
   module : {
   rules: [{
      test: 'regex path to text file'
      exclude : regex for file to not be test
      loader: loader to compile this type of file
      
   }}
}
