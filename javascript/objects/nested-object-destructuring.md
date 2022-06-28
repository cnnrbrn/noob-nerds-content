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
<!-- prettier-ignore -->
const { login: { username }} = user;
```
