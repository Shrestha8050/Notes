# Modular Programming

Modular programming is a software design technique that emphasizes separating the functionality of a program into independent, interchangeable modules, such that each contains everything necessary to execute only one aspect of the desired functionality.

# Node.js Module

    A set of functions you want to include in your application.

# Built-in Modules

    - Node.js has a set of built-in modules which you can use without any further installation.
    - such as:- buffer , fs , http , net , os ,path , vm , v8, url etc.

# Include Modules

    - To include a module, we use the require() function with the name of the module
    - To define your own modules, you need to define their path.
    - Example :
        -> var fs = require('fs');
        -> var date= require('./date');

# Creating your own module

    1. Create two files
    ![1st](https://user-images.githubusercontent.com/58983458/95645745-db69de80-0ae1-11eb-8416-d55239819aff.PNG)
    2. Export the module (Required module.exports ) 
    ![2nd](https://user-images.githubusercontent.com/58983458/95645783-41eefc80-0ae2-11eb-8ae8-761618ed7f24.PNG)
    2. Include in the main file
    ![3](https://user-images.githubusercontent.com/58983458/95645828-94c8b400-0ae2-11eb-99e5-bfbe32356174.PNG)

