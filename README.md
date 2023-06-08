# Notes

This repository will contain notes as I learn more about javascript.

## Principles

### Thread of execution

- goes through the code line by line
- stuff gets saved to memory as it encounters variables / functions
- new function call -> new execution context
  - new local memory that isn't available outside the execution context
- whenever we "return" we evaluate the function and turn it into a value which we assign to the identifier(variable)
- javascript only has 1 thread of execution (Weaves in and out of different execution context) 
- javascript uses call stack to keep track of what function is currently running aka where is the thread of execution
- whenever we run a function -> we add to the call stack -> function finishes running -> remove from call stack -> go back to the execution context where it was called
- therefore, whatever is on the top of the call stack, that is we are currently running


## Callbacks and Higher order functions

## CLosure(scope and execution context)

## Asynchronous Javascript & the event loop

## Classes and Prototypes (OOP)
