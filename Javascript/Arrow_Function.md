# Arrow Function

### Rule 1

When you want to return an object, wrap it inside parenthesis '( )' or place them in more than one line.

```jsx
const makeInstructor = (name) => {name:"Colt"}
makeInstructor() // undefined

const makeInstructor2 = (name) => ({name:"Colt"})
makeInstructor2() // {name: "Colt"}
```

### Rule 2

You should not be using arrow functions: 1) inside object method, 2) when you need your own keyword *this.* 

```jsx
const student = {
  firstName: "Melissa",
  sayHi: () => {
    return "Hello " + this.firstName
  }
}

student.sayHi()  returns// Hello undefined
```

*this* keyword inside arrow function will refer to global object (window/global). Whereas *this* keyword inside regular function declaration will refer to the object. 

### Arrow Function Summary

- Can only be used as shorthand for anonymous function expressions
- Must put parentheses around parameters if there are 0 or 2+ parameters
- Return statement is implied if you leave out curly braces
- They do not make their own

    ***this***