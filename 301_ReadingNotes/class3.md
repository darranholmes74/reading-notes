# Class 3 Reading Assignment

## React Docs - lists and keys

1. Map() returns a new array.

2. You can use `<li>{}</li>`.

3. The best way to pick a key is to use a string that uniquely identifies a list item among its siblings. Most often you would use IDs from your data as keys.

4. Keys help React identify which items have changed, are added, or are removed.

## The Spread Operator

1. In JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

2. 
* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments

3. 
`const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍`

4. 

const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]

5. 

const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂

## How to Pass Functions Between Components

1. Create an arrow-function to loop through the state and find the correct item.

2. The increment function loops through the state to find the correct item that was clicked on.

3. using array.map function and an if statement.

4. this.props.increment() and pass through the name parameter.

## Things I would like to know more about


## References

https://reactjs.org/docs/lists-and-keys.html
https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab
