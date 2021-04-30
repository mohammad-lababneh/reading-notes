
# HTML 

## chapter 1
 **structure**
 talking about commands of HTML like  , and the parts like header , main and footer .
anouther important thing about tages , and how you can make it.
## chapter 8
 **extra markup**
this chapter talking about The different versions of HTML , and the properties of each version. 
How to add comments to your code , If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters:
**<!-- comment goes here -->**.
How to add a page and control with width and hight.
Global attributes, which are attributes that can be used on any element, including the class and id attributes.

## chapter 17

### PERPOSES of this chapter:
#### HTML5 layout elements.
#### How old browsers understand new elements.
#### Styling HTML5 layout elements with CSS.
  

**HTMLs layout**
*Traditional HTML Layouts*
For a long time, web page authors used `<div>` elements to group
together related elements on the page (such as the elements that form a
header, an article, footer or sidebar). Authors used class or id attributes
to indicate the role of the `<div>` element in the structure of the page.

*The new HTML5 elements* indicate the purpose of
different parts of a web page and help to describe
its structure.
 The new elements provide clearer code.
 Older browsers that do not understand HTML5
elements need to be told which elements are
block-level elements.
 To make HTML5 elements work in Internet Explorer 8
(and older versions of IE), extra JavaScript is needed,
which is available free from Google.

### Headers & Footers
 1) The main header or footer that appears at the top or
bottom of every page on the site.
2) A header or footer for an individual `<article>` or ``<section>` within the page.


### Articles `<article>`

The `<article> `element acts as a container for any section of a
page that could stand alone and potentially be syndicated.
This could be an individual article or blog entry, a comment
or forum post, or any other independent piece of content.
If a page contains several articles (or even summaries of several
articles), then each individual article would live inside its own
`<article>` element.
The `<article>` elements can even be nested inside each other. For example, a blog post
might live inside one `<article>` element and each comment on
the article could live inside its own child `<article>` element.

### section
The `<section> ` element groups related content together, and
typically each section would have its own heading. Because the` <section> `element groups related items together,
it may contain several distinct `<article> `elements that have a common theme or purpose.
Alternatively, if you have a page with a long article, the
`<section> `element can be used to split the article up into
separate sections. The` <section> `element should not be used as a wrapper for the entire page (unless the page only contains one distinct piece of content). If you want a
containing element for the entire page, that job is still best left to the `<div>` element.

### Heading Groups
The purpose of the` <hgroup>` element is to group together a
set of one or more` <h1> `through `<h6>` elements so that they are treated as one single heading.


### Sectioning Elements
It may seem strange to follow these new elements by revisiting
the **div** element again. (After all, the new elements are often going to be used in its place.)
However, the **div** element will remain an important way to
group together related elements, because you should not be using these new elements that you have just met for purposes other than those explicitly stated.
Where there is no suitable element to group a set of
elements, the` **div** element will still be used. In this example, it is used as a wrapper for the entire
page. Some people have asked why
there is no **content** element to contain the main part of
a page. The reason is that anything that lies outside of the
**header**, **footer** or **aside** elements can be considered as
the main content.

### Linking Around Block-Level El ements
HTML5 allows web page authors to place an `a` element around a block level element that contains child elements. This allows you to turn an entire block
into a link. This is not a new element in
HTML5, but it was not seen as a correct usage of the `a` element in earlier versions of HTML.

### Helping Ol der Browsers Understand
Older browsers that do not know the new HTML5 elements
will automatically treat them as inline elements. Therefore, to help older browsers, you should
include the line of CSS on the left which states which new elements should be rendered as block-level elements.








## chapter 18  
**process and design**
In this chapter, we will learn at : How to understand the audience your site may attract and what information they will expect to find on it.
what kind of people that will visit your wep site , and how you can make it convenient for them.
it is convenient for woman or men ? or both of thim ? 
 How to organize information so that visitors can find what
they are looking for Design theory for presenting information in a way that helps visitors achieve their goals.
Design tips to help you create more attractive and
professional sites.


##### Who is the Site For?
Every website should be designed for the target audience—not just for yourself or the site owner. It is therefore very important to understand who your target audience is.

##### Target Audience: individuals
`What is the age range of your target audience?`
 Will your site appeal to more women or men? What is the mix?
 `Which country do your visitors live in?`
 Do they live in urban or rural areas?
`What is the average income of visitors?`
 What level of education do they have?
 `What is their marital or family status?`
What is their occupation?
 `How many hours do they work per week?`
 How often do they use the web?
 `What kind of device do they use to access the web?`

##### What Your Visitors are Trying to Achieve
It is unlikely that you will be able to list every reason why someone visits your site but you are looking for key tasks and motivations. This information can help guide your site designs.


##### What Information Your Visitors Need
You know who is coming to your site and why they are coming, so now you need to work out what information they need in order to achieve their goals quickly and effectively.

##### How Of ten People Will Visit Your Site
Some sites benefit from being updated more frequently than others. Some information (such as news) may be constantly changing, while other content remains relatively static.

##### WireFrames
A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.

##### Getting your message across using design
The primary aim of any kind of visual design is to communicate. Organizing and prioritizing information on a page helps users understand its importance and what order to read it in.

##### Visual hierarchy
Most web users do not read entire pages. Rather, they skim to find information. You can use contrast to create a visual hierarchy that gets across your key message and helps users find what they are looking for.

### Designing Navigation 
Site navigation not only helps people find where they want to go, but also helps them understand what your site is about and how it is organized.
Good navigation tends to follow these principles.

###### Concise
Ideally, the navigation should be quick and easy to read. It is a good idea to try to limit the
number of options in a menu to no more than eight links. These
can link to section homepages which in turn link to other pages.
###### Clear
Users should be able to predict the kind of information that
they will find on the page before clicking on the link.
Where possible, choose single descriptive words for each link
rather than phrases.
###### Selective
The primary navigation should only reflect the sections or
content of the site. Functions like logins and search, and legal information like terms and conditions and so on are best
placed elsewhere on the page.














# JAVASCRIPT 

*In these pages, the author show how the HTML, CSS, and JAVA are fit together. *
Starting with the HTML layer allows you to focus on content. Adding the CSS rules in a separate file keeps rules regarding how the page looks away from the content itself. The JavaScript is added last
and enhances the usability of the page or the experience of interacting with the site.

Creating a basic JAVASCRIPT, It is written in plain text, just like HTML and CSS, so you do not
need any new tools to write a script.
A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement.
Statements should end with a semicolon ** ; **.

Statements are instructions that the computer should follow. Each statement should start on a
new line and end with a semicolon. 
You should write comments to explain what your code does. Using single line comment ** // ** and multi-line comment ** /* ** . They help make your code easier to read and understand.

What is a variable?
The variable use to store value, and this value can change on each time the script run.