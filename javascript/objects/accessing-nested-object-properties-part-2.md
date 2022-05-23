




To get the `"suspended-or-blocked"` property we first need to get the `login` property (an object) and then get the "suspended-or-blocked" for which we'll need to use bracket notation as it contains hyphens:

```js
const suspendedOrBlocked = user.login["suspended-or-blocked"];
```

The `floor` property is nested quite deep. It is a property of the building object which is a property of the locality object which is a property of the address object.

```js
const floor = user.address.locality.building.floor;
```

######
Write a single line of code that will:
- retrieve the `password` property from the object above
- assign it to a variable called `userPassword`

~~javascript objects accessingNestedObjectProperty1~~

######
Write a single line of code that will
- retrieve the `street` property from the object above
- assign it to a variable called `userStreet`

~~javascript objects accessingNestedObjectProperty2~~

######
Write a single line of code that will
- retrieve the `"building name"` property from the object above
- assign it to a variable called `userBuildingName`

~~javascript objects accessingNestedObjectProperty3~~