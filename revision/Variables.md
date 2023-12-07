# Introduction to JavaScript: Variables


A variable is a place to store information. To create (also called declare)
a variable use the keyword 'var', as follows:


    var variableName;

So, we created a variable named variableName, but it has no information or value inside. It is 
.


If we print the variable to the console we can see that.


    console.log("variableName is " + variableName);
    The result will be "variableName is undefined".

To give our variable a value (assign a value) use the '=' sign:


    variableName = 'Hello world!';
As you can notice, we can give different types of values to our variables - Strings, Numbers, Booleans etc.

-   Strings - a set of characters, word(s), or phrases that we wrap in quotes, like 'hello world!'. This can be anything, including numbers.
-   Numbers - either integer or floating point (decimal). Not wrapped in quotes.
-   Boolean - it represents logical values - true or false.


P.S. You may see code that uses the keyword 'let' instead of 'var'.
This is a newer keyword that also creates variables, but with different rules about where that variable is available ("scope"). For now, consider 'let' and 'var' as essentially equivalent.


You can use the name of your variables to represent what information that they have inside.


Example:


    var hello = 'Hello World';
    alert(hello);
    
This will pop-up an alert box with the string 'Hello World!'
 