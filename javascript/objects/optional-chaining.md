# Optional chaining: ?

You can use the optional chaining operator `?.` to safely access nested properties that potentially don't exist on an object.

Given this object

```js
const product = {
  name: "A product",
  image: {
    url: "image url",
    altText: "alt text"
  }
};
```

we can access the url property like this:

```js
const imageUrl = product.image.url;
```

But if there was another version of the product object that didnt have an image property

```js
const product = {
  name: "A product"
};
```

then trying to access `product.image.url` would throw a [type error](uncaught-type-error).

Using the optional chaining operator to access a property that may not exist will return the value `undefined` rather than an error if the property does not exist.

So `imageUrl` will be assigned the value undefined in the code below if there is no `image` property on the `product` object.

```js
const imageUrl = product.image?.url;
```

If `image` does exist on `product` then `imageUrl` will be assigned the value of `image.url`.
