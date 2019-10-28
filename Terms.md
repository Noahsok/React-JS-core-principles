## React Terms 
This is a "dictionary" of sorts 

## Lifecycle Methods

React Lifecycle methods are the series of events that happen from the birth of a react component to its death/end.

Every component in React goes through a lifecycle of events.
- Mounting: Birth of the component.
- Updating: Growth of the component.
- Unmounting: Death of the component.

## Common LifeCycle Method Terms 

#### Render()

render() is the most used lifecycle methods, You will see it in all React classes. This is because render() is the only required method within a class component in React.

It handles the rending of the component to the UI.

#### Mounting
- The main job of React is to figure out how to modify the DOM This is called "mounting" in React to match what the components want to be rendered on screen. 
- Mounting is essentially adding nodes to the DOM

###### componentDidMount()

-componentDidMount() is called as soon as the component is mounted and ready. This is a good time place to initiate your API calls, if you need to load data from a remote endpoint.

- this allows the use of `setState()`. Calling the `setState()` here will update state and call another rendering but it will happen before the browser updates the UI.

#### Updating

###### componentDidUpdate()

- This lifecycle method is evoked as soon as the updating happens.
- the most common use case for componentDidUpdate() method is updating the DOM in response to prop or state changes.


#### Unmounting

- Removeing nodes from the DOM and "updating" (making changes to nodes already in the DOM)

###### componentWillUnmount()

- As the name suggests this lifecycle method is called just before the component is unmounted and destroyed. If there are any cleanup actions that you would need to do, this would be the right spot.
