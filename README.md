# webpack-project



Loading CSS 
In order to import a CSS file from within a JavaScript module, you need to install and add the style-loader and css-loader to your module configuration:

npm install --save-dev style-loader css-loader

This enables you to import './style.css' into the file that depends on that styling. Now, when that module is run, a <style> tag with the stringified css will be inserted into the <head> of your html file.

Loading Images 
So now we're pulling in our CSS, but what about our images like backgrounds and icons? Using the file-loader we can easily incorporate those in our system as well:

npm install --save-dev file-loader

Setting up HtmlWebpackPlugin 
First install the plugin and adjust the webpack.config.js file:

npm install --save-dev html-webpack-plugin

Cleaning up the /dist folder
npm install --save-dev clean-webpack-plugin