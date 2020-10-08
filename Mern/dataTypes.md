# Data Type

_In computer science and computer programming,_ a data type or simply type is an attribute of data which tells the compiler or interpreter how the programmer intends to use the data.
or
Data Type is the Classification of the data where we can define the type of the data according to our need and specification.

**_JavaScript is a loosely type or dynamic type language, means you don't need to specify type of the variable because it is dynamically used by JavaScript engine._**

JavaScript provides different data types to hold different types of values.

## There are two types of data types in JavaScript.

- Primitive data type
- Non-primitive (reference) data type

## Primitive data

1.  String

        - Represents a sequense of characters
        - Single quote or double quote represents a character or string
        - Example :
        - var name = Mark';
        - var address = "somewhere in the earth";
        - var character = 'a' || "b";

2.  Number

        - Represents a number
        - Example :
        - var number = 2;
        - var num = 1.222;
        - var n = 12e10; (e10 means exponential || base 10 with power 10 || e^10 )

3.  Boolean

        - Represents a boolean value i.e true or false
        - Example :
        - var bool = true;
        - var boolean = false;

4.  Undefined

        - Represents undefined value(memory is located but value is not assigned).
        - Example :
        - var x;

5.  Null

        - Represents null i.e no value at all

## Non-primitive Data type

1.  Object

        -Colection of key(or name) value pair
        - Represents a collection of properties(member) through which we can access properties(member)
        - Example :
        - var obj = {
            name : 'Mark',
            key: 'value'
            }
        - var obj1 = new Object();

2.  Array

        -Holds multiple values
        - Represents group of similar values

        - Example :
            - var arr = ['hello' , 'world'];
            - var color = new Array("red", "blue", "green");

3.  RegExp

        - Represents regular Expression
        - Example :
        - var expression = /hello/i;

## Dynamic types in JavaScript

    Means that the same variable can hold the different data types.

    Example:-
        var x ; // **Here we defined a variable and the_datatype of x is undefined_ because the memory is allocated but the value is not assigned.**//
        x= 4;    // **Here we assign Number 4 in variable x, so the _datatype of x is Number _ **//
        x="hello"; // **Here we assign string hello in variable x, so the _datatype of x is String_ **//
        x=true; // **Here we assign boolean value true in variable x, so the _datatype of x is Boolean_**//

    In this Example, x is a variable which has the dynamic capacity to store the different types of data as provided by the programmer.
