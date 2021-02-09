# Control Flow

## Loops

-Loops are type of control flow in JavaScript and are useful for running the same code over and over again.

-JavaScript supports different kinds of loops:

    for - loops through a block of code a number of times.
    for/in - loops through the properties of an object.
    for/of - loops through the values of an iterable object.
    while - loops through a block of code while a specified condition is true.
    do/while - also loops through a block of code while a specified condition is true.

## For Loops

-The for loop has the following syntax:

for (statement 1; statement 2; statement 3) {
  // code block to be executed
}

Statement 1 is executed (one time) before the execution of the code block.
Statement 2 defines the condition for executing the code block.
Statement 3 is executed (every time) after the code block has been executed.

## While Loops

-The while loop loops through a block of code as long as a specified condition is true.

Syntax
while (condition) {
  // code block to be executed
}

***If you forget to increase the variable used in the condition, the loop will never end. This will crash your browser.***

## Do/While Loops

-The do/while loop is a variant of the while loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.

Syntax
do {
  // code block to be executed
}
while (condition);

## Conditional Statements

-In JavaScript we have the following conditional statements:

    Use if to specify a block of code to be executed, if a specified condition is true.
    Use else to specify a block of code to be executed, if the same condition is false.
    Use else if to specify a new condition to test, if the first condition is false.
    Use switch to specify many alternative blocks of code to be executed.

## If Statements

-Use the if statement to specify a block of JavaScript code to be executed if a condition is true.

Syntax
if (condition) {
  //  block of code to be executed if the condition is true
}

***Note that if is in lowercase letters. Uppercase letters (If or IF) will generate a JavaScript error.***

## Else Statements

-Use the else statement to specify a block of code to be executed if the condition is false.

if (condition) {
  //  block of code to be executed if the condition is true
} else {
  //  block of code to be executed if the condition is false
}

## Else/If Statements

-Use the else if statement to specify a new condition if the first condition is false.

Syntax
if (condition1) {
  //  block of code to be executed if condition1 is true
} else if (condition2) {
  //  block of code to be executed if the condition1 is false and condition2 is true
} else {
  //  block of code to be executed if the condition1 is false and condition2 is false
}

## Logical Operators

-&& = and

-|| = or

## Logical Not

-The logical NOT (!) operator (logical complement, negation) takes truth to falsity and vice versa. It is typically used with Boolean (logical) values. When used with non-Boolean values, it returns false if its single operand can be converted to true; otherwise, returns true.

## Switch Statements

-The switch statement is used to perform different actions based on different conditions.

-Use the switch statement to select one of many code blocks to be executed.

Syntax
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}

-This is how it works:

    The switch expression is evaluated once.
    The value of the expression is compared with the values of each case.
    If there is a match, the associated block of code is executed.
    If there is no match, the default code block is executed.