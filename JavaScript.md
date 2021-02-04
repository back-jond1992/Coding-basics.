# JavaScript

-Small amounts of JavaScript can be added to a index.html file or can be 
added in a link tag (sandbox.js). File is linked using: <script scr="sandbox.js>
</script>.

-console.log logs JavaScript from our file to the console.

-'let' keyword creates a variable, same as 'var' keyword.

-'const' also creates a variable, however it cannot be changed, it is constant.
Any attempt to change the variable will result in an error message.

-'//' allow you to single line comment in JavaScript. '/* /*' allows you to mult-line
comment.

-7 data types: number (1, 2, 50, 3.79), string ('', ""), boolean (true/false), null
(explicitly set with no value), undefined (for variables with no value set yet), object
(complex data structures), symbol (used with objects).


## Strings

-Strings are series of letters, characters or numbers inside quotation marcs. '.__' (.
notions) get the properties of stings, for example: '.length' gets the length of a string.
They also have methods which are similar to functions. These are denoted and called
using parentheses '()'.


-'+' adds strings together.

-'[]' can get a single character from a string.

-The '.indexOf(). method returns the first index at which a given element can be found in the array, or -1 if it is not present.

-The 'slice(), method returns a shallow copy of a portion of an array into a new array object selected from start to end (end not included) where start and end represent the index of items in that array. The original array will not be modified.

-The 'substr()' method extracts parts of a string, beginning at the character at the specified position, and returns the specified number of characters.

-The 'replace()' method searches a string for a specified value, or a regular expression, and returns a new string where the specified values are replaced.


## Numbers

-Math operators: +, -. *, /, **, %.

-Order of operation = B (brackets), I (indexes), D (division), M (multiplication), A (addition), S (subtraction).

-'++' '--' adds 1 and minuses 1 respectively. '+=', '-+', '*=', '/=' takes the value and adds, minuses, times or divides by the specified number. (Shorthand notation).

-'Nan' = not a number.

## Templates Strings/String Literals

-Template literals are enclosed by the backtick (` `) character instead of double or single quotes.

-Template literals can contain placeholders. These are indicated by the dollar sign and curly braces (${expression}). The expressions in the placeholders and the text between the backticks (` `) get passed to a function.

## Arrays

- An array is a special variable, which can hold more than one value at a time.

-Arrays are created using '[ ]' square brackets.

-You access an array element by referring to the index number.

-Arrays have various methods, for example: '.join', '.pop', '.push'.

## Null/Undefined

-Undefined means a variable declared, but no value has been assigned a value.

-Whereas, null in JavaScript is an assignment value. You can assign it to a variable.

## Booleans

-A JavaScript Boolean represents one of two values: true or false.

-You can use the 'Boolean()' function to find out if an expression (or a variable) is true:

==	equal to
===	equal value and equal type
!=	not equal	
!==	not equal value or not equal type
> greater than
<	less than
>=	greater than or equal to	x >= 8	false	
<=	less than or equal to

- Everything with a value is true, everything without a value is false.

## Type Conversion

-Type Conversion is the conversion of object from one data type to another data type.

-The three most widely used type conversions are to string, to number, and to boolean:

    String Conversion – Occurs when we output something. Can be performed with 'String(value)'. The conversion to string is usually obvious for primitive values.

    Numeric Conversion – Occurs in math operations. Can be performed with 'Number(value)'.

    Boolean Conversion – Occurs in logical operations. Can be performed with 'Boolean(value)'.

-You can use the 'typeof' operator to find the data type of a JavaScript variable.