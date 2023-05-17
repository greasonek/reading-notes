# Class 10 Reading Notes

## Understanding JavaScript Call Back

1. What is a ‘call’?

- A call is a function invocation in a call stack (function hierarchy and execution order)

2. How many ‘calls’ can happen at once?

- The call stack is single, calls are done one at a time from top to bottom

3. What does LIFO mean?

- Last In First Out

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

function firstFunction(){
}
function secondFunction(){
  firstFunction();
}
function thirdFunction(){
  secondFunction();
}
thirdFunction();
<a href="https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4">Source</a>

5. What causes a Stack Overflow?

- Occurs when a function calls itself without an exit point.

## Script Error Messages

1. What is a ‘reference error’?

- An error that occurs when you're trying to reference a variable that has not yet been declared.

2. What is a ‘syntax error’?

- Occurs when trying to parse an invalid object or something as simple as having an extra comma when calling a function.

3. What is a ‘range error’?

- Occurs when manipulating an object with a length and giving it an invalid length like a negative length.

4. What is a ‘type error’?

- Occurs when the type you're trying to use are incompatible like accessing a property in an undefined type of variable.

5. What is a breakpoint?

- Stops the program at a point you've selected so you can debug that cycle of code. 

6. What does the word ‘debugger’ do in your code?

- Putting 'debugger' in your code creates a breakpoint on the line you want to break.
