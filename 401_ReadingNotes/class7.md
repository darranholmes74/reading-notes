# Class 7 Reading Notes

## Python Scope

1. Python scope is used to assign variables to a single function or to multiple depending on the scope.

2. A situation you can us Python scope is with local and global scope.
If you make a variable inside a function but assign it global, that variable can be used outside that function as well.

3. 
### Local scope 
- is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function. These names will only be visible from the code of the function.

### Enclosing scope - 
is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function.

### Global scope 
- is the top-most scope in a Python program, script, or module. This Python scope contains all of the names that you define at the top level of a program or a module.

### Built-in scope 
- is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python.

## Big O is simpler than you might think

The video shed some light on how the Big O works. It showed how different growth patterns like exponentiall polynomial constant exc. relate to each other and how to notate then using the Big O notation.

### Things I want to know more about