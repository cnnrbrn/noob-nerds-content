# Uncaught ReferenceError

Trying to access a property on an object that doesn't exist is a common error.

This is what the error message looks like, where `name_of_object` is the object you are trying to retrieve the property from:

```bash
Uncaught ReferenceError: name_of_object is not defined
```

Given this object

```js
const user = {
  name: "myname"
};
```

this code

```js
const userName = person.name;
```

would produce this error:

```bash
Uncaught ReferenceError: person is not defined
```

That's because the code is trying to retrieve the `name` property from an object called `person` which does not exist because the object is called `user`.

If you encounter the error above, double-check the object you are trying to access exists.

######

Rewrite the line of code above so that the `name` property is retrieved from the correct object.

~~javascript objects uncaughtReferenceError~~

<nav>
     <a href="/javascript/objects/introduction/undefined-properties">Back</a>
	 <a href="/javascript/objects/introduction/uncaught-type-error" class="next">Uncaught TypeError</a>
</nav>
