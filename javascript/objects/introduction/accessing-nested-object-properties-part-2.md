# Accessing nested object properties part 2

The object below has some properties whose keys are contained in strings and some properties that are nested several levels deep.

```js
const user = {
  login: {
    username: "randalph",
    password: "strongpassword",
    "suspended-or-blocked": false
  },
  address: {
    locality: {
      building: {
        "building name": "Nice building",
        floor: 4,
        flatNo: 21
      },
      street: "1 Some Street"
    },
    city: "The Big City"
  }
};
```

To get the `"suspended-or-blocked"` property we first need to get the `login` property (an object) and then get the "suspended-or-blocked" for which we'll need to use bracket notation as it contains hyphens:

```js
const suspendedOrBlocked = user.login["suspended-or-blocked"];
```

The `floor` property is nested quite deep. It is a property of the `building` object which is a property of the `locality` object which is a property of the `address` object.

```js
const floor = user.address.locality.building.floor;
```

######

Write a single line of code that will:

- retrieve the `password` property from the object above
- assign it to a variable called `userPassword`
- use dot notation

~~javascript objects accessingNestedObjectProperty2~~

######

Write a single line of code that will

- retrieve the `street` property from the object above
- assign it to a variable called `userStreet`
- use dot notation

~~javascript objects accessingNestedObjectProperty3~~

######

Write a single line of code that will

- retrieve the `building name` property from the object above
- assign it to a variable called `userBuildingName`

~~javascript objects accessingNestedObjectProperty4~~

<nav>
     <a href="/javascript/objects/introduction/accessing-nested-object-properties">Back</a>
	 <a href="/javascript/objects/introduction/undefined-properties" class="next">Undefined properties</a>
</nav>
