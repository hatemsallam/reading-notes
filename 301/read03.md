# Lists and Keys
Usually you would render lists inside a component.

We can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.


# Keys

Keys help React identify which items have changed, are added, or are removed.
The best way to pick a key is to use a string that uniquely identifies a list item among its siblings.


We don’t recommend using indexes for keys if the order of items may change. This can negatively impact performance and may cause issues with component state. Check out Robin Pokorny’s article for an in-depth explanation on the negative impacts of using an index as a key. If you choose not to assign an explicit key to list items then React will default to using indexes as keys.

# How to Use the Spread Operator in JavaScript

The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.


# What is the spread operator?
InJavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

“When ...arr is used in the function call, it ‘expands’ an iterable object arr into the list of arguments.” — JavaScript.info

The spread operator was added to JavaScript in ES6 (ES2015), just like the rest parameters, which have the same syntax: three magic dots ….


# What else can … do?
The … spread operator is useful for many different routine tasks in JavaScript, including the following:

- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments
- Adding an item to a list
- Adding to state in React
- Combining objects
- Converting NodeList to an array

In each case, the spread syntax expands an iterable object, usually an array, though it can be used on any interable, including a string.


# Copying an array
Using the … spread operator is a convenient way to copy an array or combine arrays, and it can even add new items:

- const fruits = ['🍏','🍊','🍌','🍉','🍍']
- const moreFruits = [...fruits];
- console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
- fruits[0] = '🍑'
- console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍


# Concatenating arrays
Asseen in the last example, the spread operator can quickly combine two arrays, an operation known as array concatenation:

- const myArray = [`🤪`,`🐻`,`🎌`]
- const yourArray = [`🙂`,`🤗`,`🤩`]
- const ourArray = [...myArray,...yourArray]
- console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩


# Adding an item to a list
Asnoted in the last example, the spread operator can add an item to an another array with a natural, easy-to-understand syntax:


- const fewFruit = ['🍏','🍊','🍌']
- const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
- console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]


# Combining objects
- The spread syntax is useful for combining the properties and methods on objects into a new object:
- const objectOne = {hello: "🤪"}
- const objectTwo = {world: "🐻"}
- const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
- console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
- const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
- objectFour.laugh() // 😂😂😂😂😂


# Increment() Function

 It takes a variable and increments (changes) its value, and also returns this value. The increment can be a positive or negative number. Note: The Increment() function changes the value of its first argument.


 ## Things I want to know more about
I want to know more details about how to pass function between components.