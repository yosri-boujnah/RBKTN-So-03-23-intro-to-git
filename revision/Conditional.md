# Introduction to JavaScript: Conditional

## If-Else statements

What if we want our program to make a decision about which function it should run? This is when we use conditions! If you have a TV you can watch it in the evening. If not, you might do something else.
It's the same with code. You can give an 'if' condition to a machine to make a decision about what part of the code to run.

Structure:

    if (condition) {
        do this
    } else {
        do something else
    }
We need condition to either be true or false, so if we have something like a number we need to compare it to something.

Example:

    var number = 7;
    if (number >= 7) {
        console.log('Our number is bigger than or equal to 7');
    } else {
        console.log('Our number is smaller than 7');
    }
## Comparison Operators

Earlier we introduced JavaScript's arithmetic operators. Now comes time to introduce you to the next set of operators. 'Comparison operators' are used to compare values (>, <, <=, >=, ===, !==). Most of them you know from math classes in school, some of them can be new for you:

-    '===' checks equality, results in true if two values are equal.
-    '!==' checks inequality, results in true if two values are not equal.

TIP: Don't mix up '=' and '===' as they have different meanings.

-    '=' means Assign
-    '===' means Is it equal

There are also '==' and '!=' operators, which are very similar to '===' and '!==', but with a slightly different meaning that is more prone to programming errors, so you should always use '===' and '!=='.

The result of a comparison operator is a boolean value (true or false).

For example:

    3 < 4 is true.
    1 + 1 === 3 is false.

## If - Else if - Else
Hmm, but what if we have 4 arithmetical operations in our calculator? Well,

we can use an if - else if - else structure.

Example:

    var number = 7;
    if (number > 7) {
        console.log('Our number is bigger then 7');
    } else if (number < 7) {
        console.log('Our number is smaller then 7');
    } else {
        console.log('Our number is equal to 7');
    }
## Boolean Operators

Putting an exclamation (!) before a Boolean variable gives the opposite value. The ! is called a "not" operator when used this way.

The result of a comparison is a Boolean value, we can save it to a variable

    var bool = (1 < 2);

Then we can check if 'bool' is true or false by using console.log

    console.log(bool); // This will return true
    console.log(!bool); // "not true", therefore returns false
    console.log(bool); // The original value isn't affected, still returns true

We can also assign a Boolean value straight to a variable with the keywords true and false:

    var aLie = false;
    var previousStatement = true;