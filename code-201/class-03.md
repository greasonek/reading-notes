# Class 3 Reading Notes

## Learn HTML - ordered/unordered lists

> The <ul> and <ol> elements are used to create lists within an HTML code - they each serve a unique listing purpose. 

- <ol> = ordered list element - usually ordered with numbers - accepts global attributes (reversed, typed, start)

- **Reversed** - items will be ordered hight to low; boolean attribute 

- **Start** - start counting from the first integer *always Arabic*; <a href=”https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol”><For example></a>, to start numbering elements from the letter "d" or the Roman numeral "iv," use start="4".

- **Types** - sets the numbering type

- <ul> = unordered list element - usually ordered with bulletin points - use CSS styling to change style of bulletin point

1. Use <ul> unordered lists when the meaning of the list would not change if you weren’t using the ordered list(<ol>) elements

2. Change the style of bulletin point by using CSS styling as the compact and type attributes are no longer used - use CSS style *list-style-type

3. A recipe would need to be ordered because the steps cannot be performed out of sequence, however a grocery list could be an unordered list because the order of items in the list does not matter

4. The numbers of the list items of an ordered list can be changed by using the *type* attribute - use *a* or *A* for lower/uppercase letter, *i* or *I* for roman numerals or *1* for numbers (this is also the default)

## CSS - The Box Model 

> To create complex CSS code, it is important to understand that everything in CSS is created with its own boxes. 

- categories : **block boxes** and **inline boxes**; type refers to how box behaves in page flower; boxes have **inner display type** and **outer display type**

- *display* property can have different values 

- *outer display type* - will break onto new line (unless display time is inline); width and height respected; padding margin and border will push away items outside of the block (unless display time is inline for vertical, horizontal would still move); 

- *inner display type* - dictates how elements INSIDE the box are laid out

1. In the “Box Model” story, the content is a child protected by a guard dog (the padding), the border is the house in which the child lives and is guarded by the padding. The margin is the parent that owns the house, the dog, and the child and guards all of these things from any outside elements (in this story, these elements would be intruders).

2. The four parts of the element box are content box, padding box, margin box and border box. The content box is where content is displayed, sized by using width, heigh, inline-size and block-size. The padding sits around the content as white space. The border wraps the content and padding. The margin is the outermost layer wrapping all the other box types as space between the box and other elements. 

## Learn JS

> Arrays store data items

- Single objects that contain multiple values stored in a list; square brackets with items listed separated by commas, numbered starting with “0” (the number of the object listed is it’s *index*; can find the length of the array by using <a href=”https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Arrays"><this example></a>> const shopping = ['bread', 'milk', 'cheese', 'hummus', 'noodles']; console.log(shopping.length);  // 5

- Multidimensional array is an array within an array

- Add to an array by using **push()** <a href=”https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Arrays"><this example></a> const cities = ['Manchester', 'Liverpool'];  
cities.push('Cardiff'); console.log(cities);      // [ "Manchester", "Liverpool", "Cardiff" ]

- Use **unshift()** to add an item to the beginning of an array

- Remove last item of an array by using **pop()**

- Use **Shift() to remove the first  item of an array

- Can use **splice()** to remove item from an array by using its index

- Accessing every item of an array use the for…of statement

1. Strings, numbers, and objects a few data types that can be stored in an array. 

2. To access every value of the array, use the for…of statement as follows:
For (const people of people) {
console.log(people);
} 

- An *expression* is a code that resolves into a value; 2 kinds: ones that have side effects (like assigning values) and ones that purely evaluate (ex) x=7 → 7 is assigned to x; x=3+4 → x evaluates to 7)

3.  Five assignment operators:

- Addition (x+  =  f()) → (x = x + f()) adds value of right operand to a variable and assigns result to the variable.

- Subtraction (x-=f()) → (x = x - f()) subtracts value of right operand to a variable and assigns the result to the variable.

- Bitwise AND assignment( x& = f()) → (x = x & f()) uses binary representation of both operands.

- Remainder (x%=f()) → (x = x % f()) divides variable by the value of the right operand and assigns result to the variable

- Nullish (x ?? =y) only assigns if x is null or undefined

4. 

- Conditions allow to represent decision making in JS from the choice that must be made to the resulting outcome; 

- If…else statements (if is the conditional)

5. If you have 0 lives left in a game, then you are dead.

6. A loop in JS is good for going through the same thing over and over again, like a list of people or a list of food items. 
