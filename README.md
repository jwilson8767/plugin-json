plugin-yaml
===========

SystemJS YAML loader plugin

Installation
-------------
If using jspm just run `jspm install github:jwilson8767/plugin-yaml`


Usage
-------------

To load all URLs with `.yaml` or `.yml` filename extension via this plugin:

```javascript
SystemJS.config({
  map: { 'plugin-yaml': 'github:jwilson8767/plugin-yaml@0.1.0/yaml.js' },
  meta: { 
    '*.yaml': { loader: 'plugin-yaml' },
    '*.yml': { loader: 'plugin-yaml' }
  }
});
```

then import your desired files with `import {data} from 'data.yaml'`

Testing this project
--------------------

```sh
npm test
```

browse to <http://localhost:3000/test> and open the browser's development console.
You should see the json object logged.
