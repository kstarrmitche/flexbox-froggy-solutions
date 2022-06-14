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

### Tricky things!
- Notice that when you set the flex-direction to a reversed row or column, the "flex" start and end are also reversed of the associated x or y axis. So for example, if you did `flex-direction: row-reverse`,  `justify-content: flex-end` would actually push the content to the left!(See level 10 for an example)

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


