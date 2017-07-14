plugin-yaml
===========

SystemJS YAML loader plugin

Configuration
-------------

To load all URLs with `.yaml` or `.yml` filename extension via this plugin:

```javascript
SystemJS.config({
  map: { 'plugin-yaml': 'plugin-yaml/yaml.js' },
  meta: { 
    '*.yaml': { loader: 'plugin-yaml' },
    '*.yml': { loader: 'plugin-yaml' }
  }
});
```

Testing this project
--------------------

```sh
npm test
```

browse to <http://localhost:3000/test> and open the browser's development console.
You should see the json object logged.
