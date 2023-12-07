# Introduction to JavaScript: Functions


Functions are required to make our code ‘run’. Functions will take data, compute it, and return the computed data. All code that is ‘run’ in JavaScript is run inside of a function.


At the end of this article, you should be able to:


-   Understand JavaScript functions, why we use them, and be able to write correct function syntax.
-   Write and call functions using arguments and parameters.
-   Explain function scope and the return statement.


## Learn to understand JavaScript functions, why we use them, and be able to write correct function syntax.


### Introduction to Functions


Now that we have the basics of JavaScript down, data types, conditional statements, and variables, we need functions to compute them, change them, and do something with them. We can think of functions as small computer programs. Functions are required to get our code to ‘run’ in JavaScript. Although you may not realize it, you have been using functions this entire time. Functions allow us to write code that will be used over and over again, keeping our code `DRY`. As such, functions will often times take input and give output, although that is not always required. Functions also have their own ‘scope’, in which we can assign a variable within a function that is not available anywhere else.


### How to Write a Function


There are three ways we can build a function. For this article, we will be focusing on just one. For our purposes right now, all three ways will act the same.


    function myFunctionName() {
        // your instructions here
    }

### Anatomy of a Function


A function will start with the `function` keyword. This tells whatever is running your program that what follows is a function and to treat it as such. After that comes the name of the function. We like to give functions names that describe what they do. Then comes an open and a close parenthesis. And finally, open and close brackets. In between these brackets is where all of our function code will go.


    function logHello() {
        console.log('hello');
    }
    
    logHello();

In this example, we declare a function `logsHello` and set it up to `console.log`  `'hello'`. We can then see that in order to run this function, we need to write or invoke its name with the parentheses after it. This is the syntax to run a function. A function always needs parentheses to run.


## Learn to write and call functions using arguments and parameters.


Parameters and arguments allow us to pass data into functions and use this data within the function. In this objective, we will learn the difference between the two and how to use them.


### Passing Data into Functions


As mentioned before, a big reason we use functions is code re-use. We are always looking for ways to keep our code `DRY` (Don’t Repeat Yourself). Because of this, functions allow us to pass data into them for use inside the function. We can declare little function variables called `parameters` and pass that data in when we call the function (the data are then called `arguments`).


### Parameters


A function parameter will represent the data we pass into a function, for use in the function. Essentially when we write a function we assign the data variable names, even without knowing what the data will be. We set these `variables` inside of the parentheses when we write the function. There is no limit to the amount of parameters we can include in a function, but each variable name must be separated by a comma. We can then use these `variables` within our function just as we would any other variable.


    function myFunc(parameter1, parameter2) {
        // we can use parameter1 and parameter2
        // in this function just like a variable
    }
    
    logHello();

### Arguments


Once we have our parameters set up in our function, we can now pass data into the function. In order to do this, we will use the parentheses we write when we call the function. We call these pieces of data  `arguments`.  `arguments`  can be ANY data type (string, number, Boolean, object, array, even other functions!). Unlike other languages, JavaScript does not require us to set the data type when we write the function, although you should make an effort to understand what type of data will be coming into the function (and if you are using pre-built functions, you should know what data type that function expects).


To use an argument, just put the data in the function call parentheses like so:


    function logName(name) {
        console.log(name)
    }
    
    logName("Pika"); // => "Pika"
    logName("Mahendra"); // => "Mahendra"

If you have more than one parameter, you will use more than one argument:


    function logPokemon(pokemon, description) {
        console.log(pokemon + " is " desctiontion)
    }
    
    logPokemon("Pika", "awesome!"); // => "Pika is awesome!"

Arguments will always line up with parameters in order, so the first argument will be the first parameter, and etc.


If an argument is not given for a parameter, the parameter will be equal to  `undefined`.


## Learn to explain function scope and the return statement.


In order to effectively use functions, we must be able to return some data from them. In order to return data from functions, we must understand function scope.


### Scope


Scope is defined as what variables we currently have access to and where. So far in this course, we have been working in `Global` scope, in that we can access any variable we have created, anywhere in our code. There are a couple different levels of scope: you may have heard of `block` level scope (used in `if` statements and `for` loops) in which a variable using either `let` or `const` is only available within the statement or loop.


### Function Level Scope


Functions have something similar, known as function scope. Function scope allows us to create variables inside of functions, that are essentially private to that function. We can not reach into a function from the outside and get access to these variables. But we are free to use these variables anywhere within our function. Conversely, we DO have access to variables outside of the function. It is a one-way street. Functions can reach out and grab variables outside of their scope, but we can not reach into a function to get a variable.


    var someVariable = "Hello";
    function myFunc() {
        var someOtherVariable = "World!";
        console.log(someVariable); // => "Hello"
        console.log(someOtherVariable); // => "World!"
    }
    
    myFunc();
    console.log(someVariable); // => "Hello"
    console.log(someOtherVariable); // => someOtherVariable is not defined

### The return statement


We will not console.log everything that comes out of a function. Most likely we will want to return something. There is one way we can access data from within a function. In fact, it is the only way for us to get ANY data from a function, and that is to use the keyword  `return`. Think of the return statement as the only way for data to escape a function. Nothing other than what is returned can be accessed outside of the function. Also note that when a function hits a return statement, the function immediately stops what it is doing and returns.


We can also assign the value of a return statement to another variable, and we will now have access to the data returned from the function.


    function addTwoNumbers(num1, num2) {
        var sum = num1 + num2;
        return sum;
        console.log("this line of code will never be reached);
    }
    
    var result = addTwoNumbers(1, 2)
    console.log(result); // => 3
    console.log(sum); // => sum is not defined
