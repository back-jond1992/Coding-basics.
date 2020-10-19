# CSS Flexbox

Flexbox or flexboxes create page layouts for a dynamic UI (user interface). Arranges different elements in a predictable way for different screen sizes and browsers.

-CSS property 'display; flex;' on an element allows flex properties to be used to build a responsive page. 

-'flex-direction' allows you to allign elements into rows or columns.

-Sometimes not all the flex items within a flew container fill the container. 'justify-content' allows us to space out flex items and aligns flex items along the main axis:
    .'center' aligns the flex items in to the center.
    .'flew-start' aligns the flex items to the start of the container.
    .'flex-end' aligns the flex items to the end of the container.
    .'space-between' aligns the flex items to the center but with space      between the items.
    .'space-around' is the same as 'space-between' but with space all around the flex items so the first and last items do not touch the edges of the container.
    .'space-evenly' distributes space evenly between all the flex items.

-'align-items' property is similar to 'justify-content' but aligns flex items along the cross axis rather than the main axis:
    .'flex-start' aligns items to the start of the flex container.
    .'flex-end' aligns items to the end of the flex container. 
    .'center' align items to the center. For rows, this vertically aligns items (equal space above and below the items).
    .'stretch' stretch the items to fill the flex container. (This is the default value if no align-items value is specified.)
    .'baseline' align items to their baselines. Baseline is a text concept, think of it as the line that the letters sit on.


-'flex-wrap' tells CSS to wrap items and moves extra items into columns or rows. There are different options for wrap direction:
    .'nowrap' is the default and does not wrap items.
    .'wrap' wraps items from left to right in rows and top to bottom in columns.
    .'wrap-reverse' is the opposite of 'wrap'.

.'flex-shrink' is used to shrink an item in a flex container when the container is too small. The higher the value the more then item will shrink.

.'flex-grow' is the opposite of 'flex-shrink' and is used to gow an item in a flex container when the container is too large.

.'flex-basis' specifies the initial size of the item before CSS makes adjustments with 'flex-shrink/grow'.

'flex-grow/shrink/basis' (**in that order) can all be set at the same time using 'flex' property.

'order' property tells CSS the order items appear in the flex box. (By default items appear in the order they come in the source HTML.)

'align-self' allows each items alignment to be adjusted individually.