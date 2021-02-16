# Objects

-JavaScript variables are containers for data values. For example his code assigns a simple value (Fiat) to a variable named car:
        var car = "Fiat";

-Objects are variables too. But objects can contain many values. For example this code assigns many values (Fiat, 500, white) to a variable named car:
        var car = {
            type:"Fiat", 
            model:"500", 
            color:"white"
        };

-The values are written as name:value pairs (name and value separated by a colon).

-JavaScript objects are containers for named values called properties or methods.

## Object Literals

-You define (and create) a JavaScript object with an object literal:

-Spaces and line breaks are not important. An object definition can span multiple lines:

-Example
        var person = {
            firstName: "John",
            lastName: "Doe",
            age: 50,
            eyeColor: "blue"
        };

-You can access object properties in two ways:

        objectName.propertyName

                or

        objectName["propertyName"]

## Object Methods

-Objects can also have methods.

-Methods are actions that can be performed on objects.

-Methods are stored in properties as function definitions.

-A method is a function stored as a property.

-Example

        var person = {
            firstName: "John",
            lastName : "Doe",
            id       : 5566,
            fullName : function() {
                return this.firstName + " " + this.lastName;
            }
        };

## This Keyword

-Example

        var person = {
            firstName: "John",
            lastName : "Doe",
            id       : 5566,
            fullName : function() {
            return this.firstName + " " + this.lastName;
           }
        };

-The JavaScript this keyword refers to the object it belongs to.

-It has different values depending on where it is used:
    .In a method, this refers to the owner object.
    .Alone, this refers to the global object.
    .In a function, this refers to the global object.
    .In a function, in strict mode, this is undefined.
    .In an event, this refers to the element that received the event.
    .Methods like call(), and apply() can refer this to any object.

## Math Objects

-The JavaScript Math object allows you to perform mathematical tasks on numbers.

-Math.round() returns the value of x rounded to its nearest integer. For example:
        Math.round(4.7);    // returns 5
        Math.round(4.4);    // returns 4

-Math.pow(x, y) returns the value of x to the power of y. For example:
        Math.pow(8, 2);      // returns 64

-Math.sqrt() returns the square root of x. For example:
        Math.sqrt(64);      // returns 8

-Math.abs() returns the absolute (positive) value of x. For example:
        Math.abs(-4.7);     // returns 4.7

-Math.ceil() returns the value of x rounded up to its nearest integer. For example:
        Math.ceil(4.4);     // returns 5

-Math.floor() returns the value of x rounded down to its nearest integer. For example:
        Math.floor(4.7);    // returns 4

-Math.sin() returns the sine (a value between -1 and 1) of the angle x (given in radians). If you want to use degrees instead of radians, you have to convert degrees to radians: Angle in radians = Angle in degrees x PI / 180. For example:
        Math.sin(90 * Math.PI / 180);     // returns 1 (the sine of 90 degrees)

-Math.cos() returns the cosine (a value between -1 and 1) of the angle x (given in radians). If you want to use degrees instead of radians, you have to convert degrees to radians: Angle in radians = Angle in degrees x PI / 180. For example:
        Math.cos(0 * Math.PI / 180);     // returns 1 (the cos of 0 degrees)

-Math.min() and Math.max() can be used to find the lowest or highest value in a list of arguments. For example:
        Math.min(0, 150, 30, 20, -8, -200);  // returns -200
        Math.max(0, 150, 30, 20, -8, -200);  // returns 150

-Math.random() returns a random number between 0 (inclusive), and 1 (exclusive) for example:
    Math.random();     // returns a random number

## Math Properties (Constants)

-JavaScript provides 8 mathematical constants that can be accessed with the Math object:

Example
Math.E        // returns Euler's number
Math.PI       // returns PI
Math.SQRT2    // returns the square root of 2
Math.SQRT1_2  // returns the square root of 1/2
Math.LN2      // returns the natural logarithm of 2
Math.LN10     // returns the natural logarithm of 10
Math.LOG2E    // returns base 2 logarithm of E
Math.LOG10E   // returns base 10 logarithm of E

## Primitive & Reference Types

-In JavaScript, a variable may store two types of values: primitive and reference.

-JavaScript provides six primitive types as undefined, null, boolean, number, string, and symbol , and a reference type object.

-The size of a primitive value is fixed, therefore, JavaScript stores the primitive value on the stack.

-On the other hand, the size of a reference value is dynamic so JavaScript stores the reference value on the heap.

-When you assign a value to a variable, the JavaScript engine will determine whether the value is a primitive or reference value.

-If the value is a primitive value, when you access the variable, you manipulate the actual value stored in that variable. In other words, the variable that stores a primitive value is accessed by value.

-Unlike a primitive value, when you manipulate an object, you work on the reference of that object, rather than the actual object. It means a variable that stores an object is accessed by reference.

-To determine the type of a primitive value you use the typeof operator.