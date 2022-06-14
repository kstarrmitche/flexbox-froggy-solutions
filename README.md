# README

## What is this? 
This is a collection of MY solutions for the in-browser game, [flexbox froggy](https://flexboxfroggy.com/). Practice makes perfect! 

I'll also be leaving notes for myself in this file as well :) 

-----


### Definitions

- `justify-content` - used to adjust items horizontally (across the x-axis)
   - flex-start: Items align to the left side of the container.
   - flex-end: Items align to the right side of the container.
   - center: Items align at the center of the container.
   - space-between: Items display with equal spacing between them.
   - space-around: Items display with equal spacing around them.
- `align-items` - used to adjust items vertically (y-axis)
    - flex-start: Items align to the top of the container.
    - flex-end: Items align to the bottom of the container.
    - center: Items align at the vertical center of the container.
    - baseline: Items display at the baseline of the container.
    - stretch: Items are stretched to fit the container.
- `flex-direction` - defines the direction items are placed in the container
    - row: Items are placed the same as the text direction.
    - row-reverse: Items are placed opposite to the text direction.
    - column: Items are placed top to bottom.
    - column-reverse: Items are placed bottom to top.
- `order` - Sometimes reversing the row or column order of a container is not enough. In these cases, we can apply the order property to individual items. By default, items have a value of 0, but we can use this property to also set it to a positive or negative integer value (-2, -1, 0, 1, 2).
- `align-self` - This property accepts the same values as align-items and its value for the specific item.
- `flex-wrap` 
   - nowrap: Every item is fit to a single line.
   - wrap: Items wrap around to additional lines.
   - wrap-reverse: Items wrap around to additional lines in reverse.
- `flex-flow` - combines `flex-direction` and `flex-wrap` as a shorthand. It accepts the value of the two properties separated by a space. 
    - example: `flex-flow: column wrap;`
- `align-content` - sets how multiple lines are spaced apart from each other. This property takes the following values:
   - flex-start: Lines are packed at the top of the container.
   - flex-end: Lines are packed at the bottom of the container.
   - center: Lines are packed at the vertical center of the container.
   - space-between: Lines display with equal spacing between them.
   - space-around: Lines display with equal spacing around them.
   - stretch: Lines are stretched to fit the container.

### Tricky things!
- Notice that when you set the flex-direction to a reversed row or column, the "flex" start and end are also reversed of the associated x or y axis. So for example, if you did `flex-direction: row-reverse`,  `justify-content: flex-end` would actually push the content to the left!(See level 10 for an example)
- `align-content` determines the spacing between lines, while `align-items` determines how the items as a whole are aligned within the container. When there is only one line, `align-content` has no effect.

### The differences between `space-around,` `space-evenly`, and `space-between`

```css
justify-content: space-between; /* Distribute items evenly
                                   The first item is flush with the start,
                                   the last is flush with the end */
justify-content: space-around;  /* Distribute items evenly
                                   Items have a half-size space
                                   on either end */
justify-content: space-evenly;  /* Distribute items evenly
                                   Items have equal space around them */ 
```
from: https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content


