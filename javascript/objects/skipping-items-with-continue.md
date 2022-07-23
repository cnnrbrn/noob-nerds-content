# Skipping items in a loop with continue

We can use the `continue` keyword to skip over items in an array.

Given this array of objects:

```js
const products = [
  {
    name: "Product 1",
    onSale: true
  },
  {
    name: "Product 2",
    onSale: false
  },
  {
    name: "Product 3",
    onSale: true
  }
];
```

if we only wanted to access product objects that are on sale, we could write this:

```js
for (i = 0; i < products.length; i++) {
  if (products[i].onSale === false) {
    continue;
  }

  const product = products[i];
  console.log(product);
}
```

This code would only log the first and third items in the array as the continue keyword would skip the second item due to the if statement condition.

######

Loop through the array of objects below with a for loop and console log the `title` property of each object but only if the `numberOfPages` property is less than 300.

```js
const books = [
  { title: "Book 1", numberOfPages: 150 },
  { title: "Book 2", numberOfPages: 250 },
  { title: "Book 3", numberOfPages: 350 }
];
```

~~javascript objects continue~~

<nav>
  <a href="/javascript/objects/looping-through-an-array-of-objects-for-loop">Back</a>
	<a href="/javascript/objects/exiting-a-loop-with-break" class="next">Exiting a loop with break</a>
</nav>
