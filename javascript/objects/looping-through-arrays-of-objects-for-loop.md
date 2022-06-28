# Looping through arrays of objects with a for loop

Given this array of objects

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

we can use a `for loop` to access each object in the array.

```js
for(let i = 0; i < products.length; i++>) {
    const product = products[i];
    console.log(product);
}
```

The `i` variable allows us to access each item in the array of objects by its index in the array.

The first item in an array has an index of 0, that's why `i` is initialised with the value `0`:

- `products[0]` is the first object in the array
- `products[1]` is the second object in the array

The last item in an array has an index value that is one less than the length of the array, hence the second part of the for loop: `i < products.length`. We only want the loop to continue while `i` is less than the length of the array.

######

Loop through the array of objects below with a for loop and console log the title property of each object.

```js
const books = [{ title: "Book 1" }, { title: "Book 2" }];
```

~~javascript objects forLoop~~

<nav>
  <a href="/javascript/objects/nested-object-destructuring">Back</a>
	<a href="/javascript/objects/skipping-items-with-continue" class="next">Skipping items with continue</a>
</nav>
