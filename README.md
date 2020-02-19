# CSS Transitions

css position
in a div, background is at the bottom, then border, then the text content. 
background, border, 块级子元素，浮动元素，内联子元素

positions: 
static (default), relative, absolute, fixed, sticky

relative: the space that the element is taking does not change, but where the element  appears changes. 
relative is relative to your original position, while absolute is absolute to the parent element 
white-space: 文字内容是否换行，nowrap就是不准换行

try not to use position fixed on mobile pages.

four important scenarios that creates a new z-index: z-index = 0; flex, opacity, and transform.
csstriggers.com it’s a website that tells you which part has been triggered during rendering. 

The transition property is specified as one or more single-property transitions, separated by commas.

Each single-property transition describes the transition that should be applied to a single property (or the special values all and none). It includes:

zero or one value representing the property to which the transition should apply. This may be any one of:
the keyword none
the keyword all
a <custom-ident> naming a CSS property.
zero or one <single-transition-timing-function> value representing the timing function to use
zero, one, or two <time> values. The first value that can be parsed as a time is assigned to the transition-duration, and the second value that can be parsed as a time is assigned to transition-delay.
See how things are handled when lists of property values aren't the same length. In short, extra transition descriptions beyond the number of properties actually being animated are ignored.
