# Learn

This document was created to help and faciliate a learning session on Data.
This guide will cover Data, Data Types, Data Structures, and Design Patterns.

### Resources: 
- https://www.javascript.com/learn
- https://developer.mozilla.org/en-US/docs/Web/JavaScript
- https://www.dofactory.com/javascript/factory-method-design-pattern 
- http://file.allitebooks.com/20190124/JavaScript%20Data%20Structures%20and%20Algorithms.pdf
- https://github.com/kdn251/interviews/blob/master/README.md
- https://khan4019.github.io/front-end-Interview-Questions/js1.html
- https://khan4019.github.io/front-end-Interview-Questions/js2.html


## Data

Data is contextless information. "Data" can be stored in several different ways but eventually given context by typing (Typing, Type, Data Types).

Data types could be "Primative" or "Non-Primative" (such as) an Object, with structure (data structure).

### Primitives

A [primitive] (primitive data type) is "data" that is not an object and has no methods.

  - [string]

    A string is simply words, (Using quotes, single quotes, or backticks)

  - [number]

    A number is any numeric value, that is not a string.

  - [boolean]

    A boolean is simply `true` or `false`. In javascript `0` is also false, and anything not `0` is true.
    Aside: There is a lot more to this, such as `!` and `!!` operators.

  - [null]

    The value null represents the intentional absence of any object value.

  - [undefined]

    A primitive value automatically assigned to variables that have just been declared or to formal arguments for which there are no actual arguments.

  - [symbol] (new)

    Every symbol value returned from Symbol() is unique.  A symbol value may be used as an identifier for object properties; this is the data type's only purpose.

    Feel free to read [more about symbols].

Source: https://developer.mozilla.org/en-US/docs/Glossary/Primitive

### Function

Functions are one of the fundamental building blocks in JavaScript. A function is a JavaScript procedure—a set of statements that performs a task or calculates a value. To use a function, you must define it somewhere in the scope from which you wish to call it.

https://developer.mozilla.org/en-US/docs/Glossary/Function

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions

#### IIFE:

Imediately invoked function expressions.

https://en.wikipedia.org/wiki/Immediately_invoked_function_expression

#### Scope:

The scope is what defines the access to JavaScript variables. In JavaScript, variables can belong to the global scope or to the local scope. Global variables are variables that belong in the global scope and are accessible from anywhere in the program.

https://en.wikipedia.org/wiki/Scope_(computer_science)

### Array

An array is a collection of elements (values or variables), each identified by at least one index or key.
The JavaScript Array object is a global object that is used in the construction of arrays; which are high-level, list-like objects.

As a JavaScript developer, you will use the array often; it is the most commonly used data structure.

### Object

In JavaScript, most things are objects, from core JavaScript features like strings and arrays to the browser APIs built on top of JavaScript.
You can even create your own objects to encapsulate related functions and variables into efficient packages.

The object-oriented nature of JavaScript is important to understand if you want to go further with your knowledge of the language and write more efficient code.

An object is a collection of related data and/or functionality (which usually consists of several variables and functions — which are called properties and methods when they are inside objects.)

Learn [object basics].

"JavaScript objects are what makes the JavaScript programming language so versatile. Before diving into data structures and algorithms, let’s review how JavaScript objects work. This chapter will focus on what JavaScript objects are, how they are declared, and how their properties can be changed. In addition, this chapter will cover how JavaScript classes are implemented using prototypal inheritance." ( JavaScript Data Structures and Algorithms)


### JSON data

JavaScript Object Notation (JSON).

## Big-O

Big O Notation is used to describe the upper bound of a particular algorithm.
Big O is used to describe worst case scenarios. This refers to the "Time Complexity" of a given argorithm. How long "could" it take to run, or in otherwords how many iterations it could potentionally take to complete.

When you see `O(1)` or `O(n)` that's big-O.

`n` in this notation referes to the size of (or length of) a given "list" (array, object, data-type).

`O(n^2)` This notation is stating that "worse case" is that you'll compute every single element in a given list twice. `n^2` or `n * n` computations.
`O(nlog(n))` This notation is stating that "worse case" is that you'll compute the `n of log(n)` If you need more help understanding [logarithms].
This is a great article on their mathmatical properties.

<img src="https://github.com/kdn251/interviews/blob/master/images/bigO.png?raw=true">


## Data Structures

See this section on [data structures].

[data structures]: /data-structures/
[string]: https://developer.mozilla.org/en-US/docs/Glossary/string
[number]: https://developer.mozilla.org/en-US/docs/Glossary/number
[boolean]: https://developer.mozilla.org/en-US/docs/Glossary/number
[null]: https://developer.mozilla.org/en-US/docs/Glossary/null
[undefined]: https://developer.mozilla.org/en-US/docs/Glossary/undefined
[symbol]: https://developer.mozilla.org/en-US/docs/Glossary/symbol
[more about symbols]: https://en.wikipedia.org/wiki/Symbol_(programming)
[primitive]: https://developer.mozilla.org/en-US/docs/Glossary/Primitive
[logarithms]: https://www.khanacademy.org/math/algebra2/exponential-and-logarithmic-functions/introduction-to-logarithms/a/intro-to-logarithms
[Object]: https://www.javascript.com/learn/objects
[object basics]: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics
