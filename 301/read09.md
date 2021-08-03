# Concepts of Functional Programming in Javascript


## What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.



## What is a pure function and how do we know if something is a pure function?


The first fundamental concept we learn when we want to understand functional programming


- It returns the same result if given the same arguments (it is also referred as deterministic)
- It does not cause any observable side effects.



## What are the benefits of a pure function?


The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts






## What is immutability?


When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.




## What is Referential transparency?



Basically, if a function consistently yields the same result for the same input, it is referentially transparent.





# Node.js

## What is a module?

is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node. js application. Each module in Node. js has its own context, so it cannot interfere with other modules or pollute global scope.


## What does the word ‘require’ do?

The require() method is used to load and cache JavaScript modules. So, if you want to load a local, relative JavaScript module into a Node. js application, you can simply use the require() method.



## How do we bring another module into the file the we are working in?

require and pass




## What do we have to do to make a module available?


module.export


