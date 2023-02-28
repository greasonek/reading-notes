# Class 8 Reading Notes

## Flexbox

- created by using *display* property and setting to *flex*

- initial values:
  - items display as a row; do not wrap; do not grow to fill the container; line up at the start of the container

- to change direction use *flex-direction* property with row, row-reverse, column, column-reverse

- initial value of flex-wrap is nowrap so if there's not enough space in the container the items will overflow; add wrap to make items wrap in the flex conainter

ex) .container {
  display: flex ;
  flex - wrap : wrap ;
}
^^^ <a href="https://web.dev/learn/css/flexbox/">source</a>

1. Flexbox is designed for one-dimensional content, meaning it takes a variety of items of different size and returns the best layout for those items. It provides flexible boundaries for how the content will be displayed.
Only one axis ca be controlled in the flex container but not multiple (i.e. row AND column)

2. **Main axis** is set by the flex-direction property wherein the items move as a group on the main axis. The **cross axis** runs in the opposite direction to the main axis. So if the main axis is row, then cross axis is column.

3. Changing the direction of the visual display can negatively affect accessibility as re-ordering only changes the visual layout, but not the logic. Row-reverse and Column-reverse are two examples.

4. Flexbox allows items to be aligned to a single axis while float moves items to the left or right of a container. 

5. This topic is useful in building my ability to create visual layouts for front end development that are aesthetically pleasing and logically sound. 