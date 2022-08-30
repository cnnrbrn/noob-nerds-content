# Accessing nested object properties

Objects are often nested within other objects.

```js
const user = {
  name: {
    firstName: "Randalph",
    lastName: "Bacharach"
  }
};
```

To access the `lastName` property in the object above we first need to get the `name` property (which also has an object value) and then get the lastName property. We can use dot notation:

```js
const lastName = user.name.lastName;
```

######

Write a single line of code that will:

- retrieve the `firstName` property from the object above
- assign it to a variable called `userFirstName`
- use dot notation

~~javascript objects accessingNestedObjectProperty1~~

<nav>
     <a href="/javascript/objects/introduction/accessing-properties-with-bracket-notation">Back</a>
     <a href="/javascript/objects/introduction/accessing-nested-object-properties-part-2" class="next">Accessing nested object properties part 2</a>
</nav>
