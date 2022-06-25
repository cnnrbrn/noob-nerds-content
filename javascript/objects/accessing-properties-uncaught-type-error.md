# Accessing properties: Uncaught TypeError

Trying to access properties or objects that don't exist is a common problem.

In Chrome and Edge the error message looks like this:

```
Uncaught TypeError: Cannot read properties of undefined (reading 'property_name')
```

where `property_name` is the name of the property where are trying to retrieve.

In Firefox the error looks like this:

```
Uncaught TypeError: object.property_name is undefined
```
