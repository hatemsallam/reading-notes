# Images

## how to choose images
Images should be :
- Be relevant
- Convey information
- Convey the right mood
- Be instantly recognisable
- Fit the color palette

## Adding Images

To add an image into the page
you need to use an img tag
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:
src
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site. (Here you can see that
the images are in a child folder
called images — relative URLs
were covered on pages 83-84).
alt
This provides a text description
of the image which describes the
image if you cannot see it.
title
You can also use the title
attribute with the img tag element
to provide additional information
about the image. Most browsers
will display the content of this
attribute in a tootip when the
user hovers over the image.

## Height & Width of Images
- height
This specifies the height of the
image in pixels.
- width
This specifies the width of the
image in pixels.
Images often take longer to
load than the HTML code that
makes up the rest of the page.
It is, therefore, a good idea to
specify the size of the image
so that the browser can render
the rest of the text on the page
while leaving the right amount of
space for the image that is still
loading.

## Three Rules for Creating Images

- Save images in the right format:
Websites mainly use images in
jpeg, gif, or png format. If you
choose the wrong image
format then your image might
not look as sharp as it should
and can make the web page
slower to load.

- Save images at the right size:
You should save the image at
the same width and height it will
appear on the website. If
the image is smaller than the
width or height that you have
specified, the image can be
distorted and stretched. If the
image is larger than the width
and height if you have specified,
the image will take longer to
display on the page.

- Use the correct resolution:
Computer screens are made up
of dots known as pixels. Images
used on the web are also made
up of tiny dots. Resolution refers
to the number of dots per inch,
and most computer screens only
show web pages at 72 pixels
per inch. So saving images at
a higher resolution results in
images that are larger than
necessary and take longer to
download.

## Summary
- The (img) tag element is used to add images to a
web page.
- You must always specify a src attribute to indicate the
source of an image and an alt attribute to describe the
content of an image.
- You should save images at the size you will be using
them on the web page and in the appropriate format.
- Photographs are best saved as JPEGs; illustrations or
logos that use flat colors are better saved as GIFs.

# Color
## Foreground Color
The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:
- rgb values
These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)
- hex codes
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80
- color names
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan
We look at these three different
ways of specifying colors on the
next double-page spread.

## Background Color
CSS treats each HTML element
as if it appears in a box, and the
background-color property
sets the color of the background
for that box.
You can specify your choice of
background color in the same
three ways you can specify
foreground colors: RGB values,
hex codes, and color names
(covered on the next page).
If you do not specify a
background color, then the
background is transparent.
By default, most browser
windows have a white
background, but browser users
can set a background color for
their windows, so if you want
to be sure that the background
is white you can use the
background-color property on
the body tag element.

## Summary
Color not only brings your site to life, but also helps
convey the mood and evokes reactions.
- There are three ways to specify colors in CSS:
RGB values, hex codes, and color names.
- Color pickers can help you find the color you want.
- It is important to ensure that there is enough contrast
between any text and the background color (otherwise
people will not be able to read your content).
- CSS3 has introduced an extra value for RGB colors to
indicate opacity. It is known as RGBA.
- CSS3 also allows you to specify colors as HSL values,
with an optional opacity value. It is known as HSLA.

# Text

## Choosing a Typeface for your Website

When choosing
a typeface, it
is important to
understand that a
browser will usually
only display it if it's
installed on that
user's computer.

## Techniques That Offera Wider Choice of Typefaces
- font-family : The user's computer needs the
typeface installed. CSS is used to
specify the typeface.
- font-face : CSS specifies where a font can
be downloaded from if it is not
installed on the computer.
- Service-based : Commercial services give users
access to a wider range of fonts
using @font-face.
Font-Face


## Specifying Typefaces
font-family

The font-family property
allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.
The value of this property is the
name of the typeface you want
to use.
The people who are visiting
your site need the typeface you
have specified installed on their
computer in order for it to be
displayed.
You can specify a list of fonts
separated by commas so that,
if the user does not have your
first choice of typeface installed,
the browser can try to use an
alternative font from the list.
It is also common to end with a
generic font name for that type
of font 
If a font name is made up of
more than one word, it should be
put in double quotes.
Designers suggest pages usually
look better if they use no more
than three typefaces on a page.

## Size of Type
font-size
 - The font-size property enables
you to specify a size for the
font. There are several ways to
specify the size of a font. The
most common are:
- pixels
Pixels are commonly used
because they allow web
designers very precise control
over how much space their text
takes up. The number of pixels is
followed by the letters px.
- percentages
The default size of text in
browsers is 16px. So a size of
75% would be the equivalent of
12px, and 200% would be 32px.
If you create a rule to make all
text inside the body tag element
to be 75% of the default size (to
make it 12px), and then specify
another rule that indicates the
content of an element inside the
body tag element should be 75%
size, it will be 9px (75% of the
12px font size).
ems
An em is equivalent to the width
of a letter m.

## UpperCase & LowerCase
The text-transform property
is used to change the case of
text giving it one of the following
values:
- uppercase
This causes the text to appear
uppercase.
- lowercase
This causes the text to appear
lowercase.
- capitalize
This causes the first letter of
each word to appear capitalized.
In this example, the h1 tag
element is uppercase, the h2 tag
element is lowercase, and the
credits are capitalized. In the
HTML, the word by in the credits
had a lowercase b.

## Summary
TEXT
 - There are properties to control the choice of font, size,
weight, style, and spacing.
- There is a limited choice of fonts that you can assume
most people will have installed.
-  If you want to use a wider range of typefaces there are
several options, but you need to have the right license
to use them.
- You can control the space between lines of text,
individual letters, and words. Text can also be aligned
to the left, right, center, or justified. It can also be
indented.
- You can use pseudo-classes to change the style of an
element when a user hovers over or clicks on text, or
when they have visited a link.