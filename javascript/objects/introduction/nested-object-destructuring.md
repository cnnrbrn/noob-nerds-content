# Nested object destructuring

Here is an example of accessing nested object properties using object destructuring.

Given this object

```js
const user = {
  login: {
    username: "some username",
    password: "good password"
  }
};
```

you can access the nested `username` property like this:

```js
const { login: { username } } = user;
```

This is the equivalent of writing:

```js
const username = user.login.username;
```

You can use aliasing with nested destructuring. 

If you wanted to rename the `username` variable to `loginName` you would write:

```js
const { login: { username: loginName } } = user;
```

######

Write a single line of code that will

- extract the `startDate` property from the `blog` object below using object destructuring 

```js
const blog = {
  title: "Blog",
  publishing: {
    startDate: "10 June"
  }
};
```

~~javascript objects nestedObjectDestructuring1~~

######

Write a single line of code that will

- extract the `full` property from the `product` object below and assign it to a variable called `fullPrice` using object destructuring aliasing

```js
const product = {
  name: "Product",
  price: {
    full: 9.99
  }
};
```

~~javascript objects nestedObjectDestructuring2~~

<nav>
  <a href="/javascript/objects/introduction/object-destructuring-aliasing">Back</a>
	<a href="/javascript/objects/introduction/looping-through-an-array-of-objects-for-loop" class="next">Looping through an array of objects</a>
</nav>