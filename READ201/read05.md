
<!-- From the Duckett HTML book:

Chapter 5: “Images” (pp.94-125)
Chapter 11: “Color” (pp.246-263)
Chapter 12: “Text” (pp.264-299) -->

# chapter 5 Images
#### How to add images to pages
 #### Choosing the right format
#### Optimizing images for the web

There are several things to consider when selecting and
preparing images for your site, but taking time to get them
right will make it look more attractive and professional.
In this chapter you will learn how to:
* Include an image in your web pages using HTML *
* Pick which image format to use *
* Show an image at the right size *
* Optimize an image for use on the web to make pages *
* load faster *


#### Choosing Images for Your Site
A picture can say a thousand words, and great
images help make the difference between an
average-looking site and a really engaging one.

Images can be used to set the
tone for a site in less time than
it takes to read a description. If
you do not have photographs
to use on your website, there
are companies who sell stock
images; these are images you
pay to use (there is a list of stock
photography websites below).
Remember that all images are
subject to copyright, and you
can get in trouble for simply
taking photographs from
another website.


##### Images should...
Be relevant
Convey information
Convey the right mood
Be instantly recognisable
Fit the color palette

##### Online extra
We have provided an online
gallery that helps you choose the
right image for your website. You
can find it in the tools section of
the site accompanying this book


### Storing Images on Your Site

If you are building a site from scratch, it is good
practice to create a folder for all of the images
the site uses.

As a website grows, keeping
images in a separate folder
helps you understand how the
site is organized. Here you can
see an example of the files for
a website; all of the images are
stored in a folder called` images`.
On a big site you might like to
add subfolders inside the images
folder. For example, images such
as logos and buttons might sit in
a folder called `interface,` product
photographs might sit in a page
called` products `, and images
related to news might live in a
folder called news.
If you are using a content
management system or blogging
platform, there are usually tools
built into the admin site that
allow you to upload images,
and the program will probably
already have a separate folder
for image files and any
other uploads

## Adding Images

To add an image into the page
you need to use an `<img>`
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:


### Height & Width of Images

You will also often see an` <img>`
element use two other attributes
that specify its size:
###### height
This specifies the height of the
image in pixels.
######  width
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

#### Where to Place Images in Your Code

Where an image is placed
in the code will affect how it
is displayed. Here are three
examples of image placement
that produce different results:
1: before a paragraph
The paragraph starts on a new
line after the image.
2: inside the start of a
paragraph The first row of text aligns with
the bottom of the image.
3: in the middle of a
paragraph The image is placed between the
words of the paragraph



##### Three Rules for Creating Images
There are three rules to remember when you
are creating images for your website which are
summarized below. We go into greater detail
on each topic over the next nine pages.


1) Save images in the right format
2) Save images at the right size
3) Use the correc resolution


#### Tools to Edit & Save Images
There are several tools you can use to edit and
save images to ensure that they are the right
size, format, and resolution.
The most popular tool amongst
web professionals is Adobe
Photoshop. (In fact, professional
web designers often use this
software to design entire sites.)
The full version of Photoshop is
expensive, but there is a cheaper
version called Photoshop
Elements which would suit the
needs of most beginners

#### Image Dimensions
The images you use on your website should be
saved at the same width and height that you
want them to appear on the page.

#### Cropping Images 
When cropping images it is important not to
lose valuable information. It is best to source
images that are the correct shape if possible.

##### Image Resolution
Images created for the web should be saved at
a resolution of 72 ppi. The higher the resolution
of the image, the larger the size of the file.

JPGs, GIFs, and PNGs belong to
a type of image format known
as bitmap. They are made up of
lots of miniature squares. The
resolution of an image is the
number of squares that fit within
a 1 inch x 1 inch square area.

#### Vector Images

Vector images differ from bitmap images and
are resolution-independent. Vector images are
commonly created in programs such as Adobe
Illustrator.

#### Animated GIFs
Animated GIFs show several frames of an
image in sequence and therefore can be used to
create simple animations.

#### Transparency
Creating an image that is partially transparent
(or "see-through") for the web involves
selecting one of two formats:

**Transparent GIF** If the transparent part of the
image has straight edges and
it is 100% transparent (that is,
not semi-opaque), you can save
the image as a GIF (with the
transparency option selected).


##### Examining Images on the Web
Checking the Si ze of Images
If you are updating a website, you might need to check the size of an
existing image before creating a new one to replace it. This can be
achieved by right-clicking on the image and making a selection from
the pop-up menu that appears. (Mac users will need to hold down the
control key and click rather than right-click.)


#### Downloading Images
If you want to download images from a website, you can do so by
accessing the same pop-up menu. (Please remember however that all
images online are subject to copyright and require explicit permission to
reuse.)



HTML 5: Figure and Figure Caption
Images often come with
captions. HTML5 has introduced
a new `<figure> `element to
contain images and their caption
so that the two are associated.
You can have more than one
image inside the `<figure>`
element as long as they all share
the same caption.

The `<figcaption> `element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.
Before these elements were
created there was no way to
associate an` <img> `element with
its caption.



## SUMMARY 
The` <img> `element is used to add images to a
web page.
You must always specify a src attribute to indicate the
source of an image and an alt attribute to describe the
content of an image.
 You should save images at the size you will be using
them on the web page and in the appropriate format.
 Photographs are best saved as JPEGs; illustrations or
logos that use flat colors are better saved as GIFs.



# CHAPTER 11 COLOR 
 How to specify colors.
 Color terminology and contrast.
 Background color.


`Color can really bring your pages to life.`
In this chapter we will look at:
How to specify colors, as there are three common ways in
which you can indicate your choice of colors (plus extra
ways made available in CSS3)
Color terminology, as there are some terms that are very
helpful to understand when it comes to picking colors
 Contrast, and ensuring that your text is readable
 Background colors for behind either your entire page or
parts of a page
What you will learn about colors in this chapter will then be
used in subsequent chapters when it comes to looking at
colors of text and boxes in CSS.


#### Foreground Color

The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:
*rgb values*
These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)
*hex codes*
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80
*color names*
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan
We look at these three different
ways of specifying colors on the
next double-page spread.

#### Background Color
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
the` <body> `element.

### Understanding Color
Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color you want, you can use a color picker.
Computer monitors are made
up of thousands of tiny squares
called pixels (if you look very
closely at your monitor you
should be able to see them).
When the screen is not turned
on, it's black because it's not
emitting any light. When it's
on, each pixel can be a different
color, creating a picture.
The color of every pixel on the
screen is expressed in terms of
a mix of red, green, and blue —
just like on a television screen.

` Color picking tools are available `
` in image editing programs like `
` Photoshop and GIMP. You can `
` see the RGB values specified `
` next to the radio buttons that `
` say R, G, B. `

** RGB Values 
Values for red, green, and blue
are expressed as numbers
between 0 and 255. **

**Hex Codes
Hex values represent values
for red, green, and blue in
hexadecimal code.**

** Color Names
Colors are represented by
predefined names. However,
they are very limited in number. **



##### Contrast
When picking foreground and background
colors, it is important to ensure that there is
enough contrast for the text to be legible.


#### CSS 3: Opacity
CSS3 introduces the opacity
property which allows you to
specify the opacity of an element
and any of its child elements.
The value is a number between
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15%
opacity).

### CSS3: HSL Colors

CSS3 introduces an entirely new and intuitive
way to specify colors using hue, saturation,
and lightness values.


**hue**
Hue is the colloquial idea of
color. In HSL colors, hue is often
represented as a color circle
where the angle represents the
color, although it may also be
shown as a slider with values
from 0 to 360.

** saturation **
Saturation is the amount of
gray in a color. Saturation is
represented as a percentage.
100% is full saturation and 0%
is a shade of gray.


**lightness**
Lightness is the amount of
white (lightness) or black
(darkness) in a color. Lightness
is represented as a percentage.
0% lightness is black, 100%
lightness is white, and 50%
lightness is normal. Lightness
is sometimes referred to as
luminosity.


## CSS3: HSL & HSLA
The hsl color property has
been introduced in CSS3 as an
alternative way to specify colors.
The value of the property starts
with the letters hsl, followed
by individual values inside
parentheses for:

## Summary

Color not only brings your s XX ite to life, but also helps
convey the mood and evokes reactions.
There are three ways to specify colors in CSS:
RGB values, hex codes, and color names.
 Color pickers can help you find the color you want.
 It is important to ensure that there is enough contrast
between any text and the background color (otherwise
people will not be able to read your content).
 CSS3 has introduced an extra value for RGB colors to
indicate opacity. It is known as RGBA.
 CSS3 also allows you to specify colors as HSL values,
with an optional opacity value. It is known as HSLA.


# CHAPTER 12 TEXT 
Size and typeface of text
 Bold, italics, capitals, underlines
 Spacing between lines, words, and letters


 `The properties that allow you to control`
`the appearance of text can be split into`
`two groups:`
 1) Those that directly affect the font and its appearance
(including the typeface, whether it is regular, bold or italic,
and the size of the text)
2) Those that would have the same effect on text no matter
what font you were using (including the color of text and
the spacing between words and letters)

#### Typeface Terminology

###### Serif
 Serif fonts have extra details on
the ends of the main strokes of
the letters. These details are
known as serifs.
###### Sans-Serif
Sans-serif fonts have straight
ends to letters, and therefore
have a much cleaner design.
###### Monospace
Every letter in a monospace (or
fixed-width) font is the same
width. (Non-monospace fonts
have different widths.)

###### Weight
The font weight not only adds
emphasis but can also affect
the amount of white space and
contrast on a page.

###### Style
Italic fonts have a cursive aspect
to some of the lettering. Oblique
font styles take the normal style
and put it on an angle.

###### Stretch
In condensed (or narrow)
versions of the font, letters are
thinner and closer together.
In expanded versions they are
thicker and further apart.



### Choosing a Typeface for your Website
When choosing
a typeface, it
is important to
understand that a
browser will usually
only display it if it's
installed on that
user's computer.

######  Monospace
Every letter in a monospace
typeface is the same width.
(Non-monospace fonts have
different widths.)
###### Cursive
Cursive fonts either have
joining strokes or other cursive
characteristics, such as
handwriting styles.
###### Fantasy
Fantasy fonts are usually
decorative fonts and are often
used for titles. They're not
designed for long bodies of text.




### Techniques That Offer a Wider Choice of Typefaces
font-family : 
font-face : 
Service-based Font-Face:

#### Specifying Typefaces

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


#### Size of Type
font-size
The font-size property enables
you to specify a size for the
font. There are several ways to
specify the size of a font. The
most common are:
**pixels**
Pixels are commonly used
because they allow web
designers very precise control
over how much space their text
takes up. The number of pixels is
followed by the letters px.
**percentages**
The default size of text in
browsers is 16px. So a size of
75% would be the equivalent of
12px, and 200% would be 32px.
**ems**
An em is equivalent to the width
of a letter m.
We will look at these
measurements in greater detail
on the next page.

## Type Scales
You may have noticed that programs such as
Word, Photoshop and InDesign offer the same
sizes of text.

** Units of Type Size ** 
*Pixels*
*Percentages*
*Ems*

### More Font Choice
@font-face allows you to use
a font, even if it is not installed
on the computer of the person
browsing, by allowing you to
specify a path to a copy of the
font, which will be downloaded if
it is not on the user's machine.

#### Underst anding Font Formats

Different browsers support
different formats for fonts
(in the same way that they
support different audio and
video formats), so you will need
to supply the font in several
variations to reach all browsers.
If you do not have all of these
formats for your font, you can
upload the font to a website
called FontSquirrel where they
will convert it for you:

#### Bold
The font-weight property
allows you to create bold text.
There are two values that this
property commonly takes:
normal This causes text to appear at a
normal weight.
bold This causes text to appear bold.
In this example, you can see
that the element whose class
attribute has a value of credits
has been bolded.


### UpperCase & LowerCase

The text-transform property
is used to change the case of
text giving it one of the following
values:
uppercase
This causes the text to appear
uppercase.
lowercase
This causes the text to appear
lowercase.
capitalize
This causes the first letter of
each word to appear capitalized.


#### Underline & Strike

The text-decoration property
allows you to specify the
following values:
none
This removes any decoration
already applied to the text.
underline
This adds a line underneath the
text.
overline
This adds a line over the top of
the text.
line-through
This adds a line through words.
blink
This animates the text to make it
flash on and off (however this is
generally frowned upon, as it is
considered rather annoying).


#### Leading

Leading (pronounced ledding) is
a term typographers use for the
vertical space between lines of
text. In a typeface, the part of
a letter that drops beneath the
baseline is called a descender,
while the highest point of a letter
is called the ascender.



#### Lett er & Word Spacing
Kerning is the term
typographers use for the space
between each letter. You can
control the space between each
letter with the letter-spacing
property.
It is particularly helpful to
increase the kerning when
your heading or sentence is
all in uppercase. If your text is
in sentence (or normal) case,
increasing or decreasing the
kerning can make it harder to
read.
You can also control the gap
between words using the
word-spacing property.


#### Alignment

The text-align property allows
you to control the alignment of
text. The property can take one
of four values:
left :
This indicates that the text
should be left-aligned.
right :
This indicates that the text
should be right-aligned.
center : 
This allows you to center text.
justify :
This indicates that every line in
a paragraph, except the last line,
should be set to take up the full
width of the containing box.

#### Vertical Alignment
The vertical-align property is
a common source of confusion.
It is not intended to allow you to
vertically align text in the middle
of block level elements such as
`<p> `and` <div>`, although it does
have this effect when used with
table cells (the `<td> `and `<th>`
elements).


#### Indenting Text

The text-indent property
allows you to indent the first
line of text within an element.
The amount you want the line
indented by can be specified in
a number of ways but is usually
given in pixels or ems.
It can take a negative value,
which means it can be used
to push text off the browser
window. You can see this
technique used in this example,
where the `<h1>` element uses a
background image to represent
the heading.



#### CSS3: Drop Shadow
The text-shadow property has
become commonly used despite
lacking support in all browsers.
It is used to create a drop
shadow, which is a dark version
of the word just behind it and
slightly offset. It can also be used
to create an embossed effect by
adding a shadow that is slightly
lighter than the text.


### First Lett er or Line
You can specify different values
for the first letter or first line of
text inside an element using
:first-letter and
:first-line.

#### Styling Links

Browsers tend to show links
in blue with an underline by
default, and they will change
the color of links that have been
visited to help users know which
pages they have been to.
In CSS, there are two pseudoclasses
that allow you to set
different styles for links that
have and have not yet been
visited.
link :
This allows you to set styles
for links that have not yet been
visited.
visited :
This allows you to set styles for
links that have been clicked on.


#### Responding to Us ers
There are three pseudo-classes
that allow you to change the
appearance of elements when a
user is interacting with them.

** hover, active, focus ** 


#### Att ribute Selectors
You met the most popular CSS selectors on page 238. There are also
a set of attribute selectors that allow you to create rules that apply to
elements that have an attribute with a specific value.


## Summary

There are properties to control t XX he choice of font, size,
weight, style, and spacing.
There is a limited choice of fonts that you can assume
most people will have installed.
If you want to use a wider range of typefaces there are
several options, but you need to have the right license
to use them.
You can control the space between lines of text,
individual letters, and words. Text can also be aligned
to the left, right, center, or justified. It can also be
indented.
You can use pseudo-classes to change the style of an
element when a user hovers over or clicks on text, or
when they have visited a link.












