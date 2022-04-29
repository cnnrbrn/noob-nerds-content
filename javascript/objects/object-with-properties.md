# An object with properties

Say we had two string variables, firstName and lastName:

```js
const firstName = "Gertrude";
const lastName = "Smith";
```

We can store the variables together in an object. We'll call the object `person`:

```js
const person = {
    firstName: "Gertrude",
    lastName: "Smith"
};
```

The variables become `properties` on the object. The object above has two properties, `firstName` and `lastName`.

The left side of the property (the left side of the colon `:`) is called the `key` and the right side is called the `value`.

The first property in the person object has a __key__ of `firstName` and a __value__ of `"Gertrude"`, a string value.

######
Create an object called `movie` with two properties, `title` and `description`. Both must have string values.

~~javascript objects movieObjectTwoStringProperties~~

<nav>
     <a href="/javascript/objects/intro">Back</a>
    <a href="/javascript/objects/object-property-value-types" class="next">Next: Object property value types</a>
</nav>
