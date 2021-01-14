# JavaScript

JavaScript is a high level programming language that all modern web browsers support. Like HTML and CSS, it is a core technology.

-'//' allows you to leave comments at the end of your code. '//' tells JavaScript to ignore the remainder of the text on the current line. '/* comment here */' allows you to make a multi-line comment.

-JavaScript provides eight different data types: undefined, null, boolean, string, symbol, bigint, number and object.

-Variables allow computers to store and manipulate data in a dynamic fashion. They do this using a label to point to data rather than using the data itself. Any of the eight data types above ^^ can be stored in a variable. You can tell JavaScript to create or declare a variable by putting the keyword 'var' in front of it. Variables can be made up of number. letter and $ or _, but no spaces or cannot start with a number.

-In JavaScript you can assign a value to a variable with '=' (the assignment operator). For Example:
var myName;
myName = 3;

-Once a value is assigned to a variable, you can assign the value of that variable to a different variable. For example:
var myVar;
myVar = 5;
var myNum;
myNum = myVar;

-You can also initialize a variable to an initial value on the same line. For example:
var myName = 9
-When JavaScript variables are declared, they have an initial value of 'undefined'.

-In JavaScript all variables and function names are case sensitive.

-'Number' is a data type in JavaScript which represents numeric data. '+' and '-' symbols are used for addition and subtraction. '*' to multiply. '/' for division. You can increment or add one to a variable with '++' and decrement or decrease a variable with '--'.

-Decimal numbers can also be used as variables too.

-'%' (the remainder operator) gives the remainder of the division of two numbers.

-'+=' assigns a number to a variable and performs a mathematical operation at the same time.

- '-=' performs the same function but subtracts a number from a variable.

-'*=' multiplies and '/=' divides.

-A series of zeros or characters in quotation marks("") are called a 'string'. A string must start and end with " or '. In JavaScript, you can escape a quote from considering it as an end of string quote by placing a backslash (\) in front of the quote.

Code	Output
\'	single quote
\"	double quote
\\	backslash
\n	newline
\r	carriage return
\t	tab
\b	word boundary
\f	form feed

-In JavaScript you can concatenate (or link) strings together using '+'

-'+=' operator will concatenate a string a string onto the end of an existing string.

-You can find the length of a String value by writing .length after the string variable or string literal.

-Bracket notation is a way to get a character at a specific index within a string. For example index 4 of the word Jack would the character K. (note most modern programming languages start counting from 0).

-In JavaScript, String values are immutable, which means that they cannot be altered once created.

-In order to get the last letter of a string, you can subtract one from the string's length. For example [.length - 1]. This principle can be be used the second to last[.length - 2], third to last [.length - 3] and so on.

-Array variables allow you to store multiple pieces of data in one place. Array variables start and end with '[  ]'. (**You can also have an array within an array. '[ [  ], [  ] ]').

-Array data can data can be accessed using indexes ([ ]). 

-Unlike strings, arrays can be changed freely.

-The push function '.push()' allows you to append data to the end of an array. It takes one or more parameters and pushes them on to the end of an array.

-'.unshift()' performs the same function except it adds elements to the front the array rather than the end. 

-'.pop()' is used to remove a value from the end of an array. We can store the "popped off" value by assigning it to a variable.

-'.shift()' performs the same function. However rather than removing the last element of an array it removes the first.

-In JavaScript, we can divide up our code into reusable parts called functions. You can call or invoke this function by using its name followed by parentheses. All of the code between the curly braces will be executed every time the function is called.