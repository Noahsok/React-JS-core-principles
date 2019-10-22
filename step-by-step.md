# Step By Step guide for React.js
These concepts have been taken from react.js Docs. I have used this as a way to deeper understand the concepts of React.js. As my understanding and this "guide" progresses I hope to incorporate code snippets(no guarantee). 

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
``` const name = 'Eric Banner';
``` const element = <h1> Hello, {name}</h1>```




