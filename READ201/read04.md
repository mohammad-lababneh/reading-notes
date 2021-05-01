
<!-- Hello Mohammed ,

Please pay attention to my notes in your submissions 🙏
I want to help you to reach the full mark but I need your effort to achieve that.

Very very important note :-
 
*There's no need to create a new repo you should continue using the 102 "reading-notes" repo and just you need to add a new table to it under the 102 table with this title "code 201 Reading Notes").

You should solve this issue ASAP Mohammed 🙏.

*But, for the Reads , the second link should be the live URL of the home page not the link of the repo (For the labs just we put the repo link).

And , Well done Mohammad your read is very good 👍
you covered everything which is great.

*Just please try to add (images/lists/etc) to empower your read. 

So, I'm looking forward to your resubmission Mohammad.
please do it ASAP and let me know when you are done with it.

Wish you the best of luck. -->

# HTML
## chapter 4 links 

 ##### creating inks between pages
 ##### Linking to other sites 
 ##### Email links 
 
 ### Writing Links
 Links are created using the` <a>` element. Users can click on anything between the opening `<a> `tag and the closing
 ` </a>` tag. You specify which page you want to link to using the href attribute.

  example ` <a href="http://www.imdb.com">IMDB</a>`


### Linking to Other Sites
Links are created using the ` <a> ` element which has an attribute called href. The value of the href attribute is the page that you want people to go to when they click on the link.


### Linking to Other Pages on the Sa me Site
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
page. You will learn more about
these.


### Email Links
To create a link that starts up
the user's email program and
addresses an email to a specified
email address, you use the ` <a> `
element. However, this time the
value of the href attribute starts
with ` mailto: ` and is followed by
the email address you want the
email to be sent to.

### Opening Links in a New Window  `target`
target
If you want a link to open in a
new window, you can use the
target attribute on the opening
`<a> `tag. The value of this
attribute should be _blank.
One of the most common
reasons a web page author
might want a link to be opened
in a new window is if it points to
another website. In such cases,
they hope the user will return
to the window containing their
site after finishing looking at the
other one.

ex : ` <a href="http://www.imdb.com" target="_blank"> `
` Internet Movie Database</a> (opens in new window) `





### Linking to a Sp ecific


Before you can link to a specific
part of a page, you need to
identify the points in the page
that the link will go to. You do
this using the id attribute (which
can be used on every HTML
element). 
The value of the id attribute
should start with a letter or an
underscore (not a number or
any other character) and, on a
single page, no two id attributes
should have the same value.
To link to an element that uses
an id attribute you use the` <a>`
element again, but the value of
the href attribute starts with
the ` # ` symbol, followed by the
value of the id attribute of the
element you want to link to. In
this example,`  <a href="#top"> `.  



### Linking to a Sp ecific Part of Another Page

If you want to link to a specific
part of a different page (whether
on your own site or a different
website) you can use a similar
technique.
As long as the page you are
linking to has id attributes that
identify specific parts of the
page, you can simply add the
same syntax to the end of the
link for that page.
Therefore, the href attribute
will contain the address for the
page (either an absolute URL or
a relative URL), followed by the
` symbol,` followed by the value
of the id attribute that is used on
the element you are linking to.
For example, to link to the
bottom of the homepage of the
website that accompanies this
book, you would write:
`<a href="http:/www. htmlandcssbookcom/ #bottom">`




## chapter 15 LAYOUT 

#### Controlling the position of elements
#### Creating site layouts
#### Designing for different sized screens

### Key Concepts in Positioning Elements

CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.
Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use
borders, margins, padding, and background colors.

`Block-level elements nstart on a new line`
`Examples include: <h1> <p> <ul> <li>`


`Inline elements flow in between surrounding text`
`Examples include: <img> <b> <i>`



###### Containing Elements
If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.


#### Controlling the Position of Elements

##### Normal flow
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

##### Relative Positioning
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed. This
does not affect the position of
surrounding elements; they stay
in the position they would be in
in normal flow.

##### Absolute positioning
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


##### Fixed Positioning
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

##### Floating Elements
Floating an element allows
you to take that element out
of normal flow and position
it to the far left or right of a
containing box. The floated
element becomes a block-level
element around which other
content can flow.



# JAVASCRIPT

![img](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQKXEPtuKHhrUBeYgffURdG09fsgEXBhosjCQ&usqp=CAU):
## CHAPTER 3 FUNCTIONS, METHODS & OBJECTS


##### WHAT IS A FUNCTION?
Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of st atements).

#### DECLEARING A FUNCTION 
 using a ` function ` keyword : ` function hello(){
     code block
 }
 where the world ` hello ` is the function name .

 #### calling a function 
 you can call a function by writing its name ex : hello().

#### deaclearing function that need information
when you decleared a function you give it parameters. inside the function the parameter act like variables. to call this function you spacify the value it should use in the parenthesesthat follow its name.

#### calling a function that need informations 
 you can call a function by writing its name and the value ex : hello(3,5).

 #### gitting a single value out of a function 
 you can do it by using ` return ` command.

##### ANONYMOUS FUNCTIONS & FUNCTION EXPRESSIONS
Expressions produce a value. They can be used where values are expected. If a function is placed where a browser expects to see an expression,


#### IMMEDIATELY INVOKED FUNCTION EXPRESSIONS
This way of writing a function is used in several different situations. Often functions are used to ensure that the variable names do not conflict with each other (especially if the page uses more than one script).


#### VARIABLE SCOPE 
The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable's scope.



# 6 Reasons for Pair Programming

Iterative loops. Code reviews. Fast feedback. Error checking and linting. These are software engineering practices that have proven to dramatically improve the quality of code developers produce. What if you can could get all of this, instantaneously, while typing code line by line and character by character? You can, with pair programming, a technique common to many agile work environments.

#### How does pair programming work?

While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code


####  Work environment readiness
Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.


