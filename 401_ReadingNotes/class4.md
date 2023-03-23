# Class 4 Reading Assignment

## Classes and Objects

```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

print(myobjectx.variable)
```

```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()
myobjecty = MyClass()

myobjecty.variable = "yackity"

# Then print out both values
print(myobjectx.variable)
print(myobjecty.variable)
```

## Thinking Recursively

The algorithm for iterative present delivery implemented in Python:

```
houses = ["Eric's house", "Kenny's house", "Kyle's house", "Stan's house"]

def deliver_presents_iteratively():
    for house in houses:
        print("Delivering presents to", house)

```

Appoint an elf and give all the work to him
Assign titles and responsibilities to the elves based on the number of houses for which they are responsible:
> 1 He is a manager and can appoint two elves and divide his work among them
= 1 He is a worker and has to deliver the presents to the house assigned to him

![](https://files.realpython.com/media/elves_7.8d1af1cd85c8.png)

### Things I want to know more about