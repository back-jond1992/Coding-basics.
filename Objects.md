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