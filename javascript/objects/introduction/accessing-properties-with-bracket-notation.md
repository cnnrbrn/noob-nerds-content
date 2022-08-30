# Accessing object properties with bracket notation

Apart from dot notation we can access object properties using bracket notation which uses `[]` around the property name we want to get.

Bracket notation is how we can access a property that has a space or hyphen in its key.

Say we had this object:

```js
const product = {
    id: 9264,
    "product name": "Lovely product",
    "product description": "What a lovely product"
    "retail-price": 9.99,
}
```

The second and third property keys have a space in them and the fourth has a hyphen so they need to be created with quotes.

We can access the `"product name"` property and assign it to a variable like this:

```js
const productName = product["product name"];
```

We can access its `"retail-price"` property and assign it to a variable like this:

```js
const producPrice = product["retail-price"];
```

######

Write a single line of code that will:

- get the `"product description"` property from the `product` object above
- assign it to a variable called `productDescription`.

~~javascript objects usingBracketNotation~~

<nav>
     <a href="/javascript/objects/introduction/object-property-value-types">Back</a>
      <a href="/javascript/objects/introduction/accessing-nested-object-properties" class="next">Accessing nested object properties</a>
</nav>
