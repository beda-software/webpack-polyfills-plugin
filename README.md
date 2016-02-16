[![npm version](https://badge.fury.io/js/webpack-polyfills-plugin.svg)](https://badge.fury.io/js/webpack-polyfills-plugin)

# webpack-polyfills-plugin

Adds polyfills from [polyfill-service](https://github.com/Financial-Times/polyfill-service) to bundle file. Without magic.

(It is fork from Sl1v3r/webpack-polyfills-plugin)

## Usage:

```javascript
var PolyfillsPlugin = require('webpack-polyfills-plugin');

module.exports = {

   // ...

   plugins: [
      new PolyfillsPlugin([
         'Array/prototype/find',
         'fetch'
      ])
   ]
}
```
