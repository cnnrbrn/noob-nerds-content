# Object Destructuring Aliasing

You can rename a property extracted from an object using object destructuring like this:

```js
const person = {
  name: "Name Surname"
};

const { name: fullName } = person;
```

This is the equivalent of writing:

```js
const fullName = person.name;
```

######

Write a single line of code that will

- extract the `summary` property from the `blog` object below and assign it to a variable called `synopsis` using object destructuring aliasing

```js
const blog = {
  title: "Title",
  summary: "Lorem ipsem dolor"
};
```

~~javascript objects objectDestructuringAliasing~~

<nav>
  <a href="/javascript/objects/object-destructuring">Back</a>
	<a href="/javascript/objects/nested-object-destructuring" class="next">Object destructuring aliases</a>
</nav>
