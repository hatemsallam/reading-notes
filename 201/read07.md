# Domain Modeling

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

## Summary
Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

Here's some tips to follow when building your own domain models.

- When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
- Model its attributes with a constructor function that defines and initializes properties.
- Model its behaviors with small methods that focus on doing one job well.
- Create instances using the new keyword followed by a call to a constructor function.
- Store the newly created object in a variable so you can access its properties and methods from outside.
- Use the this variable within methods so you can access the object's properties and methods from inside.


# Tables 

A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.


## Basic Table Structure

table tag
The table tag element is used
to create a table. The contents
of the table are written out row
by row.

tr tag
You indicate the start of each
row using the opening tr tag.
(The tr stands for table row.)
It is followed by one or more elements (one for each cell
in that row).

td tag 
At the end of the row you use a
closing td tag.

Each cell of a table is
represented using a td tag
element. (The td stands for
table data.)
At the end of each cell you use a
closing td tag.

## Summary
- The table tag element is used to add tables to a web
page.
- A table is drawn out row by row. Each row is created
with the tr tag element.
- Inside each row there are a number of cells
represented by the td tag element (or th tag if it is a
header).
- You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.
- For long tables you can split the table into a thead tag,
tbody tag, and tfoot tag.


# creating objects

## CREATING OBJECTS USING CONSTRUCTOR SYNTAX

an empty object
called hote 1 is created using the
constructor function.
Once it has been created, three
properties and a method are
then assigned to the object.
( If the object already had any
of these properties, this would
overwrite the values in those
properties.)
To access a property of this
object, you can use dot notation,
just as you can with any object.
For example, to get the hotel's
name you could use:
hotel .name
Similarly, to use the method,
you can use the object name
followed by the method name:
hotel.checkAvailability()


- var hotel = new Object();
- hotel.name= 'Park';
- hotel.rooms = 120;
- hotel .booked = 77;
- hotel .checkAvailability = function()
- return this . rooms - this.booked;
- } ;
- var elName = document.getElementByid('hotelName');
- elName.textContent = hotel . name;
- var elRooms = document .getElementByid('rooms');
- elRooms .textContent = hotel .checkAvailability(};


## ADDING AND REMOVING PROPERTIES


Once you have created an object
(using literal or constructor
notation), you can add new
properties to it.
You do this using the dot
notation that you saw for adding
properties to objects on pl03.
In this example, you can see that
an instance of the hotel object
is created using an object literal.
Immediately after t his, the
hotel object is given two
extra properties that show the
facilities (whether or not it has
a gym and/or a pool). These
properties are given values that
are Booleans (true or false).
Having added these properties
to the object, you can access
them just like any of the objects
other properties. Here, they
update the value of the cl ass
attribute on their respective
elements to show either a check
mark or a cross mark.
To delete a property, you use
the keyword delete, and then
use dot notation to identify the
property or method you want to
remove from the object.
In this case, the booked property
is removed from the object.

- var hotel = {
- name : 'Park' ,
- rooms : 120,
- booked : 77.
- } ;
- hotel .gym = t rue;
- hotel .pool = fal se;
- delete hotel .booked;
- var elName = document .getEl ementByld('hotelName ' );
- elName.textContent = hotel . name;
- var el Pool = document .getElementByid ('pool ') ;
- elPool.cl assName = ' Pool: ' + hotel. pool ;
- var elGym = document .getEl ementByld('gym ' };
- elGym.className = 'Gym: ' + hotel .gym;


## BUILT-IN OBJECTS

Browsers come with a set of built-in objects that represent things like the
browser window and the current web page shown in that window. These
built-in objects act like a toolkit for creating interactive web pages.


## GLOBAL OBJECTS:NUMBER OBJECT

Whenever you have a value that is a number,
you can use the methods and properties of the
Number object on it.

These methods are helpful
when dealing with a range of
applications from financial
calculations to animations.

Many calculations involving
currency (such as tax rates) will
need to be rounded to a specific
number of decimal places.

Or, in an animation, you might
want to specify that certain
elements. should be evenly
spaced out across the page.


## Summary
- functions allow you to group a set of related
statements together that represent a single task.
- Functions can take parameters (informatiorJ required
to do their job) and may return a value.
- An object is a series of variables and functions that
represent something from the world around you.
- In an object, variables are known as properties of the
object; functions are known as methods of the object.
- Web browsers implement objects that represent both
the browser window and the document loaded into the
browser window.
- JavaScript also has several built-in objects such as
- String, Number, Math, and Date. Their properties and
methods offer functionality that help you write scripts.
- Arrays and objects can be used to create complex data
sets (and both can contain the other).




