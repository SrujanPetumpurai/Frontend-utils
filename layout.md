# Layout

## Display
`display` controls layout mode.
Values that can be used:
- `block` (takes full width, new line)
- `inline`(no width,heigh flows with the text)
- `inline-block`(inline but supports height and width)
- `flex`(1-D layout system)
- `grid`(2-D layout system)
- `none`(removed from the layout)

## Position
`position` --- controls how a element is placed.
Vales use:
- `static` --- default,normal flow(offset properties won't work)
- `relative` --- offset from itself(means, top/left/right/bottom properties work from the items position & the original space is    reserverd)
- `absolute` --- relative to nearest positioned parent(no space is reserved)
- `fixed` --- relative to viewport(fixed to a position always)
- `sticky` --- sticks after scroll threshold(sticks to a position after you have scroll passed the setOffset)
- `top/left/bottom/right` --- distance from reference edge
  - `px/rem/%`
- `z-index` --- Used for stacking
  - `auto` --- Default stacking(The one that came later appears on top of the earlier ones)
  -`number` --- One with high number stays comes on top(Only elements with position:relative/absolute/fixed/sticky can use this)

## Overflow
`overflow` controls what happens when content goes outside its container.
-`visible` --- Extra content is shown outside the box(default)
-`hidden` --- Extra content is clipped and not visible  
-`scroll` --- Scrollbars are shown even if all the content is visible and nothing overflows(For strict ui/ux designs)
