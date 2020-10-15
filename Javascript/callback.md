# Callback

    - A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.
    - Callback is used to handle the result of Async call.

# HOF(Higher Order Function)

    A higher order function (HOF) is a function that follows at least one of the following conditions −
        - Takes on or more functions as argument
        - Returns a function as its result

### For example

    //For Synchronous Call
    // This is HOF as it takes sayhello function as it accepts the function as an argument
    function sayHello(name, sayhello) {
        const say = 'Welcome ' + name;
        sayhello(say);
    }
    // callback Function as it is passed as an argument
    sayHello('Hari', function (result) {
        console.log(result);
    });

    //For Asynchronous  Call
    // This is HOF as it takes sayhello function as it accepts the function as an argument
    function sayHello(name, sayhello) {
        const say = 'Welcome ' + name;
        setTimeout(function () {
            sayhello(say);
        }, 200);
    }

    // callback Function as it is passed as an argument
    sayHello('Hari', function (result) {
        console.log('Called after 2s ');
        console.log(result);
    });

### Note that we can call the callback function inside of callbackDemo as many times as we like.

    function callbackDemo (var1, callback) {
        callback(var1);
        callback(var1);
    }

    callbackDemo (20, function (x) {
        console.log(x);
    });
    There is no limit to how many times we can call it.

### The other thing to pay attention to is that you can pass in as many callback functions as you like to another function.

    function callbackDemo (var1, var2, callback1, callback2) {
        callback1(var1);
        callback2(var2);
    }

    callbackDemo (12,22,function (x) {
        console.log(x);
    },
    function (x) {
        console.log(x);
    }
    );

    Here in function callbackDemo we pass in two variables and two functions as arguments.
    Inside of function callbackDemo, we run callback1 with variable 1 and we run callback2 with variable 2.
