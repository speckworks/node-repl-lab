# Running JavaScript Code in Node REPL

## Objectives

1. Use REPL
1. Execute code in REPL
1. Exit REPL

## Introduction

A good understanding of Node REPL will give you a tool to test your Node code quickly. We'll practice using the REPL by writing a `sum` function and using JavaScript's `Date` instance.

## Instructions

* Enter REPL
* Write Node code to perform math by creating a sum function which adds two numbers together and returns the solution. The numbers should be passed as parameters to the function. 
* Write and call the `sum` function.
* Find out what the day of the week was the day of the Declaration of Independence (July 4th, 1776) by creating a date object for the date. For example, `new Date(2015, 12, 31)` for Dec 31, 2015. See the resources below for help with `Date`.
* Exit REPL

### Resources

* [Arguments object on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/arguments)
* [Date on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/node-repl-lab' title='node-repl-lab'>node-repl-lab</a> on Learn.co and start learning to code for free.</p>

> const decOfInd = new Date('1776, 7,4')
undefined
> const dayFree = decOfInd.getDay()
undefined
> console.log(dayFree)
4
