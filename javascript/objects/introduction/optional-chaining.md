# Optional chaining: ?

You can use the optional chaining operator `?.` to safely access nested properties that might not exist on an object.

Given this object

```js
const product = {
  name: "A product",
  image: {
    url: "image url"
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

then trying to access `product.image.url` would throw a [type error](/javascript/objects/optional-chaining).

Using the optional chaining operator will return `undefined` rather than an error if the property does not exist.

So `imageUrl` will be assigned the value `undefined` in the code below if there is no `image` property on the `product` object.

```js
const imageUrl = product.image?.url;
// undefined
```

If `image` does exist on `product` then `imageUrl` will be assigned the value of `image.url`.

The optional chaining operator is often used when looping through an array of objects and it's not clear whether an object will possess a property or not.

######

Sometimes the `user` object below may not have a `login` property. Write a single line of code to

- access the `username` property using dot notation and the optional chaining operator
- assign the value to a variable called `loginUsername`

```js
const user = {
  login: {
    username: "myusername"
  }
};
```

~~javascript objects optionalChaining~~

<nav>
  <a href="/javascript/objects/introduction/uncaught-type-error">Back</a>
	<a href="/javascript/objects/introduction/nullish-coalescing-operator" class="next">Nullish coalescing operator</a>
</nav>
