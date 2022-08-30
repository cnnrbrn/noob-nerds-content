# Looping through arrays of objects with a forEach loop

An alternative to the for loop is the `forEach` loop.

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
  const productName = product.name;
});
```

The forEach method loops over the array and each item is passed into a function as an argument.

The function can also be written with the fat arrow syntax:

```js
products.forEach((product) => {
  const productName = product.name;
});
```

Or without the curly braces if the code inside the function is one line:

```js
products.forEach((product) => console.log(product.name));
```

## Limits of forEach

You cannot use the `continue` or `break` keywords with the forEach loop. If you want to use either of those, use a [for loop](/javascript/objects/looping-through-an-array-of-objects-for-loop).

######

Loop through the array of objects below with a forEach loop

- inside the loop assign each `headline` property to a variable called `headline`
- use [object destructuring](/javascript/objects/introduction/object-destructuring)

```js
const articles = [
  { headline: "Headline 1" },
  { headline: "Headline 2" }
];
```

~~javascript forEachLoops forEach1 240~~

######

Loop through the array of objects below with a forEach loop

- use [object destructuring](/javascript/objects/introduction/object-destructuring) to retrieve the `brand`, `model` and `price` properties
- don't alias any of the properties

```js
const phones = [
  { brand: "Apple", model: "Some model", price: 199.99 },
  { brand: "Android", model: "Some other model", price: 99.95 }
];
```

~~javascript forEachLoops forEach2 240~~
<nav>
  <a href="/javascript/objects/introduction/exiting-a-for-loop-with-break">Back</a>
	<a href="/javascript/objects/introduction/forEach-is-not-a-function" class="next">forEach is not a function</a>
</nav>
