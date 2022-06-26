# Nullish Coalescing Operator: ??

The nullish coalescing operator returns what's on its right side if what's on its left is null or undefined.

Below, because the value on the left of the `??` is null, imageUrl will be assigned the value on the right:

```js
const url = null ?? "default url";
```

We can use this operand to provide default values for missing object properties.

If `product.imageUrl` is null or undefined, `url` will be assigned a placeholder image url:

```js
const url = product.imageUrl ?? "https://via.placeholder.com/200";
```

If `product.image` or `product.image.url` is null or undefined, `url` will be assigned a placeholder image url:

```js
const url = product.image?.url ?? "https://via.placeholder.com/200";
```
