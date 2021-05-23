# HTML
When creating a web page, you add tags
(known as markup) to the contents of the
page. These tags provide extra meaning
and allow browsers to show users the
appropriate structure for the page.

## - Headings
HTML has six "levels" of
headings:
h1 is used for main headings
h2 is used for subheadings
If there are further sections
under the subheadings then the
h3 element is used, and so
on...

## - Paragraph
To create a paragraph, surround
the words that make up the
paragraph with an opening p
tag and closing /p tag.
By default, a browser will show
each paragraph on a new line
with some space between it and
any subsequent paragraphs.

## - White Space
In order to make code easier to
read, web page authors often
add extra spaces or start some
elements on new lines.
When the browser comes across
two or more spaces next to each
other, it only displays one space.
Similarly if it comes across a line
break, it treats that as a single
space too. This is known as
white space collapsing.
You will often see that web page
authors take advantage of white
space collapsing to indent their
code in order to make it easier
to follow.

## - Visual Editors & Their Code views

### Visual editors 
often resemble
word processors. Although
each editor will differ slightly,
there are some features that
are common to most editors
that allow you to control the
presentation of text.

### Code views 
show you the code
created by the visual editor so
you can manually edit it, or so
you can just enter new code
yourself. It is often activated
using a button with an icon
that says HTML or has angled
brackets. White space may be
added to the code by the editor
to make the code easier to read.

## - Semantic Markup
There are some text elements that are not intended to affect the
structure of your web pages, but they do add extra information to the
pages — they are known as semantic markup.

- Strong & Emphasis
- Quotations
- Abbreviations & Acronyms
- Citations & Definitions
- Author Details
- Changes to Content

# CSS

CSS allows you to create rules that specify how the content of
an element should appear. For example, you can specify that
the background of the page is cream, all paragraphs should
appear in gray using the Arial typeface, or that all level one
headings should be in a blue, italic, Times typeface.

## how css works ?
CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration.

### Selectors 
indicate which
element the rule applies to.
The same rule can apply to
more than one element if you
separate the element names
with commas.

### Declarations 
indicate how
the elements referred to in
the selector should be styled.
Declarations are split into two
parts (a property and a value),
and are separated by a colon.

### CSS declarations
 sit inside curly brackets and each is made up of two
parts: a property and a value, separated by a colon. You can specify
several properties in one declaration, each separated by a semi-colon.



# What is Javascript?
JavaScript is a scripting or programming language that allows you to implement complex features on web pages — every time a web page does more than just sit there and display static information for you to look at.

## How does it work?

### Expressions and operators

#### Operators
JavaScript has the following types of operators. This section describes the operators and contains information about operator precedence.

- Assignment operators such as (x += y)	it means (x = x + y)
- Comparison operators such as ( < ) or  ( > )
- Arithmetic operators such as addition or substraction
- Bitwise operators such as (and) , (or) 
- Logical operators
- String operators
- Conditional (ternary) operator
- Comma operator
- Unary operators
- Relational operators


# Logical operators 
Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value. However, the && and || operators actually return the value of one of the specified operands, so if these operators are used with non-Boolean values, they may return a non-Boolean value. The logical operators are described in the following table.

# Loops
Loops offer a quick and easy way to do something repeatedly. This chapter of the JavaScript Guide introduces the different iteration statements available to JavaScript.

You can think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another. For example, the idea "Go five steps to the east" could be expressed this way as a loop:

## for statement 
A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.

 

## while statement
A while statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:

while (condition)
  statement
If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while.

## break statement
Use the break statement to terminate a loop, switch, or in conjunction with a labeled statement.

When you use break without a label, it terminates the innermost enclosing while, do-while, for, or switch immediately and transfers control to the following statement.
When you use break with a label, it terminates the specified labeled statement.



