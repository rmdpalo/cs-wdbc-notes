# FLEXBOX

_from my internship: everything is a box, containing more boxes, you control which direction the boxes go and how they react to changes to viewing widths_

- flexbox is a one-dimensional layout method for laying out items in rows or columns
- flexbox is a recent addition to CSS, included to address common layout frustrations
- flexbox allows us to distribute space dynamically across elements of an unknown size, hence the term "flex"

## flex-direction

- To use it, you have to type "display: flex;" into a CSS selector.
- In a flex container, we have to know that there are two main axes, the main axis and the cross axis.
- the "flex-direction" property allows us to choose our main axis direction in our container.
  - it defaults to "flex-direction: row;" (left-right)
  - row-reverse - flips the row (right-left)
  - column - top to bottom
  - column-reverse - bottom to top.

## justify-content

- determines how the elements (content) is distributed along the main-axis.
- dependent on flex-direction.
  - flex-start - sets our elements to the start of the main axis.
  - flex-end - sets our elements to the end of the main axis.
  - center - centers our content on the main axis.
  - space-between - will take all the extra space and distribute it __between__ the elements, but not on the outside edges.
  - space-around - gives each element the same amount of space around it. (we end up with half the amount of space on the leftmost and rightmost element)
  - space-evenly - ensures the space is even between the elements __and__ the container.
- _why is it called justify-content?_ and not something more simple.
  - because our main axis can be different from the default it has to make sense for all cases.
  
## flex-wrap
  
- it determines whether our elements are gonna wrap along the main axis to a new line.
- wrap - wraps to a new line if element doesn't fit in container.
- wrap-reverse - flips the __cross axis__ while wrapping. (if our main axis is top-bottom, regular wrap goes left-right, wrap reverse flips right-left)

## align-items

- determines how the elements in a container are distributed along the cross-axis
- flex-start - will align our items along the beginning of the __cross axis__ 
- flex-end - align along the end of the cross axis.
- center - center something along the cross axis, at the center of the element.
- baseline - it'll use the baseline of our text. 

## align-content

- what we use to control/distribute space along the cross axis, but only when we have multiple rows/columns
- does not do anything for us if we don't have flex-wrap on.
  - space-between
  - space-around
  - center 
  - flex-start
  - flex-end
  
## align-self 

- very similar to align-items, but is a property we assign to individual items in the flex container.

## flex-basis

- defines the initial size of an element before additional space is distributed

## flex-grow

- controls the amount of available space an element should take up, IF there is available space. Accepts a unit-less number.

## flex-shrink

- if items are larger than the container, they shrink according to flex-shrink. Accepts a unit-less number.
- you can say it functions the opposite of flex-grow.

## flex (shorthand)
- allows us to set the 3 previous properties all at once.
- values are in this order (flex-grow | flex-shrink | flex-basis) if there are 3 values
  - if one value, unitless number => flex grow
    - flex: 2;
  - if one value, width/height: flex-basis
    - flex: 10em; || flex: 30%; || flex: min-content;
  - if two values => flex-grow | flex-basis
    - flex: 1 30px;
  - if two values, both unitless => flex-grow | flex-shrink
- global values
  - inherit 
  - initial
  - unset

