# Accessing object properties with dot notation

There are two ways to access object properties (to get the value of a property from an object).

The most common way is called `dot notation` which uses a `.` between the object and the property we want to get.

If we had this object:

```js
const product = {
  id: 9264,
  name: "Lovely product",
  price: 9.99
};
```

we can access its `id` property and assign it to a variable like this:

```js
const productId = product.id;
```

We can access its `price` property and assign it to a variable like this:

```js
const productPrice = product.price;
```

######

Write a single line of code that will:

- get the `name` property from the `product` object above
- assign it to a variable called `productName`.

~~javascript objects usingDotNotation~~

<nav>
     <a href="/javascript/objects/introduction/object-property-value-types">Back</a>
      <a href="/javascript/objects/introduction/accessing-properties-with-bracket-notation" class="next">Accessing properties with bracket notation</a>
</nav>
