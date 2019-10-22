## JSX

``` const element = <h1>Hello, world!</h1>; ```

- JSX is a XML/HTML-like syntax used by React.

#### why

- React embraces the fact that rendering logic is inherently couple with other UI logic: how events are handled, how state changes, and how data is prepared for display.

- Doesn't seperate technologies by putting logic and markup in seperate files. 

- react seperates programs into distinct sections (seperates concernes) with loosly coupled units called "components" that contain both.

- JSX is not required

#### Embedding Expressions in JSX

###### Example:
```
const name = 'Eric Banner';
```
- Declared a variable called name `Eric Banner`

```
const element = <h1> Hello, {name}</h1>
```
- Used it in JSX by wrapping it in {}

###### Splitting JSX over multiple lines:

- Is not required but can help for readability.

- when doing this wrap it in Parentheses to avoid possible `automatic semicolon insertion`

- You can use JSX inside of `if` statements, `for` loops, assign it to variables, accept it as argurments, and return it from functions.







