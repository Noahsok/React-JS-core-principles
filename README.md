# React-JS-core-principles
Basic notes for React.JS/ JS core principles
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

## React Core Principles

### React.Component Subclasses

#### Components

- We use components to tell React what we want to see on the screen. When our data changes, React will efficiently update and re-render our components.

- A component takes in parameters, called `props` (short for “properties”), and returns a hierarchy of views to display via the `render` method.

##### Render()
- The render method returns a description of what you want to see on the screen. React takes the description and displays the result. In particular, render returns a React element, which is a lightweight description of what to render. Most React developers use a special syntax called “JSX” which makes these structures easier to write. The <div /> syntax is transformed at build time to React.createElement('div').
