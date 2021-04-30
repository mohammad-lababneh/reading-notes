

# HTML 
## Capter 2
### Headings

**h1**
**h2**
**h3**
**h4**
**h5**
**h6**
this heading you can use it to make a titles.
Each head deferant on size and importance.


### Paragraphs <p>
can use command *p* to write a paragraphs.

### Bold & Italic <b> <i>

you can use these commands <b> & <i> to make bold to a text, and make it italic. 
By enclosing words in the tags <i> and </i> we can make characters appear italic.
By enclosing words in the tags <b> and </b> we can make
characters appear bold.

### Superscript & Subscript
The **sup** element is used to contain characters that
should be superscript such as the suffixes of dates or
mathematical concepts like raising a number to a power .


### Line Breaks br & Horizontal Rules hr
<br />
 the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag <br />.
<hr />
To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections using the tag.<hr /> 

### Strong & Emphasis
<strong>
The use of the strong element indicates that its
content has strong importance. For example, the words contained in this element might be said with strong emphasis.
By default, browsers will show the contents of a strong
element in bold.

##### em
The **em** element indicates emphasis that subtly changes
the meaning of a sentence. By default browsers will show
the contents of an 'em' element in italic.


### Quotations
<blockquote>
The **blockquote** element is used for longer quotes that take
up an entire paragraph. Note how the **p** element is still
used inside the **blockquote** element.
Browsers tend to indent the contents of the **blockquote**
element, however you should not use this element just to indent a piece of text — rather you should achieve this effect using CSS.</blockquote>

<q>
The  q  element is used for shorter quotes that sit within
a paragraph. Browsers are supposed to put quotes around
the  q  element, however Internet Explorer does not —
therefore many people avoid using the  q  element.
Both elements may use the cite attribute to indicate where the
quote is from. Its value should be a URL that will have more
information about the source of the quotation.</q>


### Abbreviations & Acronyms

If you use an abbreviation or an acronym, then the **abbr**
element can be used. A title attribute on the opening tag is
used to specify the full term.


### Auth or Details
<address>Auth or Details</address>
The **address** element has quite a specific use: to contain
contact details for the author of the page.

### Changes to Content
The **ins**  element can be used to show content that has been
inserted into a document, while the **del** element can show text that has been deleted from it.

The **s** element indicates something that is no longer
accurate or relevant (but that should not be deleted).

## chapter 10 css 
CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.
p {font-family: Arial;}
p : selector 
**Selectors**  indicate which element the rule applies to.
The same rule can apply to more than one element if you
separate the element names with commas.
font-family: Arial : declaration 

**Declarations** indicate how the elements referred to in
the selector should be styled. Declarations are split into two
parts (a property and a value), and are separated by a colon.

### Using External CSS
The **link** element can be used in an HTML document to tell the
browser where to find the CSS file used to style the page.

**href** This specifies the path to the
CSS file (which is often placed in a folder called css orstyles).

**type** This attribute specifies the type of document being linked to. The value should be text/css.

### Usi ng Internal CSS
You can also include CSS rules within an HTML page by placing
them inside a **style** element, which usually sits inside the
<head> element of the page.


# js 
## capter 2 

#### COMMENTS
You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read
 your code using // or /*.

 #### WHAT IS A VARIABLE?
 A script will have to temporarily store the bits of information it needs to do its job. It can store this
data in variables.
you can declear variables using var command,  and you can assign ther command by using = .
USING A VARIABLE TO STORE A STRING by using '' & "".


## chapter 4 DECISIONS & LOOPS 

<blockquote>Looking at a flowchart (for all but the most basic scripts),
the code can take more than one path, which means the
browser runs different code in different situations. In this
chapter, you will learn how to create and control the flow of
data in your scripts to handle different situations.
</blockquote>

#### COMPARISON OPERARTORS: EVALUATING CONDITIONS

###### you can evaluat a situation by combaring one value to a nother using these operators:
is equal to **==**
is not equal to **!=**
strict equal to **===**
strict not equal to **!==**

###### you can chick the condition by using these operators:
greater than **>**
less than**<**
greater than or equal **>=**
less than or equal **<=**

### logica operators allow you to compair the results of more than comparision operator.
logical AND **&&**
logical OR **||**
 logical NOT **!**



### IF ... ELSE STATEMENTS

if .. else statement check the condition.
if the condition is true if will run the statement that inside it . if the coondition is false it will go to else statement.












