## Custom Hook
When we want to share logic between two JavaScript functions, we extract it to a third function. Both components and Hooks are functions, so this works for them too!

A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks
## Lifting State Up

**lifting state up** refers to the process of moving shared state to a common ancestor component, rather than keeping it local to a specific component. This is often necessary when multiple components need to access and update the same state.
 - Lifting state up is a common pattern in React that allows you to share state between components and manage it


## Thinking in React
In order to think in React you need to go though a couple of steps, and assuming that you as a developer have a design mock and some JSON data you need to do the following:
### 1: Break The UI Into A Component Hierarchy
The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names. If you’re working with a designer, they may have already done this, so go talk to them! Their Photoshop layer names may end up being the names of your React components!
### 2. Build A Static Version in React:
Now that you have your component hierarchy, it’s time to implement your app. The easiest way is to build a version that takes your data model and renders the UI but has no interactivity. It’s best to decouple these processes because building a static version requires a lot of typing and no thinking, and adding interactivity requires a lot of thinking and not a lot of typing
### 3. Identify The Minimal (but complete) Representation Of UI State:
During this stage you need to start making the UI interactive using states, and to do that think of the minimal set of mutable state that your actually app needs.

### WHAT IS MEMOIZATION?
There are some times when re-rendering of the component results in performance issues. To overcome this, React provides us with a performance feature known as memoization.

Memoization is an optimization technique that allows an increase in the performance of a program by storing the results of some expensive function so that we don’t need to call that function when the same inputs are given.