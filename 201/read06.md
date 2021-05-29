# WHAT IS AN OBJECT?

Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.


## IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES
If a variable is part of an object, it is called a
property. Properties te ll us about the object, such as
the name of a hotel or the number of rooms it has.
Each individual hotel might have a different name
and a different number of rooms.

## IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS
If a function is part of an object, it is called a method.
Methods represent tasks that are associated with
the object. For example, you can check how many
rooms are available by subtracting the number of
booked rooms from the total number of rooms.

# Document object model

The Document Object Model (DOM) specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.

## MAKING A MODEL OF THE HTML PAGE
When the browser loads a web page, it
creates a model of the page in memory.
The DOM specifies the way in which the
browser should structure this model using
a DOM tree.
The DOM is called an object model
because the model (the DOM tree) is
made of objects.
Each object represents a different part of
the page loaded in the browser window.

## ACCESSING AND CHANGING THE HTML PAGE
The DOM also defines methods and
properties to access and update each
object in this model, which in turn updates
what the user sees in the browser.
You will hear people call the DOM an
Application Programming Interface (API).
User interfaces let humans interact with
programs; APls let programs (and scripts)
talk to each other. The DOM states what
your script can "ask the browser about the
current page, and how to tell the browser
to update what is being shown to the user.

# THE DOM TREE IS A MODEL OF A WEB PAGE
As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
It consists of four main types of nodes.

## THE DOCUMENT NODE
Above, you can see the HTML code for a shopping
list, and on the right hand page is its DOM tree.
Every element, attribute, and piece of text in the
HTML is represented by its own DOM node.
At the top of the tree a document node is added; it
represents the entire page (and also corresponds to
the document object, which you first met on p36).
When you access any element, attribute, or text
node, you navigate to it via the document node. It is
the starting point for all visits to the DOM tree.

## ELEMENT NODES
HTML elements describe the structure of an HTML
page. (The h1   - h6) elements describe what
parts are headings; the p tags indicate where
paragraphs of text start and finish; and so on.)
To access the DOM tree, you start by looking for
elements. Once you find the element you want, then
you can access its text and attribute nodes if you
want to. This is why you start by learning methods
that allow you to access element nodes, before
learning to access and alter text or attributes

## WORKING WITH THE DOM TREE

- STEP 1: ACCESS THE ELEMENTS
- STEP 2: WORK WITH THOSE ELEMENTS

## ACCESSING ELEMENTS
DOM queries may return one element, or they may return a Nodelist,
which is a collection of nodes.

### GROUPS OF ELEMENT NODES
If a method can return more than one node, it will
always return a Nodelist, which is a collection of
nodes (even if it only finds one matching element).
You then need to select the element you want from
this list using an index number (which means the
numbering starts at 0 like the items in an array).
For example, several elements can have the same
tag name, so get El ementsByTagName () will always
return a Nodel i st.

### FASTEST ROUTE
Finding the quickest way to access an element
within your web page will make the page seem
faster and/or more responsive. This usually means
evaluating the minimum number of nodes on the
way to the element you want to work with. For
example, getEl ementByld () will quickly return one
element (because no two elements on the same
page should have the same value for an id attribute),
but it can only be used when the element you want
to access has an id attribute.

# looping through a nodelist play by play
## TRAVERSING THE DOM
When you have an element node, you can select
another element in relation to it using these five
properties. This is known as traversing the DOM.

## whitespace nodes
Traversing the DOM can be difficult because
some browsers add a text node whenever they
come across whitespace between elements.


## HOW TO GET/UPDATE ELEMENT CONTENT
So far this chapter has focused on finding elements in the DOM tree.
The rest of this chapter shows how to access/update element content.
Your choice of techniques depends upon what the element contains.

# adding or removing html content
## ACCESS & UPDATE TEXT & MARKUP WITH INNERHTML

Using the i nnerHTML property, you can access
and amend the contents of an element,
including any child elements.
innerHTML
When getting HTML from an
element, the inner HTML property
will get the content of an
element and return it as one long
string, including any markup that
the element contains.
When used to set new content
for an element, it will take a
string that can contain markup
and process that string, adding
any elements within it to the
DOM tree.
When adding new content using
i nnerHTML, be aware that one
missing closing tag could throw
out the design of the entire page.
Even worse, if i nnerHTML is used
to add content that your users
created to a page, they could add
malicious content.

## UPDATE TEXT & MARKUP
As the content of the string
is added to the element using
the i nnerHTML property, the
browser will add any elements
in the string to the DOM. In
this example, an a tag element
has been added to the page.
(Any new elements will also be
available to other scripts in the
page.)
If you use attributes in your
HTML code, escaping the
quotation using the backslash
character \ can make it clearer
that those characters are not
part of the script.
DOCUMENT.

## COMPARING TECHNIQUES:UPDATING HTML CONTENT
So far, you have seen three techniques for adding HTML to a web page.
It's time to compare when you should use each one.

In any programming language, there are often
several ways to achieve the same task. In fact, if you
asked ten programmers to write the same script, you
may well find ten different approaches.
Some programmers can be rather opinionated and
believe that their way is always the "right" way to do
things - when there are often several right ways. If
you understand why people prefer some approaches
over others, then you are in a strong position to
decide whether it meets the needs of your project.

## CROSS-SITE SCRIPTING\ (XSS) ATTACKS
If you add HTML to a page using i nnerHTML (or several jQuery methods),
you need to be aware of Cross-Site Scripting Attacks or XSS; otherwise,
an attacker could gain access to your users' accounts.

## XSS: VALIDATION & TEMPLATES
Make sure that your users can only input characters they need to use
and limit where this content will be shown on the page.

FILTER OR VALIDATE INPUT
The most basic defense is to prevent users from
entering characters into form fields that they do not
need to use when providing that kind of information.
For example, users' names and email addresses
will not contain angled brackets, ampersands, or
parentheses, so you can validate data to prevent
characters like this being used.
This can be done in the browser, but must also be
done on the server (in case the user has JavaScript
turned off). You learn about validation in Chapter 13.

LIMIT WHERE USER CONTENT GOES
Malicious users will not just use script tags to
try and create an XSS attack. As you saw on p228,
malicious code can live in an event handler attribute
without being wrapped in script tags. XSS can
also be triggered by malicious code in CSS or URLs.
Browsers process HTML, CSS, and JavaScript in
different ways (or execution contexts), and in each
language different characters can cause problems.
Therefore, you should only add content from
untrusted sources as text (not markup), and place
that text in elem·ents that are visible in the viewport.


## XSS: ESCAPING & CONTROLLING MARKUP

Any content generated by users that contain characters that are used
in code should be escaped on the server. You must control any markup
added to the page.


# attribute nodes
## CHECK FOR AN ATTRIBUTE AND GET ITS VALUES

Before you work with an
attribute, it is good practice to
check whether it exists. This will
save resources if the attribute
cannot be found.

The hasAttri bute() method
of any element node lets you
check if an attribute exists. The
attribute name is given as an
argument in the parentheses.

Using hasAttribute() in an if
statement like this means that
the code inside the curly braces
will run only if the attribute
exists on the given element.


## CREATING ATTRIBUTES & CHANGING THEIR VALUES


The className property allows
you to change the value of the
class attribute. If the attribute
does not exist, it will be created
and given the specified value.

You have seen this property
used throughout the chapter
to update the status of the
list items. Below, you can see
another way to achieve the task.


The setAttribute() method
allows you to update the va lue
of any attribute. It takes two
parameters: the attribute name,
and the value for the attribute.


## EXAMINING THE DOM IN CHROME

Modern browsers come with tools that help
you inspect the page loaded in the browser
and understand the structure of the DOM tree.



In the screenshot to the right, the
li tag element is highlighted and
the Properties panel (1) indicates
that this is an:
- 1 i element with an id
attribute whose value is one
and cl ass whose value is hot
- an HTMLLIElement
- an HTMLElement
- an element
- a node
- an object


# summary
- The browser represents the page using a DOM tree.
- DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes.
- You can select element nodes by their id or cl ass
attributes, by tag name, or using CSS selector syntax.
- Whenever a DOM query can return more than one
node, it will always return a Nadel i st.
- From an element node, you can access and update its
content using properties such as textContent and
innerHTML or using DOM manipulation techniques.
- An element node can contain multiple text nodes and
child elements that are siblings of each other.
- In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
- Browsers offer tools for viewing the DOM tree .