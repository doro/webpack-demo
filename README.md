$ mkdir webpack-demo && cd webpack-demo
$ npm init
$ npm install --save-dev webpack webpack-cli

# create webpack config file

webpack.config.js: 

const path = require('path');
module.exports = {
  
  entry: './src/js/app.js',

  output: {
    filename: 'bundle.js',
    path: path.resolve(__dirname, 'dist')
  }

};


# run webpack using one of the following ways:
$ ./node_modules/webpack-cli/bin/webpack.js 
$ ./node_modules/.bin/webpack
$ npm run build
$ npx webpack

