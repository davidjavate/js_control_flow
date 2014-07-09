# Google Shopping Lab
## Conditionals and Loops


Use the product search result in your file to check the following:

1.) The `kind` of results you're are dealing  are `shopping#products`. Go through the `items` and find all results that have `kind` of `shopping#product`. How many are there? Where else is this count information stored in the search results?

var data = require("./products.json")

// Write your solutions below
var instances = 0;

var items = data['items'];

for (i = 0; i < items.length; i += 1) {
if (items[i]['kind'] === 'shopping#product') {
instances += 1;
}
}

console.log(data["items"]);
console.log(instances);

console.log(data["items"]);

> console.log(instances);
25



2.) Find all items with a `backorder` availability in `inventories`.

var items = data['items'];

for (var i = 0; i < items.length; i++ ) {
if (items[i]['product']['inventories'][0]['availability'] === 'backorder'){
console.log("Sorry this product is unavailable")
}
}


3.) Find all items with more than one link.
var items = data ['items'];

for (var i = 0; i < items.length; i++ ) {
if (items[i]['images'][0] >1){
console.log(i)
}
}

4.) Find all `canon` products in the items (careful with case sensitivity).

var items = data ['items'];

for (var i =0; i< items.length; i++) {
	if (items[i]['product']['brand'] === 'Canon'){
	console.log(i);
}
}

5.) Find all `items` that have **product** **author** **name** of "eBay" and are brand "Canon".

var items = data ['items'];

for (var i =0; i< items.length; i++) {
	if (items[i]['product']['author']['name'] === 'eBay' && items[i]['product']['brand']==='Canon'){
	console.log(i);
}

6.) Print all the products with their **brand**, **price**, and a **image link**
var items = data ['items'];

for (var i =0; i< items.length; i++) {
	console.log(items[i]['product']['brand'] + ", " + items[i]['product']['inventories'][0]['price']+ ", " + items[i]['product']['images'][0])
}
