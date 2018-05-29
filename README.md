This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app).


## ReactJS and React Native Learn List
> Rall is intended to be a gathering of ReactJS and React Native **free** learning resources.  Although there are other resources for this information, Rall hopes to keep information current and relevant by adding tutorials, articles and other free media by date. Rall also includes a study sheet for ReactJS, React Native and related concepts.\

If one would like to contribute, one may submite an article or tutorial to [jwgravesfl@gmail.com](jwgravesfl@gmail.com).   


### Video Tutorials
May 2018
- Coming Soon

I need soemthing new

### Written Tutorials
- Coming Soon

### Audio Tutorials

### Study List
#### Primitive Types
> Immutable
- undefined\
null(object)\
boolean\
number\
string\
symbol

#### Coercion
> Type conversion (or typecasting) means transfer of data from one data type to another. 

#### Explict/Implicit
> Implicit conversion happens when the compiler automatically assigns data types, but the source code can also\
explicitly require a conversion to take place.\
For example, given the instruction 5+2.0, the floating point 2.0 is implicitly typecasted into an integer, but given the instruction Number("0x11"), the string "0x11" is explicitly typecasted as the number 17.

- Which values are falsy?\
undefined\
null\
false\
+0, -0, NaN\
""

- Which values are truthy?\
{}\
[]\
Everything else\

#### Objects
> mutable and stored by reference\
almost everything except prmitives are objects

Explict/Implicit
#### Object Literal
> An object literal is a list of zero or more pairs of property names and associated values of an object, enclosed in curly braces ({}). Do not use an object literal at the beginning of a statement. This will lead to an error or not behave as you expect, because the { will be interpreted as the beginning of a block.

#### Prototype Inheritance
> All JavaScript objects inherit properties and methods from a prototype.\
Date objects inherit from Date.prototype. Array objects inherit from Array.prototype. Person objects inherit from Person.prototype.\
The Object.prototype is on the top of the prototype inheritance chain:\
Date objects, Array objects, and Person objects inherit from Object.prototype./
- Prototype Wrappers
- Objects store a reference to its prototype
- Properties/methods defined most tightly to the instance have priority
- Recomended not to change prototype because it could change other instances of the prototype

#### Methods
> A method is a function which is a property of an object.\
[List of JavaScript Methods](https://docs.microsoft.com/en-us/scripting/javascript/reference/javascript-methods#methods)\
[JavaScript methods index](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Methods_Index)

### Scope
#### Hoisting 
> Lexical scoping (var) - Hoisted\
  Variable and function declarations are moved to the top of their containing scope.\
  The word "lexical" refers to the fact that lexical scoping uses the location where a variable is declared within the source code to determine where that variable is available. Nested functions have access to variables declared in their outer scope.\
  From declared until the function ends.

> Block Scoping (let and const) - Non Hoisted\
  Until the next } is reached.

-- Passing by Reference / by Value.  ^^^^

-- The Global Object ^^^^

#### Closures
> A closure is the combination of a function and the lexical environment within which that function was declared./
myFunc(5) & myFunc(10)/
They share the same function body definition, but store different lexical environments.\
Closures are useful because they let you associate some data (the lexical environment) with a function that operates on that data.\
JavaScript does not provide a native way of doing this, but it is possible to emulate private methods using closures.\
- Three scopes
  1. Own/Local Scope
  2. Outer Function Scope
  3. Global Scope

#### Imediately Invoved Function Expression(IIFE)
> function expression that is invoked immediately\
Creates a closure\
Doesn't add to or modify global object\
- 2 parts\
    1. anonymous function with lexical scope within () preventing pollution of global scope
    2. Create the immediately executing function expression ()

#### First-Class Functions
> A programming language is said to have First-class functions when functions in that language are treated like any other variable.  Can be assigned to variables, array values and object values.  Can be passed as arguments to other functions and can be returned from functions.

#### Higher-Order Functions
> Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions.\
map()\
filter()\
reduce()\
concat()

#### Currying  ^^^^
> 

#### Single Threaded ^^^^
> Javascript is single-threaded, synchronous language

#### Callbacks
> A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.  Callbacks can be synchronous and asynchronous.

#### Synchronous
> A synchronous callback is executed immediately. A function that takes a while can cause the page to fail.  

#### Asynchronous JavaScript
> Asynchronous callbacks are often used to continue code execution after an asynchronous operation has completed.\
1. Execution(Call) Stack\
      A mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions - what function is currently being run, what functions are called from within that function and should be called next, etc.\
  2. Heap\
      a method to store a collection of objects in such a way that the smallest element can be quickly found.\
  3. Queue\
      One or more functions waiting to run.  queue() method shows the queued functions\
  4. Event Loop\
      Never blocking, so when the application is waiting other actions can be taken When functions complete, they are removed from the stack and the frame below continues executing/

#### Promises
> A Promise is a proxy for a value not necessarily known when the promise is created. It allows you to associate handlers with an asynchronous action's eventual success value or failure reason. This lets asynchronous methods return values like synchronous methods: instead of immediately returning the final value, the asynchronous method returns a promise to supply the value at some point in the future.\

> A Promise is in one of these states:\
pending: initial state, neither fulfilled nor rejected.\
fulfilled: meaning that the operation completed successfully.\
rejected: meaning that the operation failed.\
A pending promise can either be fulfilled with a value, or rejected with a reason (error). When either of these options happens, the associated handlers queued up by a promise's then method are called. (If the promise has already been fulfilled or rejected when a corresponding handler is attached, the handler will be called, so there is no race condition between an asynchronous operation completing and its handlers being attached.)

[Further information about Promises on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

#### Async/Await
> The async function declaration defines an asynchronous function, which returns an AsyncFunction object.\
n async function can contain an await expression that pauses the execution of the async function and waits for the passed Promise's resolution, and then resumes the async function's execution and returns the resolved value.

#### this
> 1. In the global execution context (outside of any function), this refers to the global object whether in strict mode or not.
  2. Inside a function, the value of this depends on how the function is called. Call and Apply are used to pass the value of this to another context.
  3. Bind Method creates a new function with the same body and scope and it is permanently bound to the first argument of bind, regardless of how the function is being used.
    Arrow functions this retains the enclosing lexical context's this. 


#### setting 'this' ^^^^

#### Dom / Virtual Dom
> Document Object Model\
Elements(HTML tree like structure)\
The DOM can be modified using JavaScript

#### Classes
> Defines complex objects with their own prototypes

#### Instances

#### Methods

#### Static Methods

#### Properties

#### New

#### Constructor

#### Extends

#### Super

#### Declarative
> React is declarative meaning declare what you want.  

#### Performant
> 

#### Reconciliation 
> Syncing changes in app state to the DOM\
  Reconstructs virtual DOM, diffs against DOM and only makes changes needed.

#### Compoents
> React is componentized for reuse and to break problems down to their simpliest form.  Highly customizable.  


#### JSX 
> - Javascript XML\
  Transpiles to JavaScript\
  < lowercase > are HTML tags, < Uppercase > are Components\
  - Components are functions\
    returns a node that React can render\
    receives properties object

#### Props 
> The Properties object passed to a component and used to computer the returned node.\
  Unidirectional data flow

#### State
> Internally managed configuration of a component.\
  this.state is a prop of component instances\
  Update state with this.setState()\
  1. setState() calls are batched and run asynchronously, causing multiple setState() calls to be ignored.  Pass setState an object or a function of previous state.
  2. Changes in state cause re-renders.











- Expressions
- template literals




Ref



Functional Programming


Contitionals
- &&
- if

Class

Event Handling



Smart / Dumb

Controlled / Uncrolled

Pure Functions

Functional

Component Life Cycle
- Constructor
- Render

Javascript Patterns

### Redux Concepts

Store

Connect
- MapStateToProps

### Contributions:
Add to the list:

Email suggestion to jwgravesfl@gmail.com

### References and Information Sources
[CS50 Mobile App with React Native](https://cs50.github.io/mobile/)\
[MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript)\
[w3schools.com](https://www.w3schools.com/Js)\
[Eloquent JavaScript](https://eloquentjavascript.net/)\
[ReactJS Documentation](https://reactjs.org/)