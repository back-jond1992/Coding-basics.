## Object Mutation

-To ensure your data doesn't change, JavaScript provides a function Object.freeze to prevent data mutation.

-Once the object is frozen, you can no longer add, update, or delete properties from it. Any attempt at changing the object will be rejected without an error.

Example: 

    let obj = {
        name:"FreeCodeCamp",
        review:"Awesome"
    };
    Object.freeze(obj);
    obj.review = "bad"; // will be ignored. Mutation not allowed
    obj.newProp = "Test"; // will be ignored. Mutation not allowed
    console.log(obj); 
    // { name: "FreeCodeCamp", review:"Awesome"}

## Arrow Functions

-In JavaScript, we often don't need to name our functions, especially when passing a function as an argument to another function. Instead, we create inline functions. We don't need to name these functions because we do not reuse them anywhere else.

-To achieve this, we often use the following syntax:

    const myFunc = function() {
        const myVar = "value";
        return myVar;
    }

-ES6 provides us with the syntactic sugar to not have to write anonymous functions this way. Instead, you can use arrow function syntax:

    const myFunc = () => {
        const myVar = "value";
        return myVar;
    }

-When there is no function body, and only a return value, arrow function syntax allows you to omit the keyword return as well as the brackets surrounding the code. This helps simplify smaller functions into one-line statements:

    const myFunc = () => "value";

This code will still return the string value by default.

-Just like a regular function, you can pass arguments into an arrow function.

    // doubles input value and returns it
    const doubler = (item) => item * 2;
    doubler(4); // returns 8

-If an arrow function has a single parameter, the parentheses enclosing the parameter may be omitted.

    // the same function, without the parameter parentheses
    const doubler = item => item * 2;

-It is possible to pass more than one argument into an arrow function.

    // multiplies the first input value by the second and returns it
    const multiplier = (item, multi) => item * multi;
    multiplier(4, 2); // returns 8

## Default Parameters for Functions

-In order to help us create more flexible functions, ES6 introduces default parameters for functions:

    const greeting = (name = "Anonymous") => "Hello " + name;

    console.log(greeting("John")); // Hello John
    console.log(greeting()); // Hello Anonymous

-The default parameter kicks in when the argument is not specified (it is undefined). As you can see in the example above, the parameter name will receive its default value "Anonymous" when you do not provide a value for the parameter. You can add default values for as many parameters as you want.

## Rest Parameter

-In order to help us create more flexible functions, ES6 introduces the rest parameter for function parameters. With the rest parameter, you can create functions that take a variable number of arguments. These arguments are stored in an array that can be accessed later from inside the function.

    function howMany(...args) {
        return "You have passed " + args.length + " arguments.";        
    }
    console.log(howMany(0, 1, 2)); // You have passed 3 arguments.
    console.log(howMany("string", null, [1, 2, 3], { })); // You have passed 4 arguments.

-The rest parameter eliminates the need to check the args array and allows us to apply map(), filter() and reduce() on the parameters array.

## Spread Operator

-ES6 introduces the spread operator, which allows us to expand arrays and other expressions in places where multiple parameters or elements are expected.

-The ES5 code below uses apply() to compute the maximum value in an array:

    var arr = [6, 89, 3, 45];
    var maximus = Math.max.apply(null, arr); // returns 89

-We had to use Math.max.apply(null, arr) because Math.max(arr) returns NaN. Math.max() expects comma-separated arguments, but not an array. The spread operator makes this syntax much better to read and maintain:

    const arr = [6, 89, 3, 45];
    const maximus = Math.max(...arr); // returns 89

-...arr returns an unpacked array. In other words, it spreads the array. However, the spread operator only works in-place, like in an argument to a function or in an array literal. The following code will not work:

    const spreaded = ...arr; // will throw a syntax error

## Destructing Assignment

-Destructuring assignment is special syntax introduced in ES6, for neatly assigning values taken directly from an object.

-Consider the following ES5 code:

    const user = { name: 'John Doe', age: 34 };

    const name = user.name; // name = 'John Doe'
    const age = user.age; // age = 34

-Here's an equivalent assignment statement using the ES6 destructuring syntax:

    const { name, age } = user;
    // name = 'John Doe', age = 34

-Here, the name and age variables will be created and assigned the values of their respective values from the user object. You can see how much cleaner this is.

-Destructuring allows you to assign a new variable name when extracting values. You can do this by putting the new name after a colon when assigning the value.

-Using the same object from the last example:

    const user = { name: 'John Doe', age: 34 };

-Here's how you can give new variable names in the assignment:

    const { name: userName, age: userAge } = user;
    // userName = 'John Doe', userAge = 34

-You may read it as "get the value of user.name and assign it to a new variable named userName" and so on.

-You can use the same principles from the previous two lessons to destructure values from nested objects.

-Using an object similar to previous examples:

    const user = {
        johnDoe: { 
            age: 34,
            email: 'johnDoe@freeCodeCamp.com'
        }
    };

-Here's how to extract the values of object properties and assign them to variables with the same name:

    const { johnDoe: { age, email }} = user;

-And here's how you can assign an object properties' values to variables with different names:

    const { johnDoe: { age: userAge, email: userEmail }} = user;