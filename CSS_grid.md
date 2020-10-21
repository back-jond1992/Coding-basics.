# CSS Grid

CSS grid allows you to turn HTML elements into grid containers with rows and columns to place children elements within.

-Change the 'display' element to grid. This allows all the CSS grid properties to be applied.

-'grid-template-columns' element adds columns to the grid. Values need to be given for the width of each column and the numbers values determines the number of columns.

-'grid-template-rows' element adds rows to the grid. Values need to be given for the width of each rows and the numbers values determines the number of rows.

-** CSS values can be set px, em, fr (a fraction of the available space), auto and %.**

-'grid-column-gap' adds a gap between columns.

-'grid-row-gap' adds a gap between rows.

-'grid-gap' can also be used to add a gap. If there is only one value a gap will be created between all rows and columns. If there are 2 values the first value is for rows and the second for columns.

-'grid-column' controls the amount of columns an item will consume.

-'grid-row' controls the amount of rows an item will consume.

-'justify-self' aligns content within the cell (**in the CCS grid the content of each item is located in a cell):
    .'start' aligns content to the left.
    .'center' aligns content to the center.
    .'end' aligns content to the right.

-'align-self' is the same as 'justify-self' but aligns content vertically rather than horizontally. This property accepts the same values as above:
    .'start' aligns content to the top.
    .'center' aligns content to the center.
    .'end' aligns content to the bottom.

-'justify-items' aligns all the items in the CSS grid (horizontally) at one once, rather than aligning the items individually with the above properties.

-'align-items' is the same as 'justify-items' however its aligns the items vertically.

-cells can be grouped into areas and given custom names. 'grid-template-areas' can do this. **Every word/name in the values represents a cell and every pair of quotations a row. To add items to the area you reference the name you gave it using 'grid-area'.]

-'grid-area' can also be used to create an area using the line numbers to define where the area will be.

'repeat(__)' function controls the number of times a column or a row is repeated.

'minmax' is used to limit the size of items when the container changes size. A suitable size range for the items needs to be specified.

'auto-fill' function allows as many rows or columns (of a specified size) as possible to be inserted automatically into a container.

'auto-fit' has the same function however if the container size exceeds the size of all the items combined 'auto-fill' will keep inserting empty rows or columns. Whereas 'auto-fit' will stretch the size of the items to fill the container.