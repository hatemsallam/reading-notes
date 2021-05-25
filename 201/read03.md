# lists in html
There are lots of occasions when we
need to use lists. HTML provides us with
three different types:

- Ordered lists are lists where each item in the list is
numbered. For example, the list might be a set of steps for
a recipe that must be performed in order, or a legal contract
where each point needs to be identified by a section
number.

- Unordered lists are lists that begin with a bullet point
(rather than characters that indicate order).

- Definition lists are made up of a set of terms along with the
definitions for each of those terms.

## Summary
There are three types of HTML lists: ordered,unordered, and definition.
- Ordered lists use numbers.
- Unordered lists use bullets.
- Definition lists are used to define terminology.
- Lists can be nested inside one another.

# Boxes in css

## Boxes Dimensions
## width, height


The most popular ways to
specify the size of a box are
to use pixels, percentages, or
ems. Traditionally, pixels have
been the most popular method
because they allow designers to
accurately control their size.
When you use percentages,
the size of the box is relative to
the size of the browser window
or, if the box is encased within
another box, it is a percentage of
the size of the containing box.
When you use ems, the size
of the box is based on the size
of text within it. Designers
have recently started to use
percentages and ems more for
measurements as they try to
create designs that are flexible
across devices which have
different-sized screens.

## Limiting Width
## min-width, max-width
Some page designs expand and
shrink to fit the size of the user's
screen. In such designs, the
min-width property specifies
the smallest size a box can be
displayed at when the browser
window is narrow, and the
max-width property indicates
the maximum width a box can
stretch to when the browser
window is wide.
These are very helpful properties
to ensure that the content of
pages are legible (especially on
the smaller screens of handheld
devices). For example, you can
use the max-width property to
ensure that lines of text do not
appear too wide within a big
browser window and you can
use the min-width property
to make sure that they do not
appear too narrow.
You may find it helpful to try this
example out in your browser so
that you can see what happens
when you increase or decrease
the size of the browser window.

## Limiting Height
## min-height, max-height

In the same way that you might
want to limit the width of a box
on a page, you may also want
to limit the height of it. This is
achieved using the min-height
and max-height properties.
The example on this page
demonstrates these properties
in action. It also shows you what
happens when the content of the
box takes up more space than
the size specified for the box.
If the box is not big enough to
hold the content, and the content
expands outside the box it can
look very messy. To control
what happens when there is not
enough space for the content of
a box, you can use the overflow
property, which is discussed on
the next page.

## Overflowing Content
## overflow

The overflow property tells the
browser what to do if the content
contained within a box is larger
than the box itself. It can have
one of two values:
hidden
This property simply hides any
extra content that does not fit in
the box.
scroll
This property adds a scrollbar to
the box so that users can scroll
to see the missing content.
On the left, you can see two
boxes whose contents expand
beyond their set dimensions. The
first example has the overflow
property with a value of hidden.
The second example has the
overflow property with a value
of scroll.
The overflow property is
particularly handy because some
browsers allow users to adjust
the size of the text to appear as
large or as small as they want. If
the text is set too large then the
page can become an unreadable
mess. Hiding the overflow on
such boxes helps prevent items
overlapping on the page.

## Border Style
can control the style of a
border using the border-style
property. This property can take
the following values:
solid a single solid line
dotted a series of square dots
(if your border is 2px wide, then
the dots are 2px squared with a
2px gap between each dot)
dashed a series of short lines
double two solid lines (the
value of the border-width
property creates the sum of the
two lines)
groove appears to be carved
into the page
ridge appears to stick out from
the page
inset appears embedded into
the page
outset looks like it is coming
out of the screen
hidden / none no border is
shown
You can individually change the
styles of different borders using:
border-top-style
border-left-style
border-right-style
border-bottom-style


## border-color



You can specify the color of a
border using either RGB values,
hex codes or CSS color names
(as you saw on pages 251-252).
It is possible to individually
control the colors of the borders
on different sides of a box using:
border-top-color
border-right-color
border-bottom-color
border-left-color
It is also possible to use a
shorthand to control all four
border colors in the one
property:
border-color: darkcyan
deeppink darkcyan
deeppink;
The values here appear in
clockwise order: top, right,
bottom, left.
You could also use HSL values
to specify the color as shown
on pages 255-256. However,
these were only introduced in
CSS3 and will not work in older
browsers.

## padding
The padding property allows
you to specify how much space
should appear between the
content of an element and its
border.
The value of this property is
most often specified in pixels
(although it is also possible to
use percentages or ems). If a
percentage is used, the padding
is a percentage of the browser
window (or of the containing box
if it is inside another box).
Please note: If a width is
specified for a box, padding is
added onto the width of the box.
As you can see, the second
paragraph here is much easier
to read because there is a space
between the text and the border
of the box. The box is also wider
because it has padding.
You can specify different values
for each side of a box using:
padding-top
padding-right
padding-bottom
padding-left

## summary 
- CSS treats each HTML e XX lement as if it has its own box.
- You can use CSS to control the dimensions of a box.
- You can also control the borders, margin and padding
for each box with CSS.
- It is possible to hide elements using the display and
visibility properties.
- Block-level boxes can be made into inline boxes, and
inline boxes made into block-level boxes.
- Legibility can be improved by controlling the width of
boxes containing text and the leading.
- CSS3 has introduced the ability to create image
borders and rounded borders.


# USING QUOTES INSIDE A STRING (js)
Sometimes you will want to use
a double or single quote mark
within a string.
Because strings can live in single
or double quotes, if you just
want to use double quotes in the
string, you could surround the
entire string in single quotes.
If you just want to use single
quotes in the string, you could
surround the string in double
quotes (as shown in the third line
of this code example).
You can also use a technique
called escaping the quotation
characters. This is done by
using a backwards slash (or
"backslash") before any type of
quote mark that appears within
a string (as shown on the fourth
line of this code sample).
The backwards slash tells the
interpreter that the following
character is part of the string,
rather than the end of it.

# USING A VARIABLE TO STORE A BOOLEAN
A Boolean variable can only have
a va lue of true or fa 1 se, but this
data type is very helpful.
In the example on the right, the
values true or fa 1 se are used
in the cl ass attributes of HTML
elements. These values trigger
different CSS class rules: true
shows a check, fa 1 se shows a
cross. (You learn how the class
attribute is set in Chapter 5.)
It is rare that you would want to
write the words true or false
into the page for the user to read,
but this data type does have two
very popular uses:
First, Booleans are used when
the value can only be true/
fa 1 se. You could also think of
these values as on/off or 0/1:
true is equivalent to on or 1,
fa 1 se is equivalent to off or 0
Second, Booleans are used when
your code can take more than
one path. Remember, different
code may run in different
circumstances (as shown in the
flowcharts throughout the book).

## SHORTHAND FOR CREATING VARIABLES

Programmers sometimes use
shorthand to create variables.
Here are three variations of how
to declare variables and assign
them values:
1. Variables are declared and
values assigned in the same
statement.
2. Three variables are declared
on the same line, then values
assigned to each.
3. Two variables are declared
and assigned values on the same
line. Then one is declared and
assigned a value on the next line.
(The third example shows two
numbers, but you can declare
variables that hold different
types of data on the same line,
e.g., a string and a number.)
4 . Here, a variable is used to
hold a reference to an element in
the HTML page. This allows you
to work directly with the element
stored in that variable. (See
more about this on p190.)
While the shorthand might save
you a little bit of typing, it can
make your code a little harder
to follow. So, when you are
starting off, you will find it easier
to spread your code over a few
more lines to make it easier to
read and understand.

## CHANGING THE VALUE OF A VARIABLE

Once you have assigned a value
to a variable, you can then
change what is stored in the
variable later in the same script.
Once the variable has been
created, you do not need to
use the var keyword to assign
it a new value. You just use the
variable name, the equals sign
(also known as the assignment
operator), and the new va lue for
that attribute.
For example, the value of a
shipping variable might start
out as being false. Then
something in the code might
change the ability to ship the
item and you could therefore
change the value to true.
In t his code example, the values
of the two variables are both
swapped from being true to
false and vice versa.


# Logical operators 
Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value. However, the && and || operators actually return the value of one of the specified operands, so if these operators are used with non-Boolean values, they may return a non-Boolean value. The logical operators are described in the following table.

## USING LOGICAL AND
In this example, a math test
has tworounds.Foreach round
there are two variables: one
holds the user's score for that
round; the other holds the pass
mark for that round.
The logical AND is used to see
if the user's score is greater
than or equal to the pass mark
in both of the rounds of the test.
The result is stored in a variable
called passBoth.


## USING LOGICAL OR
& LOGICAL NOT
Here is the same test but this
time using the logical OR operator
to find out if the user has passed
at least one of the two rounds.
If they pass just one round, they
do not need to retake the test.




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

