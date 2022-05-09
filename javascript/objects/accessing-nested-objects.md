# Accessing nested objects

Often objects are nested within other objects.

```js
const user = {
    name: {
        firstName: "Burt",
        lastName: "Bacharach",
    },
    login: {
        username: "burt",
        password: "strongpassword",
        "suspended-or-blocked": false,
    },
    address: {
        locality: {
            building: {
                "building name": "Nice building",
                floor: 4,
                flatNo: 21
            },
            street:  "1 Some Street",          
        },
        city: "The Big City"
    },
    // interests: ["frogs", "dinosaurs", "horse hunting", "climate change denying"]
};
```

To access the `lastName` property in the object above we first need to get the `name` property (which is also an object) and then get the lastName property. We can use dot notation:

```js
const lastName = user.name.lastName;
```

To get the `"suspended-or-blocked"` property we first need to get the `login` property (an object) and then get the "suspended-or-blocked" for which we'll need to use bracket notation as it contains hyphens:

```js
const suspendedOrBlocked = user.login["suspended-or-blocked"];
```

The `floor` property nested quite deep. It is a property of the building object which is a property of the locality object which is a property of the address object.

```js
const floor = user.address.locality.building.floor;
```

######
Write a single line of code that will retrieve the `password` property from the object above.

~~javascript objects accessingNestedObjectProperty1~~

######
Write a single line of code that will retrieve the `street` property from the object above.

~~javascript objects accessingNestedObjectProperty2~~

######
Write a single line of code that will retrieve the `"building name"` property from the object above.

~~javascript objects accessingNestedObjectProperty3~~

<nav>
     <a href="/javascript/objects/accessing-properties-with-bracket-notation">Back</a>
</nav>