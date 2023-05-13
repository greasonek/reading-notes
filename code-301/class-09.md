# Class 09 Reading Notes

## Conceptes of Functional Programming in JavaScript

1. What is functional programming?

- Functional programming is a style of building the structure and elements of computer programs that takes the approach of using pure functions to create maintainalbe software, i.e. building programs by applying functions (<a href="https://www.codingdojo.com/blog/what-is-functional-programming#:~:text=Functional%20programming%20(FP)%20is%20an,by%20applying%20and%20composing%20functions.">Source</a>)

2. What is a pure function and how do we know if something is a pure function?

- A pure function is onethat returns the same result if given the same arguments and does not cause observable side effects (like modifying a global object or parameter passed by reference). An impure function would use a global object that was not passed as a parameter for the function, it would read external files, it would be able to rely on a random number generator.

3. What are the benefits of a pure function?

- Pure functions are easier to test.

4. What is immutability?

- Immutability is the inability to change or lack of changing over time. The state of data cannot change after it's been created if it is immutable. A new object would have to be created with the new value.

5. What is Referential transparency?

- Referential transparency is a pure function + immutable data. We can replacea piece of code with the value it compute and vice-versa without changing the meaning or results of the program.

## Node JS for Beginners - Modules & Require()

1. What is a module?

- There is a different module for different sets of code each with its own set of fucntionality in the application. We call upon module when it's needed. Basically the module is another js file.

2. What does the word ‘require’ do?

- Require imports a file into the app.js file to be used.

3. How do we bring another module into the file the we are working in?

- By using require and pass in string ie. require('./file name');

4. What do we have to do to make a module available?

- In the module we want to be avaialbe, use module.exports = function name of function what to be availabel outside the module, then add var + function name = require ('./file name) in app.js --> example) var counter = require('./count'); (<a href = "https://www.youtube.com/watch?v=xHLd36QoS4k">Source</a>)