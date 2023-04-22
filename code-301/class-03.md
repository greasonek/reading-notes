# Lists & Keys

- build collections of elements and inlude them in JSX using curly braces {}

- **key** = a special string attribute need to include when creating lists of elements; assign it to the list items inside the .map() method
  *- ex) li key ={number.toString()}*
        *{number}*
        */li*
  - help identify which items have been changed, are added or are removed. Gives element a stable identity

  - key uniquely identifies list item among its siblings, usually ID from data

  - Key should be specified inside the array

  - elements inside the map() call need keys

1. What does .map() return?

- .map() returns a new array without affecting the original array.

2. If I want to loop through an array and display each value in JSX, how do I do that in React?

- Build a collection of elements and include them in JSX using curly braces

3. Each list item needs a unique **key**.

4. What is the purpose of a key?

- A key assigns a list element to help identify which items have been changed, added or removed. The key gives the element stable identity.

## The Spread Operator

- spread operator is quick syntax for adding items to arrays, combining arrays/objects, and speading array out to function's arguments

- Spread operator can:
  - copy an array
  - concatenate/combine arrays
  - be used in math functions
  - be used when using an array as an argument
  - add an itme to a list
  - add to state in React
  - combine objects
  - convert NodeList to an array

1. What is the spread operator?

- uses three dots (...) to expand an iterable object into the list of argument. In other words it expands or "spreads" an array into separate arguemtns; *ex) (...arr)*

2. List 4 things that the spread operator can do.

- concatenate/combine arrays

- be used in math functions

- be used when using an array as an argument

- add an itme to a list
  
- add to state in React

3. Give an example of using the spread operator to combine two arrays.

<a href ="https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab">Source for this example</a>
const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }

4. Give an example of using the spread operator to add a new item to an array.

<a href ="https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab">Source for this example</a>
const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

5. Give an example of using the spread operator to combine two objects into one.

<a href ="https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab">Source for this example</a>
const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

### How to Pass Functions Between Elements

1. In the video, what is the first step that the developer does to pass functions between components?

- Write a function inside of state that we want to change.

2. In your own words, what does the increment function do?

- The increment function that passes in the object, "name" in this example, and loops it through the array in the constructor function. It modifies the array with the map method to create a new array and pass it back through the loop and updates it with the incremented count. setState updates the state object.

3. How can you pass a method from a parent component into a child component?

- Call the method name with ".this" in the object inside the render function

4. How does the child component invoke a method that was passed to it from a parent component?

- Use this.props.method name (in this example it is increment) and in parens do (this.props.object name (in this example it is name))