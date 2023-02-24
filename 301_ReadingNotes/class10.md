## Understanding the JavaScript Call Stack


1. At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).


2. 1


3. Last In, First Out data structure.


4. ```function printMessage(message) {
console.log(message);
}


function greetUser(name) {
const message = `Hello, ${name}!`;
printMessage(message);
}


function main() {
greetUser("John");
}


main();```


5. Occurs when there is a recursive function (a function that calls itself) without an exit point.


## JavaScript error messages


1. When you try to use a variable that is not yet declared.


2. When you have something that cannot be parsed in terms of syntax.


3. Trying to manipulate an object with some kind of length and give it an invalid length


4. These types of errors show up when the types (number, string, and so on) you are trying to use or access are incompatible.


5. Makes your code stop running at a certain point.


6. How you achieve a breakpoint.

### Things I want to know more about

## References

https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4