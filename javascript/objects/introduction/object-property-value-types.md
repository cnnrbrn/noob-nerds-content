# Object property value types

Some of the property types an object can have are:

- `string`, e.g. `"Hello"`
- `number`, e.g. `123`
- `boolean`, `true` or `false`
- `array`, e.g. `["red", "yellow", "blue"]`
- another `object`, e.g. `{colour: "red"}`
- a `function`, e.g. `function() {}`

Here is an object with one of each of the above types:

```
const animal = {
     type: "elephant",
     age: 32,
     isAfrican: true,
     nicknames: ["Blob", "Slob"],
     medicalHistory; {
          isCurrentlyDead: false
     },
     trumpet: function() {
          return "Praaaarrp!";
     }
}
```

######

Create an object called `user` with three properties:

- `id` with a `number` value
- `name` with a `string` value
- `isActive` with a `boolean` value

~~javascript objects objectWithThreeProperties 160~~

<nav>
     <a href="/javascript/objects/introduction/object-with-properties">Back</a>
     <a href="/javascript/objects/introduction/accessing-properties-with-dot-notation" class="next">Accessing properties with dot notation</a>
</nav>
