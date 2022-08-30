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
for (let i = 0; i < products.length; i++) {
  if (products[i].onSale === false) {
    continue;
  }

  const product = products[i];
}
```

This code would only log the first and third items in the array as the continue keyword would skip the second item due to the if statement condition.

######

Loop through the array of objects below with a for loop and

- inside the loop assign each `name` property to a variable called `recipeName` but only if the `numberOfIngredients` property is **less than 10**
- use the `continue` keyword to skip items that don't match the criteria
- declare the counting variable inside the for loop parenthesis, not before.
- use dot notation

```js
const recipes = [
  { name: "Recipe 1", numberOfIngredients: 4 },
  { name: "Recipe 2", numberOfIngredients: 12 },
  { name: "Recipe 3", numberOfIngredients: 7 },
  { name: "Recipe 4", numberOfIngredients: 10 }
];
```

~~javascript forLoops continue1 260~~

<nav>
  <a href="/javascript/objects/introduction/looping-through-an-array-of-objects-for-loop">Back</a>
	<a href="/javascript/objects/introduction/exiting-a-loop-with-break" class="next">Exiting a loop with break</a>
</nav>
