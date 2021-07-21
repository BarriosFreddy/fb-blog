---
path: array_methods_find_index
date: 2021-07-21T02:31:18.633Z
title: "Array methods: findIndex"
description: "Array methods: findIndex"
---
The **findIndex** receives a function (predicate) that accepts three arguments and returns a value that is coercible to the Boolean value true or false.

The predicate returns true. If such an element is found, findIndex immediately returns the index of the first element value. Otherwise, findIndex returns -1, indicating that no element passed the test.

```
const array = [
    {name: 'Freddy', age: 10}, 
    {name: 'Francisco', age: 3}, 
    {name: 'Emilia', age: 4}
];

const preschoolerIndex = array.findIndex(kid => kid.age < 5);

console.log(preschoolerIndex);
// 1

```

### Parameters

1. **callback**
Testing function to execute on each value in the array, taking 3 arguments:
> **element**
The current element in the array.
 **index** (Optional)
The index (position) of the current element in the array.
 **array** (Optional)
The array that _find_ was called on.

2. **thisArg** (Optional)
Object to use as this inside callback.


The findIndex function is intentionally generic; it does not require that its this value be an Array object. Therefore it can be transferred to other kinds of objects for use as a method.
