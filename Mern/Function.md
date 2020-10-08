# Function

_A JavaScript function is a block of code designed to perform a particular task._
JavaScript functions are used to perform operations.A JavaScript function is executed when "something" invokes it (calls it). We can call JavaScript function many times to reuse the code.

### Advantages of Function

1. Code Reusability

   - We can call a function more than one time (several times ) in program.

2. Less Coding
   - We dont need to write code each time to perform the common task.

### Syntax of Function

A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

        //Function Initialization
        function name(p1,p2){
            //executing code
        }

        //Function call
        name('Mark','Shrestha');

## Ways of Writing a Function

1. Expression Syntax
2. Declerative Syntax

### Expression Syntax

    In this syntax, we can define a function inside a expression.

        //Function Initialization
            var work = function(){
                //Code
            }
        //Function Call
             work();

    NOTE :  We cannot call the function before initialization

        //Function Call
            work();
        //Function Initialization
            var work = function(){
                //Code
            }

                This will Produce an TypeError : work is not a function

### Declerative Syntax

    In this syntax, we defines a function with specified name and parameters.
    we can call the function from anywhere.

        //Function Call
            work();
        //Function Initialization
            function work(){
                //Code
            }
        //Function Call
            work();

## Type of Function

1.  Named function expression

        function name(){
            //Code
        }
        name();

2.  UnNamed Function expression

        function(){
            //code
        }

3.  Function with argument

        function detail(name,address){
            //code
        }
        detail('Mark','UK');

4.  Function with return type

        function detail(name,address){
            //code

            return result;
        }
        var resultContainer = detail('Mark','UK');

5.  IIFE(Immediately Invoked Functional Expression)

        (function () {
        // code
        })();
