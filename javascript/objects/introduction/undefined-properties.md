# Undefined: Retrieving properties that don't exist

If you try to access a property on an object that doesn't exist you will receive the value `undefined`.

Given this object

```js
const product = {
  name: "A product",
  price: 10.99
};
```

the code below will return `undefined` as there is no property called `cost`:

```js
const productPrice = product.cost;
```

If you receive an undefined value when trying to retrieve an object property, make sure the property exists on the object.

######

Rewrite the line of code above to retrieve the `price` property from the product.

~~javascript objects undefinedProperties~~

<nav>
     <a href="/javascript/objects/introduction/accessing-nested-object-properties-part-2">Back</a>
	 <a href="/javascript/objects/introduction/uncaught-reference-error" class="next">Uncaught ReferenceError</a>
</nav>
