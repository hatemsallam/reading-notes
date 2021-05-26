# Writing Links

Links are created using the a element. Users can click on anything
between the opening a tag and the closing a tag. You specify
which page you want to link to using the href attribute.
Writing Links

 href="http://www.imdb.com">IMDB   with closing and opening (a) tags.

## Linking to Other Pages on the Same Site

When you are linking to other
pages within the same site,
you do not need to specify the
domain name in the URL. You
can use a shorthand known as a
relative URL.
If all the pages of the site are in
the same folder, then the value
of the href attribute is just the
name of the file.
If you have different pages of a
site in different folders, then you
can use a slightly more complex
syntax to indicate where the
page is in relation to the current
page.
If you look at the download
code for each chapter, you will
see that the index.html file
contains links that use relative
URLs.

## Directory Structure
On larger websites it's a good idea to organize your code by placing the
pages for each different section of the site into a new folder. Folders on a
website are sometimes referred to as directories.

 ### The root folder contains:
- A file called index.html which
is the homepage for the
entire site
- Individual folders for the
movies, music and theatre
sections of the site
### Each sub-directory contains:
- A file called index.html which
is the homepage for that
section
- A reviews page called reviews
.html
- A listings page called listings
.html (except for the DVD
section)
 ### The movies section contains:
- A folder called cinema
- A folder called DVD.

## Relative URLs
Relative URLs can be used when linking to pages within your own
website. They provide a shorthand way of telling the browser where to
find your files.

When you are linking to a page
on your own website, you do
not need to specify the domain
name. You can use relative URLs
which are a shorthand way to tell
the browser where a page is in
relation to the current page.
This is especially helpful when
creating a new website or
learning about HTML because
you can create links between
pages when they are only on
your personal computer (before
you have got a domain name and
uploaded them to the web).
Because you do not need to
repeat the domain name in each
link, they are also quicker to
write.

## Email Links
To create a link that starts up
the user's email program and
addresses an email to a specified
email address, you use the a
element. However, this time the
value of the href attribute starts
with mailto: and is followed by
the email address you want the
email to be sent to.
On the right you can see that
an email link looks just like any
other link but, when it is clicked
on, the user's email program
will open a new email message
and address it to the person
specified in the link.

## Opening Links in a New Window

target
If you want a link to open in a
new window, you can use the
target attribute on the opening
(a) tag. The value of this
attribute should be blank.
One of the most common
reasons a web page author
might want a link to be opened
in a new window is if it points to
another website. In such cases,
they hope the user will return
to the window containing their
site after finishing looking at the
other one.

## Summary
LINKS
- Links are created using the (a) tag element.
- The (a) tag element uses the href attribute to indicate
the page you are linking to.
- If you are linking to a page within your own site, it is
best to use relative links rather than qualified URLs.
- You can create links to open email programs with an
email address in the "to" field.
- You can use the id attribute to target elements within
a page that can be linked to.

# Layout

## Key Concepts in Positioning Elements

### Building Blocks
CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.
Block-level boxes start on a new line and act as the main building blocks
of any layout, while inline boxes flow between surrounding text. You can
control how much space each box takes up by setting the width of the
boxes (and sometimes the height, too). To separate boxes, you can use
borders, margins, padding, and background colors.

### Containing Elements
If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.
It is common to group a number of elements together inside a (div) tag
(or other block-level) element. For example, you might group together
all of the elements that form the header of a site (such as the logo and
the main navigation). The (div) tag element that contains this group of
elements is then referred to as the containing element.


## Controlling the Position of Elements

### Normal flow
Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
Even if you specify the width
of the boxes and there is space
for two elements to sit side-byside,
they will not appear next
to each other. This is the default
behavior (unless you tell the
browser to do something else).

### Relative Positioning
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed. This
does not affect the position of
surrounding elements; they stay
in the position they would be in
in normal flow.

### Absolute positioning
This positions the element
in relation to its containing
element. It is taken out of
normal flow, meaning that it
does not affect the position
of any surrounding elements
(as they simply ignore the
space it would have taken up).
Absolutely positioned elements
move as users scroll up and
down the page.

### Fixed Positioning
This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.
Elements with fixed positioning
do not affect the position of
surrounding elements and they
do not move when the user
scrolls up or down the page.

### Floating Elements
Floating an element allows
you to take that element out
of normal flow and position
it to the far left or right of a
containing box. The floated
element becomes a block-level
element around which other
content can flow.

## Relative Positioning
Relative positioning moves an
element in relation to where it
would have been in normal flow.
For example, you can move it 10
pixels lower than it would have
been in normal flow or 20% to
the right.
You can indicate that an element
should be relatively positioned
using the position property
with a value of relative.
You then use the offset
properties (top or bottom and
left or right) to indicate how
far to move the element from
where it would have been in
normal flow.
To move the box up or down,
you can use either the top or
bottom properties.
To move the box horizontally,
you can use either the left or
right properties.
The values of the box offset
properties are usually given in
pixels, percentages or ems.

## Absolute Positioning

When the position property
is given a value of absolute,
the box is taken out of normal
flow and no longer affects the
position of other elements on
the page. (They act like it is not
there.)
The box offset properties (top
or bottom and left or right)
specify where the element
should appear in relation to its
containing element.
In this example, the heading has
been positioned at the top of the
page and 500 pixels from its left
edge. The width of the heading is
set to be 250 pixels wide.
The width property has
also been applied to the (p) tag
elements in this example
to prevent the text from
overlapping and becoming
unreadable.

## Fixed Positioning
Fixed positioning is a type
of absolute positioning that
requires the position property
to have a value of fixed.
It positions the element in
relation to the browser window.
Therefore, when a user scrolls
down the page, it stays in the
exact same place. It is a good
idea to try this example in your
browser to see the effect.
To control where the fixed
position box appears in relation
to the browser window, the box
offset properties are used.
In this example, the heading
has been positioned to the top
left hand corner of the browser
window. When the user scrolls
down the page, the paragraphs
disappear behind the heading.
The (p) tag elements are in normal
flow and ignore the space that
the (h1) tag element would have
taken up. Therefore, the
margin-top property has
been used to push the first (p) tag
element below where the fixed
position (h1) element is sitting.

## Overlapping Elements

When you use relative, fixed, or
absolute positioning, boxes can
overlap. If boxes do overlap, the
elements that appear later in the
HTML code sit on top of those
that are earlier in the page.
If you want to control which
element sits on top, you can use
the z-index property. Its value
is a number, and the higher the
number the closer that element
is to the front. For example, an
element with a z-index of 10
will appear over the top of one
with a z-index of 5.
This example looks similar to
the one on page 368, but it
uses relative positioning for
the (p) tag elements. Because
the paragraphs are relatively
positioned, by default they
would appear over the top of the
heading as the user scrolls down
the page. To ensure that the
(h1) tag element stays on top, we
use the z-index property on the
rule for the (h1) tag element.
The z-index is sometimes
referred to as the stacking
context (as if the blocks have
been stacked on top of each
other on a z axis). If you are
familiar with desktop publishing
packages, it is the equivalent
of using the 'bring to front' and
'send to back' features.

## Floating Elements

the float property allows you
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.
Anything else that sits inside
the containing element will
flow around the element that is
floated.
When you use the float
property, you should also use the
width property to indicate how
wide the floated element should
be. If you do not, results can be
inconsistent but the box is likely
to take up the full width of the
containing element (just like it
would in normal flow).
In this example, a
blockqoute tag element is
used to hold a quotation. It's
containing element is the
body tag element.
The blockqoute tag element
is floated to the right, and the
paragraphs that follow the quote
flow around the floated element.


# Screen Sizes 

Resolution refers to the number of dots a screen shows per inch. Some
devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens.

## Page Sizes
Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens).

## Fixed Width Layouts

Fixed width layout
designs do not
change size as the
user increases
or decreases
the size of their
browser window.
Measurements tend
to be given in pixels.

## Liquid Layouts

Liquid layout designs
stretch and contract
as the user increases
or decreases the
size of their browser
window. They tend to
use percentages.

## Layout Grids

Composition in any visual art (such as design, painting, or photography)
is the placement or arrangement of visual elements — how they are
organized on a page. Many designers use a grid structure to help them
position items on a page, and the same is true for web designers.

## CSS Frameworks
CSS frameworks aim to make your life easier by providing the code for
common tasks, such as creating layout grids, styling forms, creating
printer-friendly versions of pages and so on. You can include the CSS
framework code in your projects rather than writing the CSS from scratch.

## Summary
LAYOUT
- div tag elements are often used as containing elements
to group together sections of a page.
- Browsers display pages in normal flow unless you
specify relative, absolute, or fixed positioning.
- The float property moves content to the left or right
of the page and can be used to create multi-column
layouts. (Floated items require a defined width.)
- Pages can be fixed width or liquid (stretchy) layouts.
- Designers keep pages within 960-1000 pixels wide,
and indicate what the site is about within the top 600
pixels (to demonstrate its relevance without scrolling).
- Grids help create professional and flexible designs.
- CSS Frameworks provide rules for common tasks.
- You can include multiple CSS files in one page.