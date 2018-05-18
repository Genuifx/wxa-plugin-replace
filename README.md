# wxa-plugin-replace

[![NPM version](https://img.shields.io/npm/v/@wxa/plugin-replace.svg)](https://www.npmjs.com/package/@wxa/plugin-replace)

:tada:replace string in wxa

## Usage
### add replace target
```javascript
    new ReplacePlugin({
      list: [{
        regular: new RegExp('APP_ENV', 'gm'),
        value: 'bcds'
      }]
    })
```
### object configs
```javascript
    new ReplacePlugin({
      list: {
        'APP_ENV': 'bcds'
      }
    })
```

## Configurations
- **list**
  - **type**: `{Object, Array} list`
  - **default**: `[]`

an array or object to replace in `wxa` project
  
- **flag**
  - **type**: `{String} flag`
  - **default**: `gm`

regular express's flag.

