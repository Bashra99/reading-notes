# Class 04
## React and Forms

### React Docs - Forms
* What is a _Controlled Component_?
   - An input form element whose value is controlled by React
*Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them?* 
    we should update the state. to keep it sync with the input’s value
    
*How do we target what the user is entering if we have an event handler on an input field?*
By setting a state for it in the constructor to make the react state the source of truth.


### The Conditional (Ternary) Operator Explained
* *Why would we use a ternary operator?*
 to improve the readability of the code
* Rewrite the following statement using a ternary statement:
```
    if(x===y){
    console.log(true);
    } else {
    console.log(false);
    }
```

  
```
(x===y)?  console.log(true) : console.log(false)

```

