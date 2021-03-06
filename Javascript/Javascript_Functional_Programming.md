# Functional Programming

## Functional vs OOP

* Read [Functional vs OOP](http://raganwald.com/2013/04/08/functional-vs-OOP.html)

|     | data and operations upon it are | central model for abstraction  | central activity  | describe |
| --- |:-------------------------------:|:------------------------------:|:-----------------:|:--------:|
| OOP | tightly coupled                 | data structure                 | composing new objects and extending existing objects by adding new methods to them  | how to do it
| FP  | loosely coupled                 | function                       | writing new (higher-order) functions | what to do

* Those things that change relatively often can be written in an OO style.
* Those that are unlikely to change but are subject to being operated upon by a changing cast of entities should be written in a more FP style.

## FP in JavaScript

JS contains:
* YES: first-class function, lambdas/anonymous functions with closures
* NO: recursion through tail call optimization, pattern matching, lazy evaluation, homoiconicity

Definitions:
* **pure function** is a function have no side effects. It always returns the same result given the same arguments.
* **closure** is a function containing one or more free variables. Free variable are not bound within the function environment. [Read](https://leanpub.com/javascript-allonge/read#closures)
* **higher-order function** is a function that either takes functions as arguments or returns a function (or both).
* **combinator** is a higher-order pure function that takes only functions as arguments and returns a function.
* **function decorator** is a higher-order function that takes one function as an argument, returns another function, and the returned function is a variation of the argument function.
* **currying** is the process of converting functions that take multiple arguments into ones that, when supplied fewer arguments, return new functions that accept the remaining ones.
* **partial application**

Building blocks:
* **composition** - chaining functions
* **partial application** - applying only some of the arguments of a function

## [Advantages](http://scott.sauyet.com/Javascript/Talk/FunctionalProgramming/#slide-143)

* Elegance and simplicity
* Easier decomposition of problems
* Code more closely tied to the problem domain

And through these, we can also achieve

* Straightforward unit testing
* Easier debugging
* Simple concurrency

## Disadvantages?

* **debugging** - the stack traces are harder to follow? (comment - is this true?) Using named functions?
* **performance** - any issues? Brian Lonsdorf (see videos) reports no relevant performance issues.

## Learn

Read:
* [Scott Sauyet- Functional Programming](http://scott.sauyet.com/Javascript/Talk/FunctionalProgramming/)
* [Javascript Allonge](https://leanpub.com/javascript-allonge/read) - learn how to write higher-order functions.

Watch:
* [Brian Lonsdorf - Hey Underscore, You're Doing It Wrong!](https://www.youtube.com/watch?v=m3svKOdZijA)
* [Reginald Braithwaite - Javascript Combinators](https://vimeo.com/97408202)

## Libraries

* https://lodash.com/
* http://underscorejs.org/
* https://github.com/raganwald/allong.es
* http://ramdajs.com/
 
