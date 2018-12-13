# SimpleDB.js

Simplistic Node.js database model.

## Install

> npm install --save https://github.com/lp1dev/SimpleDB-js.git

## Example

```javascript

const db = require('simpledb')

db
    .init('database.json')
    .then(() => {
        console.log('Database initialized')
    })
    .catch(error => {
        console.error(error)
    })


db.set('test', 42)

db.get('test') // 42

db.write() // Saves your changes