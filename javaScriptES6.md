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