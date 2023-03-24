[![npm version](https://badge.fury.io/js/polyfills-webpack-plugin.svg)](https://badge.fury.io/js/polyfills-webpack-plugin)

# polyfills-webpack-plugin

Adds polyfills from [polyfill-service](https://github.com/Financial-Times/polyfill-service) to bundle file. Without magic.


Now the **maintained** plugin, forked from https://github.com/beda-software/webpack-polyfills-plugin/ and ownership transferred.

## Usage:

* Fist Parameter is which you want to Polyfills
* Second Parameter is provide for customer config which file you do not want to Poly, If you not provide this parameter, All files will execute Poly. This must be a Regular Expression

```javascript
var PolyfillsPlugin = require('polyfills-webpack-plugin');

module.exports = {

   // ...

   plugins: [
      new PolyfillsPlugin([
         'Array/prototype/find',
         'fetch'
      ], /\.(css|scss)$/)
   ]
}
```
