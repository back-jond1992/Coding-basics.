## Test Method

-Regular expressions are used in programming languages to match parts of strings. You create patterns to help you do that matching.

-If you want to find the word "the" in the string "The dog chased the cat", you could use the following regular expression: /the/. Notice that quote marks are not required within the regular expression.

-JavaScript has multiple ways to use regexes. One way to test a regex is using the .test() method. The .test() method takes the regex, applies it to a string (which is placed inside the parentheses), and returns true or false if your pattern finds something or not.

    let testStr = "freeCodeCamp";
    let testRegex = /Code/;
    testRegex.test(testStr);
    // Returns true

-That regex searched for a literal match of the string "Hello". Here's another example searching for a literal match of the string "Kevin":

    let testStr = "Hello, my name is Kevin.";
    let testRegex = /Kevin/;
    testRegex.test(testStr);
    // Returns true

-Any other forms of "Kevin" will not match. For example, the regex /Kevin/ will not match "kevin" or "KEVIN".

    let wrongRegex = /kevin/;
    wrongRegex.test(testStr);
    // Returns false

-You can search for multiple patterns using the alternation or OR operator: |.

-This operator matches patterns either before or after it. For example, if you wanted to match "yes" or "no", the regex you want is /yes|no/.

-You can also search for more than just two patterns. You can do this by adding more patterns with more OR operators separating them, like /yes|no|maybe/.

## Match with Case Differences

-You can match both cases using what is called a flag. There are other flags but here you'll focus on the flag that ignores case - the i flag. You can use it by appending it to the regex. An example of using this flag is /ignorecase/i. This regex can match the strings "ignorecase", "igNoreCase", and "IgnoreCase".

## Extract Matches

-You can also extract the actual matches you found with the .match() method.

-To use the .match() method, apply the method on a string and pass in the regex inside the parentheses.

-Here's an example:

    "Hello, World!".match(/Hello/);
    // Returns ["Hello"]
    let ourStr = "Regular expressions";
    let ourRegex = /expressions/;
    ourStr.match(ourRegex);
    // Returns ["expressions"]

***Note that the .match syntax is the "opposite" of the .test method you have been using thus far:

    'string'.match(/regex/);
    /regex/.test('string');

-So far, you have only been able to extract or search a pattern once.

    let testStr = "Repeat, Repeat, Repeat";
    let ourRegex = /Repeat/;
    testStr.match(ourRegex);
    // Returns ["Repeat"]

-To search or extract a pattern more than once, you can use the g flag.

    let repeatRegex = /Repeat/g;
    testStr.match(repeatRegex);
    // Returns ["Repeat", "Repeat", "Repeat"]

## Wildcard Period

-Sometimes you won't (or don't need to) know the exact characters in your patterns. Thinking of all words that match, say, a misspelling would take a long time. Luckily, you can save time using the wildcard character: .

-The wildcard character . will match any one character. The wildcard is also called dot and period. You can use the wildcard character just like any other character in the regex. For example, if you wanted to match "hug", "huh", "hut", and "hum", you can use the regex /hu./ to match all four words.

    let humStr = "I'll hum a song";
    let hugStr = "Bear hug";
    let huRegex = /hu./;
    huRegex.test(humStr); // Returns true
    huRegex.test(hugStr); // Returns true

## Match Single Characters with Multiple Possibilities

-You can search for a literal pattern with some flexibility with character classes. Character classes allow you to define a group of characters you wish to match by placing them inside square ([ and ]) brackets.

-For example, you want to match "bag", "big", and "bug" but not "bog". You can create the regex /b[aiu]g/ to do this. The [aiu] is the character class that will only match the characters "a", "i", or "u".

    let bigStr = "big";
    let bagStr = "bag";
    let bugStr = "bug";
    let bogStr = "bog";
    let bgRegex = /b[aiu]g/;
    bigStr.match(bgRegex); // Returns ["big"]
    bagStr.match(bgRegex); // Returns ["bag"]
    bugStr.match(bgRegex); // Returns ["bug"]
    bogStr.match(bgRegex); // Returns null