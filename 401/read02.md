# Packages and Import 

## Package declaration

The first statement, other than comments, in a Java source file, must be the package declaration.

Following the optional package declaration, you can have import statements, which allow you to specify classes from other packages that can be referenced without qualifying them with their package.

Default package. Altho all Java classes are in a directory, it's possible to omit the package declaration. For small programs it's common to omit it, in which case Java creates what it calls a default package. Sun recommends that you do not use default packages.



## Package declaration syntax 

The statement order is as follows. Comments can go anywhere.

- Package statment (optional).
- Imports (optional).
- Class or interface definitions.



## Common imports


There are 166 packages containing 3279 classes and interfaces in Java 5. However, only a few packages are used in most programming. GUI programs typically use at least the first three imports.

import java.awt.*;	Common GUI elements.
import java.awt.event.*;	The most common GUI event listeners.
import javax.swing.*;	More common GUI elements. Note "javax".
import java.util.*;	Data structures (Collections), time, Scanner, etc classes.
import java.io.*;	Input-output classes.
import java.text.*;	Some formatting classes.
import java.util.regex.*;	Regular expression classes.



## Static imports in Java 5


Java 5 added an import static option that allows static variables (typically constants) to be referenced without qualifying them with a class name. For example, after

import static java.awt.Color;
It would then be possible to write

   Color background = RED;
instead of

   Color background = Color.RED;
Adding this "feature" wasn't the best idea because it leads to name pollution and confusion about which class constants come from. Even Sun (see References below) basically advises not to use it!



## A Guide to Java Loops

### Intro to Loops
In programming languages, looping is a feature which facilitates the execution of a set of instructions until the controlling Boolean-expression evaluates to false.

Java provides different types of loops to fit any programming need. Each loop has its own purpose and a suitable use case to serve.

Here are the types of loops that we can find in Java:

Simple for loop
Enhanced for-each loop
While loop
Do-While loop


### For Loop
A for loop is a control structure that allows us to repeat certain operations by incrementing and evaluating a loop counter.


###  While Loop
The while loop is Java's most fundamental loop statement. It repeats a statement or a block of statements while its controlling Boolean-expression is true.

For a detailed example, have a look at the dedicated post: Java While Loop.

### Do-While Loop
The do-while loop works just like the while loop except for the fact that the first condition evaluation happens after the first iteration of the loop.

For a detailed example, have a look at the dedicated post: Java Do-While Loop.