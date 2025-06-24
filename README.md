# toad-grid-flex
Introduction to css grid and flex

## Modern Layout Systems (Recommended)
These are the go-to methods for robust and flexible layout management in modern web development.

- #  Flexbox (Flexible Box Layout Module)
Flexbox is a one-dimensional layout system, meaning it can arrange items in a single row or a single column. It's incredibly powerful for distributing space among items in a container.

#### Concepts:

Flex Container: The parent element on which display: flex; is applied.
Flex Items: The direct children of the flex container.
Main Axis: The primary axis along which flex items are laid out (either horizontal or vertical).
Cross Axis: The axis perpendicular to the main axis.
1. Container Properties:

 - display: flex;: Initializes a flex container.
 - flex-direction: Sets the direction of the main axis (row - default, row-reverse, column, column-reverse).
 - justify-content: Aligns flex items along the main axis (flex-start, flex-end, center, space-between, space-around, space-evenly).
 - align-items: Aligns flex items along the cross axis (stretch - default, flex-start, flex-end, center, baseline).
 - flex-wrap: Controls whether flex items wrap onto multiple lines (nowrap - default, wrap, wrap-reverse).
 - align-content: When flex items wrap, aligns the lines of content along the cross axis (similar to justify-content but for lines).

2. Item Properties:

 - flex-grow: Defines the ability of a flex item to grow if necessary.
 - flex-shrink: Defines the ability of a flex item to shrink if necessary.
 - flex-basis: Defines the default size of an element before remaining space is distributed.
 - flex: Shorthand for flex-grow, flex-shrink, and flex-basis.
 - order: Controls the visual order of flex items (default is 0).
 - align-self: Overrides the align-items value for a specific flex item.
Use Cases: Navigation bars, evenly spaced items, centering content, responsive components.

- #  CSS Grid Layout
CSS Grid is a two-dimensional layout system, allowing you to arrange items in rows and columns simultaneously. It's ideal for overall page layouts and complex component structures.

#### Concepts:

Grid Container: The parent element on which display: grid; or display: inline-grid; is applied.
Grid Items: The direct children of the grid container.
Grid Lines: The horizontal and vertical lines that define the grid structure.
Grid Tracks: The spaces between grid lines (rows and columns).
Grid Cells: The smallest unit of the grid, defined by the intersection of a row and column track.
Grid Areas: Named areas within the grid that can span multiple cells.

1. Container Properties:

display: grid;: Initializes a grid container.
grid-template-columns, grid-template-rows: Define the number and size of columns and rows using various units (e.g., px, em, rem, %, fr - fractional unit).
repeat(), minmax(), auto-fit, auto-fill are powerful functions for flexible grid track sizing.
grid-template-areas: Allows you to name areas of your grid and place items into those named areas, creating highly readable layout definitions.
gap (or grid-gap - deprecated): Sets the spacing between grid cells (both row and column gaps).
justify-items, align-items: Aligns content within grid cells along the row and column axes, respectively.
justify-content, align-content: Aligns the grid itself within the grid container if there's extra space.

2. Item Properties:

grid-column-start, grid-column-end, grid-row-start, grid-row-end: Specify which grid lines an item spans.
grid-column, grid-row: Shorthand for the start/end properties.
grid-area: Assigns an item to a named grid area or defines its starting/ending lines.
place-self: Shorthand for justify-self and align-self.
Use Cases: Entire page layouts (header, nav, main, sidebar, footer), complex component arrangements, gallery layouts.