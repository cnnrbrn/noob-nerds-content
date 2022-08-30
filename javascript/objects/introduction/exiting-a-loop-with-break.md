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
for (let i = 0; i < products.length; i++) {
  if (i === 2) {
    break;
  }

  const product = products[i];
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
}
```

######

Loop through the array of objects below with a for loop and 

- inside the loop assign each `title` property to a variable called `blogTitle` but only for the first three objects
- use the `break` keyword to exit the loop before any other code inside the loop
- declare the counting variable inside the for loop parenthesis, not before.
- use dot notation

```js
const blogs = [
    { title: "Blog 1" },
    { title: "Blog 2" },
    { title: "Blog 3" },
    { title: "Book 4" },
];
```

~~javascript forLoops break1 260~~

<nav>
  <a href="/javascript/objects/introduction/skipping-items-with-continue">Back</a>
	<a href="/javascript/objects/introduction/looping-through-an-array-of-objects-forEach" class="next">forEach</a>
</nav>