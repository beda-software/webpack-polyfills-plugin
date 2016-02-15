# webpack-polyfills-plugin

Adds polyfills from [polyfill-service](https://github.com/Financial-Times/polyfill-service) to bundle file. Without magic.


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
