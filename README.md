# Notes

This repository will contain notes as I learn more about javascript.

### Javascript Principles

- goes through the code line by line
- stuff gets saved to memory as it encounters variables / functions
- new function call -> new execution context
  - new local memory that isn't available outside the execution context
- whenever we "return" we evaluate the function and turn it into a value which we assign to the identifier(variable)
- javascript only has 1 thread of execution (Weaves in and out of different execution context) 
- javascript uses call stack to keep track of what function is currently running aka where is the thread of execution
- whenever we run a function -> we add to the call stack -> function finishes running -> remove from call stack -> go back to the execution context where it was called
- therefore, whatever is on the top of the call stack, that is we are currently running


### Functions and Callbacks
- need to generalize functions so we don't repeat ourselves
- hence the need for higher order functions
- functions are first class objects
- can co-exist with and can be treated like any other javascript object
- can be assigned to variables and properties of other objects, passed as arguments into functions, returned as values from functions
- arrow functions
- should you declare functions using `function` keyword or arrow syntax?
  - mostly preference with some minor difference: arrow functions do not have their own bindings to `this`, `arguments`, or `super` 

### Closure
- most esoteric of javascript concepts
- enables powerful prolevel functions like once and memoize
- many js design patterns including the module pattern use closure
- build iterators, handle partial application and maintain state in an asynchronous world
- when function finishes, local memory is deleted except the returned value (what if we return a function?)
- when function gets declared is also stores the local memory in the "backpack" so when it's called and a variable cannot be found in the local memory, it checks the "backpack" before going down a level in the call stack
- basically closure is a collection of all the variables in scope at the time of creation of the function.
- backpack is technically a persistent lexical scope referenced data

### Asynchronous Javascript & the event loop

### Promises

### Classes and Prototypes (OOP)
