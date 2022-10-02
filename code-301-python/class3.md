# Passing Functions as Props

> General Props and states are very strong and can be widely used, however, passing functions as props is next level, it allows you to control events for example the way you want.
---
**What does .map() return?**
map( ) return an array.
**If I want to loop through an array and display each value in JSX, how do I do that in React?**
- By map()
**Each list item needs a unique  key What is the purpose of a key?**
- Keys help React identify which items have changed, are added, or are removed.
**What is the spread operator?**
- a new addition to the set of operators in JavaScript ES6. It takes in an iterable (e.g an array) and expands it into individual elements. The spread operator is commonly used to make shallow copies of JS objects. Using this operator makes the code concise and enhances its readability

**List 4 things that the spread operator can do.**
- You can add items to an array
- combine arrays 
- combine objects  
- and spreading an array out into a function’s arguments
**Give an example of using the spread operator to combine two arrays.**
> const myArray = [`🤪`,`🤗`]  
> const yourArray = [`🤗`,`🤩`]  
>console.log(...ourArray) // 🤪  🙂 🤗 🤩 ]

**Give an example of using the spread operator to add a new item to an array.**
> const fewFruit = ['🍏','🍊','🍌']
> const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
> console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]

**Give an example of using the spread operator to combine two objects into one.**

> onst objectOne = {hello: "🤪"}
> const objectTwo = {world: "🐻"}
> const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
> console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
> const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
> objectFour.laugh() // 😂😂😂😂😂

**In the video, what is the first step that the developer does to pass functions between components?**

__Create a function where ever the state exists__

**In your own words, what does the increment function do?**

- It takes a name, loop through an array and increase the count  

**How can you pass a method from a parent component into a child component?**
- passing props

**How does the child component invoke a method that was passed to it from a parent component?**

- By calling the method

## Things I want to know more about


####resource 

https://www.educative.io/answers/what-is-the-spread-operator-in-javascript
https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab