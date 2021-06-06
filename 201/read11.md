# Images

## Controlling sizes of images in CSS

You can control the size of an
image using the width and
height properties in CSS, just
like you can for any other box.
Specifying image sizes helps
pages to load more smoothly
because the HTML and CSS
code will often load before the
images, and telling the browser
how much space to leave for an
image allows it to render the rest
of the page without waiting for
the image to download.
You might think that your site
is likely to have images of all
different sizes, but a lot of sites
use the same sized image across
many of their pages.
For example, an e-commerce site
tends to show product photos
at the same size. Or, if your site
is designed on a grid, then you
might have a selection of image
sizes that are commonly used on
all pages, such as:
Small portrait: 220 x 360
Small landscape: 330 x 210
Feature photo: 620 x 400
Whenever you use consistently
sized images across a site,
you can use CSS to control
the dimensions of the
images, instead of putting the
dimensions in the HTML.

img.large {
width: 500px;
height: 500px;}
img.medium {
width: 250px;
height: 250px;}
img.small {
width: 100px;
height: 100px;}


## Aligning images using CSS

In the last chapter, you saw how
the float property can be used
to move an element to the left or
the right of its containing block,
allowing text to flow around it.
Rather than using the img tag
element's align attribute, web
page authors are increasingly
using the float property to align
images. There are two ways that
this is commonly achieved:
1: The float property is added
to the class that was created to
represent the size of the image
(such as the small class in our
example).
2: New classes are created with
names such as align-left or
align-right to align the images
to the left or right of the page.
These class names are used in
addition to classes that indicate
the size of the image.
In this example you can see the
align-left and align-right
classes used to align the image.
It is also common to add a
margin to the image to ensure
that the text does not touch their
edges.

img.align-left {
float: left;
margin-right: 10px;}
img.align-right {
float: right;
margin-left: 10px;}
img.medium {
width: 250px;
height: 250px;}


## Background Images

The background-image
property allows you to place
an image behind any HTML
element. This could be the entire
page or just part of the page. By
default, a background image will
repeat to fill the entire box.
The path to the image follows
the letters url, and it is put
inside parentheses and quotes.
Here is the image
tile used in this
example.
In the first example, you can
see a background image being
applied to an entire page
(because the CSS selector
applies to the body element).
In the second example, the
background image just applies to
a paragraph.
If you search online, you will
find lots of resources that offer
background textures that you
can use on your pages.


## summary
- You can specify the dimensions o XX f images using CSS.
This is very helpful when you use the same sized
images on several pages of your site.
- Images can be aligned both horizontally and vertically
using CSS.
- You can use a background image behind the box
created by any element on a page.
- Background images can appear just once or be
repeated across the background of the box.
- You can create image rollover effects by moving the
background position of an image.
- To reduce the number of images your browser has to
load, you can create image sprites









# Practical Information


## Search Engine Optimization (SEO )

SEO is a huge topic and several books have been written on the subject.
The following pages will help you understand the key concepts so you can
improve your website's visibility on search engines.


## On-Page SEO
 1. Page Title
The page title appears at the top
of the browser window or on the
tab of a browser. It is specified in
the title element which lives
inside the head element.
2. URL / Web Address
The name of the file is part of
the URL. Where possible, use
keywords in the file name.
3. Headings
If the keywords are in a heading
hn element then a search
engine will know that this page is
all about that subject and give it
greater weight than other text.
4. Text
Where possible, it helps to
repeat the keywords in the main
body of the text at least 2-3
times. Do not, however, over-use
these terms, because the text
must be easy for a human to
read.
5. Link Text
Use keywords in the text that
create links between pages.

6. Image Alt Text
Search engines rely on you
providing accurate descriptions
of images in the alt text. This
will also help your images show
up in the results of image-based
searches.

7. Page Descriptions
The description also lives inside
the head element and is
specified using a meta tag.
It should be a sentence that
describes the content of the
page. (These are not shown in
the browser window but they
may be displayed in the results
pages of search engines.)

## Analytics: Learning about your Visitors

As soon as people start coming to your site, you can start analyzing
how they found it, what they were looking at and at what point they are
leaving. One of the best tools for doing this is a free service offered by
Google called Google Analytics.

- Signing Up
The Google Analytics service
relies on you signing up for an
account at:
www.google.com/analytics
The site will give you a piece of
tracking code which you need to
put on every page of your site.


- How it Works
Every time someone loads a
page of your site, the tracking
code sends data to the Google
servers where it is stored.
Google then provides a webbased
interface that allows you
to see how visitors use your site.


- The Tracking Code
A tracking code is provided
by Google Analytics for each
website you are tracking. It
should appear just before the
closing head tag. The code
does not alter the appearance of
your web pages.



## What Are Your Visitors Looking At?


The content link on the left-hand side allows
you to learn more about what the visitors are
looking at when they come to your site.

- Pages
This tells you which pages your
visitors are looking at the most
and also which pages they are
spending the most time on.

- Landing Pages
These are the pages that people
arrive on when first visiting your
site. This can be particularly
helpful because you may find
people are not always coming
into your site via the homepage.

- Top Exit Pages
This shows which pages people
most commonly leave from. If
a lot of people are leaving from
the same page then you might
consider changing that page or
improving it.

- Bounce Rate
This shows the number of people
who left on the same page that
they arrived on. A high bounce
rate suggests that the content is
not what they were looking for or
that the page did not sufficiently
encourage them to look around
the rest of the site.



## Summary
- Search engine optimization h XX elps visitors find your
sites when using search engines.
- Analytics tools such as Google Analytics allow you to
see how many people visit your site, how they find it,
and what they do when they get there.
- To put your site on the web, you will need to obtain a
domain name and web hosting.
- FTP programs allow you to transfer files from your
local computer to your web server.
- Many companies provide platforms for blogging, email
newsletters, e-commerce and other popular website
tools (to save you writing them from scratch).