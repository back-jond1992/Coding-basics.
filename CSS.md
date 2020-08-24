## CSS

Text color is changed by changing the 'style' of elements. The property responsible for colour is the 'color' style property. For example <h1 style="color: pink;">Korean Cooking Recipes,/h1>.

(good practice to end inline style declarations with ';')

            or

Instead of styling the individual elements with inline CC, a style block can be created at the top of the code. To create a style block 'style' tags are used and inside the style block a CSS selector for the different elements can be made.

(curly braces must be used around each elements style rules.)

Classes are style which can be reused and added to HTML elements. In the CSS style element class names start with a period. The HTML element must have a class applied, for example <h1 class="red-text">Korean Cooking Recipes</h1>

Font size is controlled by 'font-size' CSS property.

Font is controlled by 'font-family' CSS property.

Element width is controlled by the 'width' CSS property.

CSS borders have 'style', 'color' and 'width' properties. CSS borders can also be rounded with the CCS property 'border-radius' (border-radius can be specified in pixels or %).

Elements background colour is set with the CCS 'background-color' property.

In addition to classes elements can be given 'id' attributes. ('id' attributes are not reusable and should only be applied tp one element).

** note ** classes are referenced with a '.' and id's with a '#'.

CSS properties 'padding', 'margin' and 'border' control the spaces around HTML elements:
    -'padding' controls the amount of space between an elements content and its 'border'. With the 'padding' element all four sides of an element can be controlled (padding-top/right/left/bottom). These can be specified individually or all as one line.
    -'margin' controls the amount of space between an elements 'border' and surrounding elements. Negative value makes the element grow larger. Same as the 'padding' element the 'margin' element controls all four sides of an element (margin-top/right/left/bottom). These can be specified individually or all as one line.

'!important' CSS attribute is used to override all CCS declarations.
