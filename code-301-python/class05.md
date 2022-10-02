# class 05

# Putting it all together

**What is the single responsibility principle and how does it apply to components?**

- that means each component should be responsible for doing only one thing same as functions .
  **What does it mean to build a _static_ version of your application?**
  that means displays the UI but it is not interactive

**Once you have a static application, what do you need to add?**

- add functionality by passing states.

**What are the three questions you can ask to determine if something is state?**

- s it passed in from a parent via props? If so, it probably isn’t state.
- Does it remain unchanged over time? If so, it probably isn’t state.
- Can you compute it based on any other state or props in your component? If so, it isn’t state.

**How can you identify where state needs to live?**

- Identify every component that renders something based on that state.
- Find a common owner component (a single component above all the components that need the state in the hierarchy).
- Either the common owner or another component higher up in the hierarchy should own the state.
- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

**What is a “higher-order function”?**
- Functions that operate on other functions, either by taking them as arguments or by returning them.

**Explore the `greaterThan` function as defined in the reading. In your own words, what is line 2 of this function doing?**
- it returns true if the left operand is greater than the right operand  and false otherwise




**Explain how either map or reduce operates, with regards to higher-order functions.**

- map() loops through an array and take an argument to execute something or mutable the data in the original array


## References

1. <https://riptutorial.com/javascript/example/13351/higher-order-functions#:~:text=In%20general%2C%20functions%20that%20operate,are%20called%20higher%2Dorder%20functions.>
2. <https://reactjs.org/docs/thinking-in-react.html>
