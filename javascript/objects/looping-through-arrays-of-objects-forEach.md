# Looping through arrays of objects with a forEach loop

An alternative to the for loop is the forEach loop.

We can loop through this array of objects

```js
const products = [
  {
    name: "Product 1"
  },
  {
    name: "Product 2"
  }
];
```

with this code

```js
products.forEach(function (product) {
  console.log(product.name);
});
```

The forEach method loops over the array and each item is passed into a function as an argument.

The function can also be written with the fat arrow syntax:

```js
products.forEach((product) => {
  console.log(product.name);
});
```

Or without the curly braces if the code inside the function is one line:

```js
products.forEach((product) => console.log(product.name));
```

## Limits of forEach

You cannot use the `continue` or `break` keywords with the forEach loop. If you want to use either of those, use a [for loop](/javascript/objects/looping-through-arrays-of-objects-for-loop).

######

Loop through the array of objects below with a forEach loop and console log the title property of each object.

```js
const books = [{ title: "Book 1" }, { title: "Book 2" }];
```

~~javascript objects forEach~~

<nav>
  <a href="/javascript/objects/nested-object-destructuring">Back</a>
	<a href="/javascript/objects/forEach-is-not-a-function" class="next">forEach is not a function</a>
</nav>
