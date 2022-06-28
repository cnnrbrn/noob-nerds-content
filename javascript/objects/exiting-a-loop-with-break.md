# Exiting a loop with break

You can exit a loop with the `break` keyword.

Given this array of objects

```js
const products = [
  {
    name: "Product 1"
  },
  {
    name: "Product 2"
  },
  {
    name: "Product 3"
  }
];
```

if we only wanted to access the first two items and then leave the loop, we could write

```js
for (i = 0; i < products.length; i++) {
  if (i === 2) {
    break;
  }

  const product = products[i];
  console.log(product);
}
```

We can also exit the loop based on an object property.

```js
const movies = [
  { name: "Movie 1", inProduction: true },
  { name: "Movie 2", inProduction: false },
  { name: "Movie 3", inProduction: null }
];
```

The code below will leave the loop as soon as an object with an `inProduction` value of `null` is encountered:

```js
for (i = 0; i < movies.length; i++) {
  if (movies[i].inProduction === null) {
    break;
  }

  const movie = movies[i];
  console.log(movie);
}
```

######

Loop through the array of objects below with a for loop and console log the `title` property of only the first three objects. Use the break keyword to exit the loop.

```js
const books = [
    { title: "Book 1" },
    { title: "Book 2" },
    { title: "Book 3" },
    { title: "Book 4" },
];
```

~~javascript objects break~~

<nav>
  <a href="/javascript/objects/skipping-items-with-continue">Back</a>
	<a href="/javascript/objects/looping-through-arrays-of-objects-forEach" class="next">forEach</a>
</nav>