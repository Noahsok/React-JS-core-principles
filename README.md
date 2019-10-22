# React-JS-core-principles
Basic notes for React.JS/ JS core principles
- readme are basic notes and are not indepth.
- Step-by-step files walk through core principles for react.js.
## Javascript  Cor Principles

#### Arrow function expressions

- With arrow functions there are no binding of `this` . In regular functions the `this` keyword represented the object that called the function, which could be the window, the document, a button or whatever. With arrow functions the `this` keyword always represents the object that defined the arrow function.

- `=>` 

#### Class function

- A JavaScript class is a type of function

[classReference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

#### let statement

- The let statement declares a block scope local variable, optionally initializing it to a value.

[letReference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let)

#### const

- Constants are block-scoped, much like variables defined using the `let` statement. The value of a constant can't be changed through reassignment, and it can't be redeclared.

[constReference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const)

#### slice()

- slice() method returns a shallow copy of a portion of an array into a new array object selected from begin to end (end not included) where begin and end represent the index of items in that array. The original array will not be modified.

#### map method

- map method creates a new array with the results of calling a provided function on every element in the calling array

## React Core Principles

### React.Component Subclasses

#### Components

- We use components to tell React what we want to see on the screen. When our data changes, React will efficiently update and re-render our components.

- A component takes in parameters, called `props` (short for “properties”), and returns a hierarchy of views to display via the `render` method.

- Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

##### Render()

- The render method returns a description of what you want to see on the screen. React takes the description and displays the result. In particular, render returns a React element, which is a lightweight description of what to render. Most React developers use a special syntax called “JSX” which makes these structures easier to write. The <div /> syntax is transformed at build time to React.createElement('div').

#### Super

- In JavaScript classes, you need to always call `super` when defining the constructor of a subclass. All React component classes that have a constructor should start it with a `super(props)` call.

#### JSX

- JSX comes with the full power of JavaScript. You can put any JavaScript expressions within braces inside JSX. **Each React element is a JavaScript object that you can store in a variable or pass around in your program.

#### State

- state holds information about the component.

-  by default a `component` has no `state` 

- use `state` when a `component` needs to keep track of information between renderings, that is when a `component` itself can create, update, and use `state`.

- `state` is created in the `component`

##### Constructor method

- the constructor method is a special method for creating and initializing an object created within a class.

#### Handling Events

####### Handling events with React elements is very similar to handling events on DOM elements. There are some syntactic differences:

- Events are named using camelCase, rather than lowercase.

- With JSX you pass a function as an event handler, rather than a string. 

####  immutability objects

###### immutability

- immutability means that something cannot change its value or state.

- Avoiding direct data mutation lets us keep previous versions and reuse them

- Detecting changes in immutable objects is considerably easier. If the immutable object that is being referenced is different than the previous one, then the object has changed.

#### concat

- concat() method doesn’t mutate the original array, so we prefer it.

#### key

- `key` is a special and reserved property in React. When an element is created, React extracts the `key` property and stores the `key` directly on the returned element. Even though `key` may look like it belongs in `props`, `key` cannot be referenced using `this.props.key`. React automatically uses `key` to decide which components to update. A component cannot inquire about its `key`.

- keys do not need to be globally unique; they only need to be unique between components and their siblings.







