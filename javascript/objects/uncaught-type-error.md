# Objects: Uncaught TypeError

Trying to access properties or objects that don't exist is a common problem.

In Chrome and Edge the error message looks like this:

```bash
Uncaught TypeError: Cannot read properties of undefined (reading 'property_name')
```

where `property_name` is the name of the property you are trying to retrieve.

In Firefox the error looks like this:

```bash
Uncaught TypeError: object.property_name is undefined
```

Given this object

```js
const user = {
  name: "Blob"
};
```

Running this code below would produce the error above:

```js
const userName = person.name;
```
