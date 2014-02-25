# Indexed localStorageDB
### a simple, tiny database layer for localStorage

Documentation: http://kailashnadh.name/code/localstoragedb
Licensed under the MIT license.

# Usage / Examples
### Refer to the documentation for the whole CRUD, just change the createTable:

<pre>
...
// create the "books" table
lib.createTable("books",
		["id", "title", "author", "year", "copies"],
		["id", "title"] // Add an array as the 3rd parameter with the name of the column that you want to index
		);
...
}
</pre>
After the creation, each insert/update goes also to affect the indexes.

The performances for medium/large data extraction/update from/to your localStorage will raise **significantly**.

# Tests / Performance gain

Check this link http://jsperf.com/indexed-localstoragedb/14 to see the performance gain at his best
