reposit.db is a lightweight and simple Node.js module for managing key-value pairs using a single SQLite database file. With reposit.db, you can easily add, get, update, and delete records without dealing with multiple files or complex database configurations.

**Installation**
To install reposit.db, run the following command:
npm install reposit.db
Here's a quick guide on how to use reposit.db:

Require and Initialize

const R3posit = require('reposit.db');
const reposit = new R3posit('mytest.db'); // You can specify the database file name

**#Add Data**

reposit.add('key', 'value');
const value = reposit.get('key');
console.log(`Value: ${value}`);

**Update Data**
reposit.update('key', 'new value');

**Delete Data**

reposit.delete('key');

**Close Database**

reposit.close();

**API**
```
add(key, value): Adds a new record to the database or updates the existing one.
get(key): Retrieves the value associated with the specified key. Returns null if the key does not exist.
update(key, value): Updates the value of an existing record.
delete(key): Deletes the record associated with the specified key.
close(): Closes the database connection.
```

***License***

reposit.db is licensed under the ISC License. See the LICENSE file for more details.
