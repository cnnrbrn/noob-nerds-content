# Accessing nested objects

Objects are often nested within other objects.

```js
const user = {
    name: {
        firstName: "Burt",
        lastName: "Bacharach",
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

~~javascript objects accessingNestedObjectProperty4~~

<nav>
     <a href="/javascript/objects/accessing-nested-object-properties-2">Back</a>
</nav>