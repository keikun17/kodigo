# Webpack


Configuraton files

    - `webpack.config.js` For the local server
    - `webpack.dist.config.js` For dist

These config files are Loaded in the `Gruntfile` as

    var webpackDistConfig = require('./webpack.dist.config.js'),
        webpackDevConfig = require('./webpack.config.js');

    module.exports = function (grunt) {
      // ...

      grunt.initConfig({
        pkg: pkgConfig,

        webpack: {
          options: webpackDistConfig,
          dist: {
            cache: false
          }
        },

        'webpack-dev-server': {
          options: {
            hot: true,
            port: 8000,
            webpack: webpackDevConfig,
            publicPath: '/assets/',
            contentBase: './<%= pkg.src %>/'
          },
        // ...


## Loaders

Webpack loaders allow you to preprocess files as you load them with `require()`

### Usage example

#### Case 1: runtime

    var css = require('!css!autoprefixer!./file.css');

#### Case 2: Configuration level

Setting loaders at the configuration with the css-loader,sass-loader and autoprefixer-loader (separate loaders installed via npm)

      // File: webpack.config.js

      // ...
      module: {
        // ...
        loaders: [
        test: /\.sass/,
          loader: 'style-loader!css-loader!sass-loader?outputStyle=expanded&indentedSyntax!autoprefixer-loader?safe=true'
        }, {
          test: /\.css$/,
          loader: 'style-loader!css-loader!autoprefixer-loader?safe=true'
        },
        // ...
