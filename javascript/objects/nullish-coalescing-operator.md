# Nullish Coalescing Operator: ??

The nullish coalescing operator returns what's on its right side if what's on its left is null or undefined.

Below, because the value on the left of the `??` is null, the value on the right will be assigned to the `url` variable:

```js
const url = null ?? "default url";
```

We can use this operand to provide default values for missing object properties.

In the code below, if `product.imageUrl` is null or undefined, a default value of _"https://via.placeholder.com/200"_ will be assigned to the `url` variable:

```js
const url = product.imageUrl ?? "https://via.placeholder.com/200";
```

Below, if `product.image` or `product.image.url` is null or undefined, a default value of _"https://via.placeholder.com/200"_ will be assigned to the `url` variable:

```js
const url = product.image?.url ?? "https://via.placeholder.com/200";
```

######

Write a single line of code to

- select the price property from the object below
- assign the value to a variable called `productPrice`
- provide the default value "Price unkown" for the price property if it is null or undefined using the nullish coalescing operator

```js
const product = {
  price: null
};
```

######

Write a single line of code to

- select the city property from the object below
- assign the value to a variable called `propertyCity`
- provide a default value if the city or address property is null or undefined using the nullish coalescing operator
- use the <a href="/javascript/objects/optional-chaining">optional chaining operator</a> to prevent an error being thrown if the address property is null or undefined

```js
const property = {
  address: {
    city: null
  }
};
```

~~javascript objects nullishCoalescing~~

<nav>
  <a href="/javascript/objects/optional-chaining">Back</a>
	<a href="/javascript/objects/object-destructuring" class="next">Object destructuring</a>
</nav>
