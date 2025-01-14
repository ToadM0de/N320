## Assignment 2: Node.js Modules

### Running a Node Script

Run it:

- directly in the terminal
  1. Using filename and extension
  ```console
  node index.js
  ```
  2. Using just filename
  ```console
  node index
  ```
  3. Using just folder / directory
  ```console
  node ./functions
  ```
- through a npm package script shortcut `(package.json)`
  ```json
  {
    "scripts": {
      "start": "node index.js"
    }
  }
  ```

### Importing / Exporting files in Node.js

Import - using another file for your script

```js
const fileVar = require("./filepath/fileName.js");
```

Export - allowing variables / methods to be used by other scripts

```js
const thingToUse = 3.141592653589793238462643383279502;

module.exports = {
  thingsToUse: thingsToUse,
};
```
