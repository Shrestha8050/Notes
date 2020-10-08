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
        ~~ work();~~
         //Function Initialization
        var work = function(){
            //Code
        }

### Declerative Syntax

        //Function Initialization

         function work(){
            //Code
        }

        //Function Call
        work();
