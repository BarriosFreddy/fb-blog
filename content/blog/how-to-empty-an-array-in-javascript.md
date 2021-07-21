---
path: how-to-empty-an-array-in-javaScript
date: 2021-07-21T02:40:05.572Z
title: How to empty an array in JavaScript
description: How to empty an array in JavaScript
---
The simplest way to empty an array in JavaScript is by assigning **0** to the property **length** of the array affected. For Example

```
let numbers = [1,3,5,7,9];

numbers.length = 0;

console.log(numbers);
// []

```

This is possible because the **length** property is read/write property in an array. Therefore, you can assign zero and the array will be clear. 