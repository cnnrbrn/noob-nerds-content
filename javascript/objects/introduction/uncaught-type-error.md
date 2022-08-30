# Uncaught TypeError

Trying to access a nested property of a property that doesn't exist will return this error in Chrome and Edge:

```bash
Uncaught TypeError: Cannot read properties of undefined (reading 'property_name')
```

where `property_name` is the name of the property you are trying to retrieve.

In Firefox the error looks like this:

```bash
Uncaught TypeError: object.property_name is undefined
```

Given this object

```js
const user = {
  login: {
    username: "name",
    password: "password"
  }
};
```

Running this code

```js
const username = user.credentials.username;
```

would return this error in Chrome:

```bash
Uncaught TypeError: Cannot read properties of undefined (reading 'username')
```

and this error in Firefox:

```bash
Uncaught TypeError: user.credentials is undefined
```

This is because there is no property called `credentials` on the `user` object, `user.credentials` is undefined so we are trying to access a property on an undefined value.

######

Rewrite the line of code above so that the `username` property is retrieved from the correct property.

~~javascript objects uncaughtTypeError~~

<nav>
    <a href="/javascript/objects/introduction/uncaught-reference-error">Back</a>
	  <a href="/javascript/objects/introduction/optional-chaining" class="next">Optional chaining</a>
</nav>
