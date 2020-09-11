# What is TDD?
TDD stands for Test Driven Development. The process is simple:
![](https://r-stylelab.com/wp-content/uploads/2018/07/tdd-cycle1.png)
1. write some code that proves that the implementation works or fails. Watch the test fail before moving to the next step 
2. Write the implementation code and watch the test pass.
3. Refactor if needed. You should feel confident refactoring your code now that you have a test to tell you if you’ve broken something.
---
# This, Bind, Call, and Apply in JavaScript

In JavaScript, `this` is a reference to an object. The object that `this `refers to can vary, implicitly based on whether it is global, on an object, or in a constructor, and can also vary explicitly based on usage of the `Function` prototype methods `bind`,`call`, and `apply`
## Implicit Context
There are four main contexts in which the value of `this` can be implicitly inferred:
* the global context
* as a method within an object
* as a constructor on a function or class
* as a DOM event handler

### Global
In the global context, `this` refers to the global object. When you're working in a browser, the global context is `window`. When you're working in Node.js, the global context is `global`.
### An Object Method
A method is a function on an object, or a task that an object can perform. A method uses `this `to refer to the properties of the object.
### A Function Constructor
When you use the `new `keyword, it creates an instance of a constructor function or class. 
Function constructors were the standard way to initialize a user-defined object before the `class `syntax was introduced in the ECMAScript 2015 update to JavaScript. 
### A Class Constructor
A constructor on a class acts the same as a constructor on a function. 
### A DOM Event Handler
In the browser, there is a special `this `context for event handlers. In an event handler called by `addEventListener`, `this `will refer to` event.currentTarget`. More often than not, developers will simply use `event.target` or `event.currentTarget` as needed to access elements in the DOM, but since the `this `reference changes in this context, it is important to know.
## Explicit Context:
### Call and Apply
`call` and `apply` are very similar—they invoke a function with a specified this context, and optional arguments. The only difference between `call `and `apply `is that `call` requires the arguments to be passed in one-by-one, and `apply `takes the arguments as an array.


### Bind
Both `call` and `apply` are one-time use methods—if you call the method with the `this` context it will have it, but the original function will remain unchanged.

Sometimes, you might need to use a method over and over with the `this` context of another object, and in that case you could use the `bind` method to create a brand new function with an explicitly bound `this`.

-------------
## Inheritance
####  Inheriting properties 
JavaScript objects are dynamic "bags" of properties (referred to as own properties). JavaScript objects have a link to a prototype object. When trying to access a property of an object, the property will not only be sought on the object but on the prototype of the object, the prototype of the prototype, and so on until either a property with a matching name is found or the end of the prototype chain is reached.
####  Inheriting "methods" 
JavaScript does not have "methods" in the form that class-based languages define them. In JavaScript, any function can be added to an object in the form of a property. An inherited function acts just as any other property, including property shadowing as shown above (in this case, a form of method overriding).


-----
## Classes
Classes are in fact "special functions", and just as you can define function expressions and function declarations, the class syntax has two components: class expressions and class declarations.


