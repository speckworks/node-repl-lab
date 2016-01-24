# Running JavaScript Code in Node REPL

## Objectives

1. Use REPL
1. Execute code in REPL
1. Exit REPL

## Introduction

Understanding global and scoping will give you a good foundation for future development.

## Instructions

1. Enter REPL
1. Write Node code to perform math by creating a sum function
1. Call the sum function to add numbers
2. Find out what the day of the week was the day of the Declaration of Independence (July 4th, 1776)
1. Exit REPL


### Extra Info



* [Arguments object on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/arguments)
* [Date on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)

## Solution

A sum function for two numbers:

```js
var sum = function(a, b) { return a+b}
```

A sum function for indefinite number of arguments:

```js
var sum = function() { 
  var result = 0
  var args = (arguments.length === 1?[arguments[0]]:Array.apply(null, arguments))
  args.forEach(function summarize(item, index, list) {
    result += parseInt(item, 10)
  })
  return result
}
```

And the Declaration of Independence was on Thursday:

```
> new Date(1776, 6, 4)
Thu Jul 04 1776 00:00:00 GMT-0400 (EDT)
```

Note: The month argument (second in the `Date()` call) is 0-based so July is 6.