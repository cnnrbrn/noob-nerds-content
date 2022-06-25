# Uncaught ReferenceError

Trying to access properties on an object that don't exist is a common bug.

This is what the error message looks like, where `name_of_object` is the object you are trying to retrieve the property from:

```js
Uncaught ReferenceError: name_of_object is not defined
```

Given this object

```js
const user = {
  name: "Blob"
};
```

this code

```js
const userName = person.name;
```

would produce this error:

```
Uncaught ReferenceError: person is not defined
```

That's because the code is trying to retrieve the `name` property from an object called `person` which does not exist as the object is called `user`.

If you encounter the error above, double-check the object you are trying to access exists.

######

Rewrite the line of code above so that the name property is retrieved from the correct object.

~~javascript objects uncaughtReferenceError~~

<nav>
     <a href="/javascript/objects/undefined">Back</a>
	 <a href="/javascript/objects/uncaught-type-error" class="next">Uncaught TypeError</a>
</nav>
