# Forms
HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state. 


# Controlled Components
In HTML, form elements such as input tag, textarea tag, and select tag typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.


# Handling Multiple Inputs

When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.


# Controlled Input Null Value
Specifying the value prop on a controlled component prevents the user from changing the input unless you desire so. If you’ve specified a value but the input is still editable, you may have accidentally set value to undefined or null.


# Alternatives to Controlled Components
It can sometimes be tedious to use controlled components, because you need to write an event handler for every way your data can change and pipe all of the input state through a React component. This can become particularly annoying when you are converting a preexisting codebase to React, or integrating a React application with a non-React library.


# Fully-Fledged Solutions
If you’re looking for a complete solution including validation, keeping track of the visited fields, and handling form submission, Formik is one of the popular choices. However, it is built on the same principles of controlled components and managing state — so don’t neglect to learn them.




# JavaScript — The Conditional (Ternary) Operator Explained


Starting With the Basics — The if statement
Using a conditional, like an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met.



# ternary operator

condition ? value if true : value if false



## Here’s what you need to know:
- The condition is what you’re actually testing. The result of your condition should be true or false or at least coerce to either boolean value.
- A ? separates our conditional from our true value. Anything between the ? and the : is what is executed if the condition evaluates to true.
- Finally a : colon. If your condition evaluates to false, any code after the colon is executed.


## Ternary Operator example
-  if(x===y){
- console.log(true) ;
-   } else {
 - console.log(false);
 -  }


## Rewrite 

x = y  ? console.log(true) : console.log(false);



 ## Things I want to know more about
more details about the Conditional Ternary Operator
 



