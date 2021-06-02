# Forms

The most famous example about forms is the google the search box in the middle of google's home page.

## Form Controls
There are several types of form controls that
you can use to collect information from visitors
to your site.

- ADDING TEXT
- Making Choices
- Submitting Forms
- Uploading Files:


## Form Structure

- Form tag
Form controls live inside a
form element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.
- action
Every form element requires
an action attribute. Its value
is the URL for the page on the
server that will receive the
information in the form when it
is submitted.
- method
Forms can be sent using one of
two methods: get or post.


## Summary
- Whenever you want to c XX ollect information from
visitors you will need a form, which lives inside a
form element.
- Information from a form is sent in name/value pairs.
- Each form control is given a name, and the text the
user types in or the values of the options they select
are sent to the server.
- HTML5 introduces new form elements which make it
easier for visitors to fill in forms.



# Lists,tables and forms

## Bullet Point Styles

The list-style-type property
allows you to control the shape
or style of a bullet point (also
known as a marker).
It can be used on rules that
apply to the ol, ul, and li
elements.


## List Shorthand
As with several of the other CSS
properties, there is a property
that acts as a shorthand for list
styles. It is called list-style,
and it allows you to express
the markers' style, image and
position properties in any order.


## Table Properties
You have already met several
properties that are commonly
used with tables. Here we will
put them together in a single
example using the following:
width to set the width of the
table
padding to set the space
between the border of each table
cell and its content
text-transform to convert the
content of the table headers to
uppercase
letter-spacing, font-size
to add additional styling to the
content of the table headers
border-top, border-bottom
to set borders above and below
the table headers
text-align to align the writing
to the left of some table cells and
to the right of the others
background-color to change
the background color of the
alternating table rows
:hover to highlight a table row
when a user's mouse goes over it


## Summary
- In addition to the CSS p XX roperties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.
- List markers can be given different appearances
using the list-style-type and list-style image
properties.
- Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.
- Forms are easier to use if the form controls are
vertically aligned using CSS.
- Forms benefit from styles that make them feel more
interactive.



# Events


When you browse the web, your browser registers different
types of events. It's the browser's way of saying, "Hey, this
just happened." Your script can then respond to these events.


## Event types
### UI events
- load
- unload
- error
- resize
- scroll

### keyboard events
- keydown
- keyup
- keypress


### Mouse Events
- click
- db click
- mousedown
- mouseup
- mousemove
- mouseover
- mouseout

## HOW EVENTS TRIGGER JAVASCRIPT CODE

- Select t he element
node(s) you want the
script to respond to.

- Indicate which event on
the selected node(s) will
trigger the response.

- State the code you want
to run when the event
occurs.


## TRADITIONAL DOM EVENT HANDLERS
All modern browsers understand this way of creating an event handler,
but you can only attach one function to each event handler.


Here is the syntax to bind an event to an element using an event handler,
and to indicate which function should execute when that event fires:


element .onevent functionName


## Summary
- Events are the browser's way of indicating when
something has happened (such as when a page has
finished loading or a button has been clicked).
- Binding is the process of stating which event you are
waiting to happen, and which element you are waiting
for that event to happen upon.
- When an event occurs on an element, it can trigger a
- JavaScript function. When this function then changes
the web page in some way, it feels interactive because
it has responded to the user.
- You can use event delegation to monitor for events
that happen on all of the children of an element.
- The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events.