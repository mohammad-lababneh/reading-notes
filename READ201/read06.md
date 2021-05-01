# chapter 3 
### WHAT IS AN OBJECT? 
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.

#### IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES
If a variable is part of an object, it is called a
**property**. Properties tell us about the object, such as the name of a hotel or the number of rooms it has.
Each individual hotel might have a different name and a different number of rooms.


#### IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS
If a function is part of an object, it is called a method.
Methods represent tasks that are associated with
the object. For example, you can check how many
rooms are available by subtracting the number of
booked rooms from the total number of rooms.


Like variables and named functions, properties and methods have a name and a va lue. In an object,
that name is called a *key.* An object cannot have two keys
with the same name. This is because keys are used to access their corresponding values.
The value of a property can be a string, number, Boolean, array, or even another object. The va lue of a
method is always a function.



Programmers use a lot of name/value pairs:
• HTML uses attribute names and values.
• CSS uses property names and values.
**In JavaScript:**
• Variables have a name and you can assign them a
value of a string, number, or Boolean.
• Arrays have a name and a group of values. (Each
item in an array is a name/value pair because it
has an index number and a value.)
• Named functions have a name and value that is a
set of statements to run if the function is called.
• Objects consist of a set of name/value pairs
(but the names are referred to as keys).


### creating an object: literal notaton.
literal notation is trhe easiest and most popular way to create objects.


### accessing an object and dot notation.
you access the properties or methods of an object using dot notation.
you can also access properties using square brackets.

to access a property or method of an object you use the name of the object, followed by a period, then the name of the property or method you want to access.


### CREATING· OBJECTS USING LITERAL NOTATION
To access a property of this object, the object name is
followed by a dot (the period symbol) and the name of the
property that you want.
Similarly, to use the method, you can use the object name
followed by the method name.
hotel .checkAvailability()

### CREATING MORE OBJECT LITERALS
If you had two objects on the
same page, you would create
each one using the same
notation but store them in
variables with different names.


# chapter 5 DOCUMENT OBJECT MODEL
The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

## MAKING A MODEL OF THE HTML PAGE
When the browser loads a web page, it creates a model of the page in memory.
The DOM specifies the way in which the
browser should structure this model using
a **DOM** tree.
The DOM is called an object model
because the model (the DOM tree) is
made of objects.

#### THE DOM TREE IS A MODEL OF A WEB PAGE
As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
It consists of four main types of nodes.

#### ELEMENT NODES
HTML elements describe the structure of an HTML
page. (The `<h l >` - `<h6>` elements describe what
parts are headings; the `<p>` tags indicate where
paragraphs of text start and finish; and so on.)
To access the DOM tree, you start by looking for
elements. Once you find the element you want, then
you can access its text and attribute nodes if you
want to. This is why you start by learning methods
that allow you to access element nodes, before
learning to access and alter text or attributes.


Each node is an object with methods and properties. Scripts access and update this DOM tree Any changes made to the DOM tree are reflected in the browser.


### TEXT NODES
Once you have accessed an element node, you
can then reach the text within that element. This is
stored in its own text node.


### ATTRIBUTE NODES
The opening tags of HTML elements can carry attributes and these are represented by attribute nodes in the DOM tree.

### WORKING WITH THE DOM TREE
Accessing and updating the DOM tree involves two steps:
1: Locate the node that represents the element you want to work with.
2: Use its text content, child elements, and attributes.


### ACCESSING ELEMENTS
DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes.

### GROUPS OF ELEMENT NODES
If a method can return more than one node, it will
always return a Nodelist, which is a collection of
nodes (even if it only finds one matching element).

### FASTEST ROUTE
Finding the quickest way to access an element
within your web page will make the page seem
faster and/or more responsive. This usually means
evaluating the minimum number of nodes on the
way to the element you want to work with.


##### getElementByld( ' id ')
Selects an individual element given the value of its i d attribute .
The HTML must have an id attribute in order for it to be selectable.
##### querySel ector( '1css selector ')
Uses CSS selector syntax that would select one or more element s .
This method returns only the first of the matching elements.

 ### getEl ement sByClassName( 1class 1 )
Selects one or more elements given the va lue of their cl ass attribute.
The HTML must have a cl ass attribu te for it to be selectable.
This method is faster than querySe 1ectorA11 () .

### getEl ementsByTagName(  tagName )
Selects all elements on the page with the specified tag name.
This method is faster than querySe 1ectorA11 ().


### querySelectorAll ( css selector )
Uses CSS selector syntax to select one or more elements and returns all of those that match.


## SELECTING ELEMENTS USING ID ATTRIBUTES
get El ementByid () al lows you
to select a single element node
by specifying the value of its
id attribute.
This method has one parameter:
the value of the id attribute on
the element you want to select.
This value is placed inside quote
marks because it is a string. The
quotes can be single or double
quotes, but they must match.

## NODELISTS: DOM QUERIES THAT RETURN MORE THAN ONE ELEMENT
When a DOM method can return more than one element, it returns a Nodelist (even if it only finds one matching element).

Nodelists look like arrays and are numbered like
arrays, but they are not ac tually arrays; they are a
type of object called a collection.



### SELECTING ELEMENTS USING CLASS ATTRIBUTES

The get El ementsByCl ass Name() method allows you to select
elements whose c 1 ass attribute contains a specific value.

The method has one parameter: the class name which is given
in quotes within the parentheses after the method name.

### SELECTING ELEMENTS BYTAG NAME

The get El ementsByTagName () method allows you to select
elements using their tag name.
The element name is specified as a parameter, so it is placed
inside the parentheses and is contained by quote marks.

### SELECTING ELEMENTS USING CSS SELECTORS

querySe 1 ector() returns the first element node that
matches the CSS-style selector.
querySe 1ectorA11 () returns a Nodelist of all of the matches


Both methods take a CSS selector as their only parameter.
The CSS selector syntax offers more flexibility and accuracy
when selecting an element than.


### LOOPING THROUGH A NODELIST
If you want to apply the same code to numerous elements,
looping through a Nodelist is a powerful technique.
It involves finding out how many items are in the Nodelist, and then setting a counter to loop through them, one-by-one.


### TRAVERSING THE DOM
When you have an element node, you can select
another element in relation to it using these five
properties. This is known as traversing the DOM.

## parentNode
This property finds the element
node for the containing (or
parent) element in the HTML.


## previousSibling nextSibling
These properties find the
previous or next sibling of a node
if there are siblings.

### i rstChild lastChild
These properties find the first or
last child of the current element.



### PREVIOUS & NEXT SIBLING
You have just seen that these properties can return
inconsistent results in different browsers. However, it is safe to use them when there is no
whitespace between elements.

For this example, all spaces between the HTML elements
have been removed. In order to demonstrate these properties,
the second list item is selected using getEl ementByld ().

### FlRST & LAST CHILD
These properties also return inconsistent resu lts if there is whitespace between elements.
In this example, a slightly different solution is used in the
HTML - the closing tags are put.

### HOW TO GET/UPDATE ELEMENT CONTENT
So far this chapter has focused on finding elements in the DOM tree.
The rest of this chapter shows how to access/update element content.
Your choice of techniques depends upon what the element contains.


### ACCESS & UPDATE A TEXT NODE WITH NODEVALUE
When you select a text node, you can retrieve or amend the content of it using the node Va 1 ue property.
In order to use node Va 1 ue, you
must be on a text node, not the
element that contains the text.


### ACCESSING & CHANGING A TEXT NODE
To work with text in an element,
first the element node is
accessed and then its text node.

The text node has a property
called node Value which returns
the text in that text node.

You can also use the node Va 1 ue
property to update the content
of a text node.



### ACCESS & UPDATE TEXT WITH TEXTCONTENT (& INN ERTEXT)
The textCon tent property allows you to
collect or update just the text that is in the
containing element (and its children).




### textContent
To collect the text from the
`<li>` elements in our example
(and ignore any markup inside
the element) you can use the
textContent property on the
containing `<li >` element. In this
case it would return the value.



### innerText
You may also come across a property called i nner Text, but you should generally avoid it for three key reasons:

###### SUPPORT
Although most browser
manufacturers adopted the
property, Firefox does not
because i nnerText is not part of
any standard.

###### OBEYS CSS
It will not show any content
that has been hidden by CSS.
For example, if there were a CSS
rule that hid the `<em>` elements,
the i nnerText property would
return only the word figs.


### PERFORMANCE
Because the i nnerText property
takes into account layout rules
that specify whether the element
is visible or not, it can be slower
to retrieve the content than the
textContent property.



### ACCESSING TEXT ONLY
In order to demonstrate the
difference between textContent
and i nnerText, this example
features a CSS rule to hide the
contents of the` <em> ` element.
The script starts off by getting
the content of the first list item
using both the textContent
property and i nnerText. It then
writes the values after the list.

Finally, the value of the first
list item is then updated to say
sourdough bread. This is done
using the textContent property.



### ACCESS & UPDATE TEXT & MARKUP WITH INNERHTML

Using the i nnerHTML property, you can access
and amend the contents of an element,
including any child elements.


##### innerHTML
When getting HTML from an
element, the i nnerHTML property
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


### UPDATE TEXT & MARKUP
This example starts by storing
the first list item in a variable
called fi rstltem.
It then retrieves the content of
t his list item and stores it in a
variable called i temContent.
Finally, the content of the list
item is placed inside a link. Note
how the quotes are escaped.



#### ADDING ELEMENTS USING DOM MANIPULATION
DOM manipulation offers another technique
to add new content to a page (rather than
i nnerHTML). It involves three steps:

1 ) CREATE THE ELEMENT createEl ement ()
2) GIVE IT CONTENT createTextNode()
3) ADD IT TO THE DOM appendChild()


#### ADDING AN ELEMENT TO THE DOM TREE
createEl ement () creates an
element that can be added to the
DOM tree, in this case an empty
`<li> `element for the list.
This new element is stored
inside a variable called newEl
until it is attached to the DOM
tree later on.
createTextNode() allows you to
create a new text node to attach
to an element. It is stored in a
variable called newText.

### REMOVING ELEMENTS VIA DOM MANIPULATION
DOM manipulation can be used to remove
elements from the DOM tree.
1) STORE THE ELEMENT TO BE REMOVED IN A VARIABLE
2) STORE THE PARENT OF THAT ELEMENT IN A VARIABLE
3) REMOVE THE ELEMENT FROM ITS CONTA INING ELEMENT



### COMPARING TECHNIQUES: UPDATING HTML CONTENT
So far, you have seen three techniques for adding HTML to a web page. It's time to compare when you should use each one.

In any programming language, there are often
several ways to achieve the same task. In fact, if you
asked ten programmers to write the same script, you
may well find ten different approaches.



### DOM MANIPULATION
DOM manipulation refers to using a set of methods
and properties to access, create, and update
elements and text nodes.


## ADVANTAGES
It is suited to changing one element from a DOM
fragment where there are many siblings.
It does not affect event handlers.
It easily allows a script to add elements
incrementally (when you do not want to alter a lot
of code at once).


### DEFENDING AGAINST CROSS-SITE SCRIPTING
VALIDATE INPUT GOING TO THE SERVER
1. Only let visitors input the kind
of characters they need to when
supplying information. This is
known as validation. Do not
allow untrusted users to submit
HTML markup or JavaScript.

2. Double-check validation on
the server before displaying user
content/storing it in a database.
This is important because users
could bypass validation in the
browser by turning JavaScript off.

3. The database may safely
contain markup and script
from trusted sources (e.g., your
content management system).
This is because it does not try to
process the code; it just stores it.



#### XSS: VALIDATION & TEMPLATES
Make sure that your users can only input characters they need to use and limit where this content will be shown on the page.

#### FILTER OR VALIDATE INPUT
The most basic defense is to prevent users from
entering characters into form fields that they do not
need to use when providing that kind of information.


#### LIMIT WHERE USER CONTENT GOES
Malicious users will not just use `<script> `tags to
try and create an XSS attack. As you saw on p228,
malicious code can live in an event handler attribute
without being wrapped in `<script> `tags. XSS can
also be triggered by malicious code in CSS or URLs.

### XSS: ESCAPING & CONTROLLING MARKUP
Any content generated by users that contain characters that are used in code should be escaped on the server. You must control any markup added to the page.


### ESCAPING USER CONTENT
All data from untrusted sources should be escaped
on the server before it is shown on the page.
Most server-side languages offer helper functions
that will strip-out or escape malicious code.

### ADDING USER CONTENT
When you add untrusted content to an HTML page,
once it has been escaped on the server, it should still
be added to the page as text. JavaScript and jQuery
both offer tools for doing this.

### CHECK FOR AN ATTRIBUTE AND GET ITS VALUES

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


### CREATING ATTRIBUTES & CHANGING THEIR VALUES

The cl assName property allows
you to change the value of the
cl ass attribute. If the attribute
does not exist, it will be created
and given the specified value.

You have seen this property
used throughout the chapter
to update the status of the
list items. Below, you can see
another way to achieve the task.
The setAttri bute() method
allows you to update the va lue
of any attribute. It takes two
parameters: the attribute name,
and the value for the attribute.


### REMOVING ATTRIBUTES
To remove an attribute from an
element, first select the element,
then call removeAtt r i bute () .
It has one parameter: the name
of the attribute to remove.

Trying to remove an attribute
that does not exist will not cause
an error, but it is good practice
to check for its existence before
attempting to remove it.


In this example, the
get El ementByld () method is
used to retrieve the first item
from this list, which has an id
attribute with a value of one.


### EXAMINING THE DOM IN CHROME
Modern browsers come with tools that help
you inspect the page loaded in the browser
and understand the structure of the DOM tree.



### EXAMINING THE DOM IN FIREFOX

Firefox has similar built-in tools, but you can
also download a DOM inspector tool that
shows the text nodes.

If you search online for "DOM
Inspector", you will find the tool
designed for Firefox shown on
the left. In the screen shot, you
can see a similar tree view to
the one shown in Chrome, but
it also shows you where there
are whitespace nodes (they are
shown as # text). In the panel to
the right, you can see the value
in the nodes; whitespace nodes
have no va lue in this panel.


### summary 
The browser represents the page using a DOM tree.

DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes.

You can select element nodes by their id or cl ass
attributes, by tag name, or using CSS selector syntax.

Whenever a DOM query can return more than one
node, it will always return a Nadel i st.

From an element node, you can access and update its
content using properties such as textContent and
i nnerHTML or using DOM manipulation techniques.

An element node can contain multiple text nodes and
child elements that are siblings of each other.

In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
Browsers offer tools for viewing the DOM tree .








