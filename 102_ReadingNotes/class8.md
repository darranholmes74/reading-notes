# Expressions and Operators

## Assignment operators

At a high level, an expression is a valid unit of code that resolves to a value. There are two types of expressions: those that have side effects (such as assigning values) and those that purely evaluate.

An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = f() is an assignment expression that assigns the value of f() to x.

```
Assignment	x = f()	x = f()
Addition assignment	x += f()	x = x + f()
Subtraction assignment	x -= f()	x = x - f()
Multiplication assignment	x *= f()	x = x * f()
Division assignment	x /= f()	x = x / f()
Remainder assignment	x %= f()	x = x % f()
Exponentiation assignment	x **= f()	x = x ** f()
Left shift assignment	x <<= f()	x = x << f()
Right shift assignment	x >>= f()	x = x >> f()
Unsigned right shift assignment	x >>>= f()	x = x >>> f()
Bitwise AND assignment	x &= f()	x = x & f()
Bitwise XOR assignment	x ^= f()	x = x ^ f()
Bitwise OR assignment	x |= f()	x = x | f()
Logical AND assignment	x &&= f()	x && (x = f())
Logical OR assignment	x ||= f()	x || (x = f())
Nullish coalescing assignment	x ??= f()	x ?? (x = f())
```

If an expression evaluates to an object, then the left-hand side of an assignment expression may make assignments to properties of that expression. For example:

const obj = {};

```
obj.x = 3;
console.log(obj.x); // Prints 3.
console.log(obj); // Prints { x: 3 }.

const key = "y";
obj[key] = 5;
console.log(obj[key]); // Prints 5.
console.log(obj); // Prints { x: 3, y: 5 }.
Copy to ClipboardCopy to Clipboard
```

If an expression does not evaluate to an object, then assignments to properties of that expression do not assign.

```
const val = 0;
val.x = 3;

console.log(val.x); // Prints undefined.
console.log(val); // Prints 0.
```

It is an error to assign values to unmodifiable properties or to properties of an expression without properties (null or undefined).

Destructuring

const foo = ['one', 'two', 'three'];

```
// without destructuring
const one   = foo[0];
const two   = foo[1];
const three = foo[2];

// with destructuring
const [one, two, three] = foo;
Copy to ClipboardCopy to Clipboard
```

Evaluation and nesting

```
// Declares a variable x and initializes it to the result of f().
// The result of the x = f() assignment expression is discarded.
let x = f();

x = g(); // Reassigns the variable x to the result of g().
```

## Comparison operators

A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values.

```
const var1 = 3;
const var2 = 4;
```

```
Equal (==)	Returns true if the operands are equal.	3 == var1
"3" == var1
3 == '3'
Not equal (!=)	Returns true if the operands are not equal.	var1 != 4
var2 != "3"
Strict equal (===)	Returns true if the operands are equal and of the same type. See also Object.is and sameness in JS.	3 === var1
Strict not equal (!==)	Returns true if the operands are of the same type but not equal, or are of different type.	var1 !== "3"
3 !== '3'
Greater than (>)	Returns true if the left operand is greater than the right operand.	var2 > var1
"12" > 2
Greater than or equal (>=)	Returns true if the left operand is greater than or equal to the right operand.	var2 >= var1
var1 >= 3
Less than (<)	Returns true if the left operand is less than the right operand.	var1 < var2
"2" < 12
Less than or equal (<=)	Returns true if the left operand is less than or equal to the right operand.	var1 <= var2
var2 <= 5
```

## Loops and Iteration

You can think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another. For example, the idea "Go five steps to the east" could be expressed this way as a loop:

```
for (let step = 0; step < 5; step++) {
  // Runs 5 times, with values of step 0 through 4.
  console.log('Walking east one step');
}
```

The statements for loops provided in JavaScript are:

for statement - A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.

do...while statement - The do...while statement repeats until a specified condition evaluates to false.

while statement - A while statement executes its statements as long as a specified condition evaluates to true.

labeled statement - A label provides a statement with an identifier that lets you refer to it elsewhere in your program.

break statement - Use the break statement to terminate a loop, switch, or in conjunction with a labeled statement.


continue statement - The continue statement can be used to restart a while, do-while, for, or label statement.


for...in statement - The for...in statement iterates a specified variable over all the enumerable properties of an object.

for...of statement- The for...of statement creates a loop Iterating over iterable objects (including Array, Map, Set, arguments object and so on), invoking a custom iteration hook with statements to be executed for the value of each distinct property.

### for statement

HTML

```
<form name="selectForm">
  <label for="musicTypes">Choose some music types, then click the button below:</label>
  <select id="musicTypes" name="musicTypes" multiple>
    <option selected>R&B</option>
    <option>Jazz</option>
    <option>Blues</option>
    <option>New Age</option>
    <option>Classical</option>
    <option>Opera</option>
  </select>
  <button id="btn" type="button">How many are selected?</button>
</form>
```

### JavaScript

```
function howMany(selectObject) {
  let numberSelected = 0;
  for (let i = 0; i < selectObject.options.length; i++) {
    if (selectObject.options[i].selected) {
      numberSelected++;
    }
  }
  return numberSelected;
}

const btn = document.getElementById('btn');

btn.addEventListener('click', () => {
  const musicTypes = document.selectForm.musicTypes;
  console.log(`You have selected ${howMany(musicTypes)} option(s).`);
});
```

### While Statement

```
while (condition)
  statement
```


### References

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#assignment_operators

https://canvas.instructure.com/courses/5713005/discussion_topics/16453811?module_item_id=75786747
