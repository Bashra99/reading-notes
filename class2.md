# State and Props
---
**Lifecycle of Components**
> Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting.
### React lifecycle
* what happens first, the _render_ or the _componentDidMount_?
  **render**


* What is the very first thing to happen in the lifecycle of React?
**constructor**
* Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
_constructor_ --> _render_ --> _React Updates_  --> _componentDidMount_ -->  _componentWillUnmount_
* What does componentDidMount do? 
   allows us to execute the React code when the component is already placed in the DOM 
## React State Vs Props
* What types of things can you pass in the props?

  The initial values of components could be any data type

* What is the big difference between props and state?  
  The  difference between props and state is that state is internal and controlled by the component it self while props are external and controlled by whatever renders the component.
* When do we re-render our application?
when we change the state inside our application.
* What are some examples of things that we could store in state?
timer , counter
## Things I want to know more about:

---










**resource**
- https://www.w3schools.com/react/react_lifecycle.asp
- https://stackoverflow.com/questions/27991366/what-is-the-difference-between-state-and-props-in-react#:~:text=The%20key%20difference%20between%20props,by%20whatever%20renders%20the%20component.
