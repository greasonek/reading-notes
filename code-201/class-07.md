# Class 7 Reading Notes

## Domain Modeling

> Domain modeling is a communication tool that can be used between technical and business teams

- describes the entities of code, their attributes and behavior, and constraints of domain

- **object-oriented model** - entity that stores data in properties and encapsulates behaviors in methods (<a href="https://github.com/codefellows/domain_modeling#domain-modeling">source</a>)

- **function expression** - variable declared is assigned a function with parameters - parameters are stored in properties (i.e. this.epicRating) which allows for newly created objects to access that data later
  - new object **instantiated** with *new* keyword and properties *initialized* by calling constructor function
  - after all this, objects are stored inside variable and console logged


1. Domain modeling allows the coder to change a small part of a complex code so it can apply to a number to another object that has similar attributes and behaviors without having to change the entire code.

## HTML Table Basics

- **colspan** attribute allows a cell to span over mulitple columns. Example: colspan="2" allows the cell to span two columns

- **rowspan** attrubiute allows cell to span over multiple rows. 

- **< col> and < colgroup> - col specified inside colgroup beneath opening table tag - allows to style columns instead of styling individual cells which is not efficient. 

1. Tables should not be used for page layouts because they reduced accessibility for viewers who are visually impaired. They also involve complex markup structures that can result in the code being harder to read and maintain. Lastly, tables are not automatically responsive.

2. 3 semantic elements for html tables include: < th> which stands for 'table header', this denotes the header and is not a normal cell, they allow the table to be more accessible and screenreaders are able to read a whole row or column of data at once. The < tr> element ('table row') allows to place subsequent cells on a second w=row instead of having one long row. The < td> element ('table data') holds data in a table cell which is the smallest container of a table. 

## Introducing Constructors

- **constructors start with a capital letter!**

1. A **onstructor** is a function called using the keyword *new* which will create a new object, bind "this" to the new object, run your code in the new constructor and return a new object. This will allow you to create new objects without having to write as much code.

2. In object literal, "this" is used to deliver a single object, but in a constructor code, "this" can be instantiated into multiple instances.

## Object Prototypes Using A Constructor

- **prototype** allows us to share methods across all instances of a function (<a href="https://ui.dev/beginners-guide-to-javascript-prototype">source</a>)

1. 

