# Error Handling and Debugging
When you are writing JavaScript, do not expect to write it perfectly the first time.
Programming is like problem solving: you are given a puzzle and not only do you have to solve
it, but you also need to create the instructions that allow the computer to solve it. too.


## ORDER OF EXECUTION

To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run.


## EXECUTION CONTEXTS

The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope.

EXECUTION CONTEXT
Every statement in a script lives in one of three
execution contexts:
- GLOBAL CONTEXT
Code that is in the script, but not in a function.
There is only one global context in any page.
- FUNCTION CONTEXT
Code that is being run within a function.
Each function has its own function context.
- EVAL CONTEXT
Text is executed like code in an internal function
called eval.



## UNDERSTANDING ERRORS

If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code.

If you are anticipating that something in your code
may cause an error, you can use a set of statements
to handle the error.
This is important because if the error is not handled,
the script will just stop processing and the user will
not know why. So exception-handling code should
inform users when there is a problem.


## HOW TO DEAL WITH ERRORS


1. DEBUG THE SCRIPT TO FIX ERRORS
If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.
You will find that the developer tools available in
every major modern browser will help you with
this task. In this chapter, you will learn about the
developer tools in Chrome and Firefox. (The tools in
Chrome are identical to those in Opera.)
IE and Safari also have their own tools (but there is
not space to cover them all).


2. HANDLE ERRORS GRACEFULLY
You can handle errors gracefully using try, catch,
throw, and f i na 1 ly statement s.
Sometimes, an error may occur in the script for a
reason beyond your control. For example, you might
request data from a third party, and their server
may not respond. In such cases, it is particularly
important to write error-handling code.
In the latter part of the chapter, you will learn how to
gracefully check whether something will work, and
offer an alternative option if it fails.


## DEBUGGING TIPS

Here are a selection of practical tips that you
can try to use when debugging your scripts.


- ANOTHER BROWSER
Some problems are browserspecific.
Try the code in another
browser to see which ones are
causing a problem.

- ADD NUMBERS
Write numbers to the console
so you can see which the items
get logged. It shows how far your
code runs before errors stop it.

- STRIP IT BACK
Remove parts of code, and strip
it down to the minimum you
need. You can do this either by
removing the code altogether, or
by just commenting it out using
multi-line comments:
/* Anything between these
characters is a cofllllent */

- EXPLAINING THE CODE
Programmers often report
finding a solution to a problem
while explaining the code to
someone else.

- CODE PLAYGROUNDS
If you want to ask about
problematic code on a forum, in
addition to pasting the code into
a post, you could add it to a code
playground site (such as
JSBin.com, JSFiddle. com, or
Dabbl et. corn) and then post a
link to it from the forum.

- VALIDATION TOOLS
There are a number of on line
validation tools that can help you
try to find errors in your code:
JAVASCRIPT
http://www.jslint.com
http://www.jshint .com
JSON
http:// www.jsonlint.com


- JQUERY
There is a jQuery debugger
plugin available for Chrome
which can be found in the
Chrome web store.