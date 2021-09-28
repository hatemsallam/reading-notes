# OOP

## Object-Oriented Programming Concepts

- Class : Is a blue print That have specific "real world" state and behavior and used to model real world objects .

- Object : Is an instance of what called a class Have it's own state and behavior , it's a small copy of that class .


## Classes :

- Think of objects like an instance of a more generalized blue print which is the class .

- Classes are ways to model different kind of objects with a blue print of a specific behavior .

- Classes uses instance variables for modeling the states .

- Classes uses methods to model the behavior .

### Declaring a class : 
- A class will have at the ver begining the name of the class followed by :
    - extends to inherit another class (Only one subclass) .
    - Implements to implement whatever interface we want to use(Multiple allowed seperated by commas ) .
- Followed by {} and inside it the body of the class .
- Access modifiers (Public , private) to initialize states and behaviors (Private only applied for nested classes ).
- **The class name inital letters are capital according to the naming convention .**


### Declaring Member Variables

- Kinds of variables :
    - Fields : class member variables .
    - Local variables : variables in a block of code (e.g : Methods) .
    - parameters : Variables which are passed to methods .

- To Declare member variables : 
    - Access modifier at the very begining to restrict access .
        - Private : Accesible only from it's class .
        - Public : Visible and accesible from all of the project or classes .

    - Types : Declare the type after the access modifier (int , double ,Integer , Double)  .

    - Followed by the name of the variable following the naming convention will be better .

### Defining a method :

- The required components of method are the return type , the name , () and the body of it inside {} .

- Components of method :
    - Access modifiers : public , private to restrict access .
    - Return type : datat type that the method should return .
    - The name of the method : camel cased is preffered .
    - The list of parameters : that the method will do operations among .
    - exception list .
    - The method body : the block of code which will be compiled when calling the method .

- Naming a method : 

    - Method names might not be unique due to overloading .
    - Camel case is used to name methods (by convention).

- Method overloading : 

    - Java can identify methods by it's signature .
    - Overloading is to add two methods with the same name with different parameter signature .
    - it should be used sparingly due to it make the code less readable .

### Constructors :

- Constructors are invoked to create a new object .

- Constructor name must be the same as the class name , with no return type .

- It will be called directly when the object is created .

- They are called using the newKeyword .

- Java initializes a default no-arg constructor .

- It can have access modifiers to restrict access .


### Passing data to methods or constructors : 

- The declaration of a method or a constructor contains the number and types of arguments that will be used in the method .

- Parameters are the name and type that is defined with the method , constructor .

- Arguments are the real values that is passed to these methods .

- You can use the varagas construct to pass an arbitary number of parameters to the method .

- It is used when you dont know how many of a particular type would be passed to a method .

- Parameters can be a primitive type or a reference type .

- parameters must be provided to a name that is unique to it's scope .

- Name of parameter can be the same of the data member name .

- Primitive data types are called by value that means that when editing it's value it will not change in the global scope .

- Reference data types are passed by value but there value can change if the right access is provided .



## Objects :

- In programming aspects objects have states and behaviors which can expressed through Instance variables and methods for behavior .

- Think of a car object as an example : It have the states of color , model , engine Capacity and the behaviors of driving , changing gears or braking for example .

- Advantages of working with objects are :
    - Modularity : Each object can be maintained and worked with independantly .
    - Information Hiding : It uses some programming concepts to hide the operations of that specific object .
    - Code re-use : The developer can get use of another software developer object which will enhance the process of coding .
    - Pluggability : Easir to debug and fix problems while using objects .

- Creating object : 
    - Declare using the name of the class followed by the name of the object .
    - instantiate : using the new keyword that will create the object .
    - Initialize : the new keyword will call the constructor to initialize the object .

### Using Objects :

- To refer to an object field you can do that by the name of object then .the name of the field .

- The same applies to refer to a method followed by paranthesses (and arguments if exists) .

- **Garbage collector is a handy way built-in in java to destroy objects that are no longer needed to use .**


### Return a value from method : 

- A method return a value if it completes the whole code .

- Reaches a return statement .

- throws an exception .

- we Use the return keyword too return a value from a method .

- We can return a class or interface from a method if provided .


### using this keyword :

- this refers to the current object .

- can be used to refer to a field in constructor if same names are provided .

- this can be used to call another constructor with the following constructos this(par , par , par) this will call the constructor with the 3 parameters .


### Static variables and methods : 

- static is declared once in the memory . 

- can be accessed from a static context without the need to create an instance of that class .

- final keyword is used to declare constants which can't be changed when initialized .


### Decimal numbers : 

- Uses base 10 to count .

- The decimal point helps to know the position of each number .

- Consists of base 1 and base 0 combined .

### Binary numbers :

- base 2 numbers system .

- You start counting from zero to one there is no other digits to use . 

- digit at position (if 1 ) represents 2 to the power of the position .

- The value of the number is the sum of all 1's values .

- this system is used in computers .


### Hexadecimal numbers :

- base 16 number system .

- start counting from 0 to 16 .

- there are digits from 0 to 9 .

- from 10 to 15 letters from A to F .