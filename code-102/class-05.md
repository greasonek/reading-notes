# Class 5 Reading Notes

## What is CSS?

> Cascade Style Sheets - controls how the html will look; presentaion; 

- change color, size create layout (ex. have main content area with sidebar for related ifo); create animation

### CSS Syntax

> CSS = rule based language - define rules by specifying groups of styles that should be applied to particular elements/groups of elements on your page

- ex. h1 {
    color : red ;
    font - size : 5em;
      } -- > inside the brackets we have DECLARATOINS in the form of PROPERTY and VALUES
      color is the property; red is the value; font-size is the property; 5em is the value

### 3 Ways to Insert CSS

1. External CSS 

    - change look of entire website by changing one file; each html page but include reference to external style sheet file inside a <link> element in <head> section -- link must be saved with CSS extension

2. Internal CSS 

    - defined within the <style> element, inside <head> section of html page

3. Inline CSS

    - used to apply unique style for single element; to use, add style attribute to relevant element 

### Multiple Style Sheets

- If the there are mutliple styles, the last defined style will be used UNLESS it is a internal style that is used first, in which case that one will take priority

### Cascading Order

- Priority of styles is:

1. Inline (inside HTML element) -- overrides external and interal!

2. External and Internal style sheets (in head section)

3. Browser default

#### CSS Color 
- defined by a color name, a hex code or rgb color code

#### CSS Syntax
- color specifies text color
- initial sets property to its default value
- inherit inherits this property from its parent element




> 