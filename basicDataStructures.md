# Basic Data Structures

## Bracket Notation

-When we define a simple array as seen below, there are 3 items in it:

    let ourArray = ["a", "b", "c"];

-In an array, each array item has an index. This index doubles as the position of that item in the array, and how you reference it. However, it is important to note, that JavaScript arrays are zero-indexed, meaning that the first element of an array is actually at the zeroth position, not the first. In order to retrieve an element from an array we can enclose an index in brackets and append it to the end of an array, or more commonly, to a variable which references an array object. This is known as bracket notation. For example, if we want to retrieve the a from ourArray and assign it to a variable, we can do so with the following code:

    let ourVariable = ourArray[0];
    Now ourVariable has the value of a.

-In addition to accessing the value associated with an index, you can also set an index to a value using the same notation:

    ourArray[1] = "not b anymore";

-Using bracket notation, we have now reset the item at index 1 from the string b, to not b anymore. Now ourArray is ["a", "not b anymore", "c"].

## push() and unshift()

-Both methods take one or more elements as parameters and add those elements to the array the method is being called on; the push() method adds elements to the end of an array, and unshift() adds elements to the beginning. Consider the following:

    let twentyThree = 'XXIII';
    let romanNumerals = ['XXI', 'XXII'];

    romanNumerals.unshift('XIX', 'XX');

-romanNumerals would have the value ['XIX', 'XX', 'XXI', 'XXII'].

    romanNumerals.push(twentyThree);

-romanNumerals would have the value ['XIX', 'XX', 'XXI', 'XXII', 'XXIII']. ***Notice that we can also pass variables, which allows us even greater flexibility in dynamically modifying our array's data.***

## pop() and shift()

-pop() removes an element from the end of an array, while shift() removes an element from the beginning. The key difference between pop() and shift() and their cousins push() and unshift(), is that neither method takes parameters, and each only allows an array to be modified by a single element at a time.

    let greetings = ['whats up?', 'hello', 'see ya!'];

    greetings.pop();

-greetings would have the value ['whats up?', 'hello'].

    greetings.shift();
    greetings would have the value ['hello'].

-We can also return the value of the removed element with either method like this:

    let popped = greetings.pop();

-greetings would have the value [], and popped would have the value hello.

## splice()

-What if we want to remove an element from somewhere in the middle? Or remove more than one element at once? Well, that's where splice() comes in. splice() allows us to do just that: remove any number of consecutive elements from anywhere in an array.

-splice() can take up to 3 parameters, but for now, we'll focus on just the first 2. The first two parameters of splice() are integers which represent indexes, or positions, of the array that splice() is being called upon. And remember, arrays are zero-indexed, so to indicate the first element of an array, we would use 0. splice()'s first parameter represents the index on the array from which to begin removing elements, while the second parameter indicates the number of elements to delete. For example:

    let array = ['today', 'was', 'not', 'so', 'great'];

    array.splice(2, 2);

H-ere we remove 2 elements, beginning with the third element (at index 2). array would have the value ['today', 'was', 'great'].

-splice() not only modifies the array it's being called on, but it also returns a new array containing the value of the removed elements:

    let array = ['I', 'am', 'feeling', 'really', 'happy'];

    let newArray = array.splice(3, 2);

-newArray has the value ['really', 'happy'].

-splice() can take up to three parameters? Well, you can use the third parameter, comprised of one or more element(s), to add to the array. This can be incredibly useful for quickly switching out an element, or a set of elements, for another.

    const numbers = [10, 11, 12, 12, 15];
    const startIndex = 3;
    const amountToDelete = 1;

    numbers.splice(startIndex, amountToDelete, 13, 14);
    console.log(numbers);

-The second entry of 12 is removed, and we add 13 and 14 at the same index. The numbers array would now be [ 10, 11, 12, 13, 14, 15 ].

-Here, we begin with an array of numbers. Then, we pass the following to splice(): The index at which to begin deleting elements (3), the number of elements to be deleted (1), and the remaining arguments (13, 14) will be inserted starting at that same index. Note that there can be any number of elements (separated by commas) following amountToDelete, each of which gets inserted.
