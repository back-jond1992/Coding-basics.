# Functions

-A JavaScript function is a block of code designed to perform a particular task.

-A JavaScript function is executed when "something" invokes it (calls it).

-You can reuse code: Define the code once, and use it many times.    

-You can use the same code many times with different arguments, to produce different results.

## JavaScript Function Syntax

-A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

-Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

-The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)

T-he code to be executed, by the function, is placed inside curly brackets: {}

    function name(parameter1, parameter2, parameter3) {
        // code to be executed
    }

-Function parameters are listed inside the parentheses () in the function definition.

-Function arguments are the values received by the function when it is invoked.

-Inside the function, the arguments (the parameters) behave as local variables.

## Function Declartions

-A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

    .The name of the function.
    .A list of parameters to the function, enclosed in parentheses and separated by commas.
    .The JavaScript statements that define the function, enclosed in curly brackets, {...}.

-For example, the following code defines a simple function named square:

    function square(number) {
        return number * number;
    }

## Function Expressions

-A JavaScript function can also be defined using an expression.

-A function expression can be stored in a variable:

    var x = function (a, b) {
        return a * b
    };

-After a function expression has been stored in a variable, the variable can be used as a function. Functions stored in variables do not need function names. They are always invoked (called) using the variable name.

## Function Return

-When JavaScript reaches a return statement, the function will stop executing.

-If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

-Functions often compute a return value. The return value is "returned" back to the "caller":

Example
Calculate the product of two numbers, and return the result:

    var x = myFunction(4, 3);   // Function is called, return value will end up in x

    function myFunction(a, b) { 
        return a * b;             // Function returns the product of a and b
    }

## Arrow Function

-Arrow functions were introduced in ES6.

-Arrow functions allow us to write shorter function syntax:

-Before:
        hello = function() {
            return "Hello World!";
        }

-With Arrow Function:

        hello = () => {
            return "Hello World!";
        }

