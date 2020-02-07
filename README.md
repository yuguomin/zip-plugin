# zip-plugin
Used for webpack, his plugin packages all the bundle files into a single zip file.

# how to use
install this package
```
npm install zip-plugin -D
```

and use in webpack.config
```JavaScript
// demo webpack.config.plugin
const zipPlugin = require('zip-plugin');

module.exports = {
  entry: ...,
  output: ...,
  plugins: [
    new zipPlugin({
      filename: 'bundle' // this property used to set zip file name
    })
  ]
}
```

then, webpack build.