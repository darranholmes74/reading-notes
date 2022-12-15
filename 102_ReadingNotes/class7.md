# Class 7 - Reading Notes

## Control flow

The control flow is the order in which the computer executes statements in a script.
```
if (isEmpty(field)) {
  promptUser();
} else {
  submitForm();
}
```
Control flow means that when you read a script, you must not only read from start to finish but also look at program structure and how it affects order of execution.

## JavaScript Functions

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

```
// Function to compute the product of p1 and p2
function myFunction(p1, p2) {
  return p1 * p2;
}
```

Function parameters are listed inside the parentheses () in the function definition.

Function arguments are the values received by the function when it is invoked.

Inside the function, the arguments (the parameters) behave as local variables.

### Function Return

When JavaScript reaches a return statement, the function will stop executing.

```
let x = myFunction(4, 3);   // Function is called, return value will end up in x

function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
}
```

You can reuse code: Define the code once, and use it many times.

```
function toCelsius(fahrenheit) {
  return (5/9) * (fahrenheit-32);
}
document.getElementById("demo").innerHTML = toCelsius(77);
```

## The () Operator Invokes the Function

Using the example above, toCelsius refers to the function object, and toCelsius() refers to the function result.

```
function toCelsius(fahrenheit) {
  return (5/9) * (fahrenheit-32);
}
document.getElementById("demo").innerHTML = toCelsius;
```

## Functions Used as Variable Values

Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations.

Instead of using a variable to store the return value of a function:

```
let x = toCelsius(77);
let text = "The temperature is " + x + " Celsius";
```

```
You can use the function directly, as a variable value:

let text = "The temperature is " + toCelsius(77) + " Celsius";
```

## Local Variables

Variables declared within a JavaScript function, become LOCAL to the function.

Local variables can only be accessed from within the function.

```
// code here can NOT use carName

function myFunction() {
  let carName = "Volvo";
  // code here CAN use carName
}

// code here can NOT use carName
```

## JavaScript Operators

The Assignment Operator (=) assigns a value to a variable.

```
// Assign the value 5 to x
let x = 5;
// Assign the value 2 to y
let y = 2;
// Assign the value x + y to z:
let z = x + y;
```
The Addition Operator (+) adds numbers:

```
let x = 5;
let y = 2;
let z = x + y;
```

### JavaScript Arithmetic Operators

Arithmetic Operators are used to perform arithmetic on numbers.

```
let a = 3;
let x = (100 + 50) * a;
```

Adding two numbers, will return the sum, but adding a number and a string will return a string.

```
let x = 5 + 5;
let y = "5" + 5;
let z = "Hello" + 5;
```

JavaScript Comparison Operators

```
==	equal to
===	equal value and equal type
!=	not equal
!==	not equal value or not equal type
>	greater than
<	less than
>=	greater than or equal to
<=	less than or equal to
?	ternary operator
```


#### References

https://developer.mozilla.org/en-US/docs/Glossary/Control_flow

https://www.w3schools.com/js/js_functions.asp

https://www.w3schools.com/js/js_operators.asp



