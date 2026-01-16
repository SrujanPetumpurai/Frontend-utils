## Layout_Systems(FlexBOX & GRID)

## FlexbOX
- `display-flex` -- Turns a element into a flex container;children turn into flex items.
- `flex-direction` (row/column) -- sets the main axis direction
- `justify-content:` -- aligns items in the main axis
  - `flex-start`
  - `flex-end`
  - `center` -- Centers the elements in the main axis
  - `space-between` -- first and last at edges and equal gaps between
  - `space-around` -- equal space around items
  - `space-evenly` -- equal space between all items and edges
- `align-items` -- aligns items in the cross axis
  -`stretch` --  items fill cross section(default)
  -`flex-start | flex-end | center` -- (*Same as in justify-content*)
  -`baseline` -- text baselines aligned
- `align-content` -- align-content is for controlling how rows are packed/more like the space between the rows(cross axis,rows only)
  - `stretch` -- rows streatch to fill space
  - `flex-start` -- rows packed at start
  - `center | flex-end | space-between | space-around | space-evenly` -- (*Same as others*)
- `flex-wrap` -- controls whether items are allowed to go to a new line.
  - `nowrap` -- all items stay on one line and items shrink to fit the container
  - `wrap` -- items stay normal size, and when space runs out they move to next line
  - `wrap-reverse` -- same as wrap but instead rows appear above instead of below

## Grid
- `display-grid` -- turns an element into a grid
- `grid-template-columns` -- defines column structure
  - repeat(3,1fr) -- 3 equal columns (1fr is one fraction of available space)
- `grid-template-rows` --defines row structure
  - *Same value as col*
- `grid-column` -- used to set horizontal placement of the child.(Used on child)
  -ex: `1/3` -- start at line 1 and end at line 3
  -`2/ span 2` -- start at line 2 and span 2 columns
- `grid-row` -- controls vertical placement
  -ex:`1/2
  -`span 2` -- span 2 rows
- `align-items | justify-items` -- Same as flex box but they control the items inside a cell.
- `place-items` -- shorthand for `align-items + justify-items`.
  -`start|center|end|streatch`
- `gap` -- gap between rows and columns
  - `20px` -- both rows and columns
  - `20px 10px` -- row-gap & col-gap
