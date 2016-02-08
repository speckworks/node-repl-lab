# Running JavaScript Code in Node REPL

## Objectives

1. Use REPL
1. Execute code in REPL
1. Exit REPL

## Introduction

Understanding of Node REPL will give you a tool to test your Node code quickly. A good example will be writing a `sum` function and a date function.

## Instructions

* Enter REPL
* Write Node code to perform math by creating a sum function
* Write and call the `sum` function which adds two numbers together and returns the solution. The numbers are arguments to the function. 
* Find out what the day of the week was the day of the Declaration of Independence (July 4th, 1776) by creating a data object for the date. For example, `new Date(2015, 11, 31)` for Dec 31, 2015.
* Exit REPL

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