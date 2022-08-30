# Object Destructuring

Object destructuring extracts properties from objects and assigns them to variables.

Given this object

```js
const movie = {
  title: "Title",
  description: "Description",
  releaseDate: "20 January 2022"
};
```

We can extract the `title` property and assign it to a variable called `title` like this:

```js
const { title } = movie;
```

This is the same as writing:

```js
const title = movie.title;
```

We can extract multiple variables at the same time:

```js
const { title, description, releaseDate } = movie;
```

This is the same as writing:

```js
const title = movie.title;
const description = movie.description;
const releaseDate = movie.releaseDate;
```

######

Write a single line of code that will

- extract the `summary` property from the `blog` object below using object destructuring

```js
const blog = {
  title: "Title",
  summary: "Lorem ipsem dolor"
};
```

~~javascript objects objectDestructuring~~

<nav>
  <a href="/javascript/objects/introduction/nullish-coalescing-operator">Back</a>
	<a href="/javascript/objects/introduction/object-destructuring-aliasing" class="next">Object destructuring aliasing</a>
</nav>
