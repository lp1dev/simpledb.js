# SimpleDB.js

Simplistic Node.js database model.

## Install

> npm install --save https://github.com/lp1dev/simpledb.js.git

## Example

```javascript

const db = require('simpledb')

db.initSync('database.json')

db.set('test', 42)

db.get('test') // 42

db.write() // Saves your changes
