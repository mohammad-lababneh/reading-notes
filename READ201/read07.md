<!-- From the Duckett HTML book:

Chapter 6: “Tables” (pp.126-145)
From the Duckett JS Book:

Chapter 3: “Functions, Methods, and Objects” (pp.106-144) -->



# HTML 

### CHAPTER 6 Tables
![TABLE](https://data-flair.training/blogs/wp-content/uploads/sites/2/2020/07/Html-Tables.jpg)

`How to create tables.`
`What information suits tables.`
`How to represent complex data in tables.`

When representing information in a table, you need to think
in terms of a grid made up of rows and columns 
(a bit like aspreadsheet)
. In this chapter you will learn how to:
Use the four key elements for creating tables
Represent complex data using tables
Add captions to tables

#### What's a Table?
A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.


#### Basic Table Structure
`<table>`
The `<table>` element is used
to create a table. The contents
of the table are written out row
by row.
`<tr> `
You indicate the start of each
row using the opening` <tr> `tag.
(The tr stands for table row.)
It is followed by one or more
`<td> `elements (one for each cell
in that row).
At the end of the row you use a
closing` </tr>` tag.
`<td> `
Each cell of a table is
represented using a` <td> `
element. (The td stands for
table data.)
At the end of each cell you use a
closing ` </td>  `tag.

![TABLE](https://images.slideplayer.com/20/6057530/slides/slide_3.jpg)


#### Table Headings

`<th>`
The` <th> `element is used just
like the` <td> ` element but its
purpose is to represent the
heading for either a column or
a row. (The` th `stands for table
heading.)
Even if a cell has no content,
you should still use a` <td> `or
`<th> `element to represent
the presence of an empty cell
otherwise the table will not
render correctly. (The first cell
in the first row of this example
shows an empty cell.)


#### Spanning ColumnS
Sometimes you may need the
entries in a table to stretch
across more than one column.
The colspan attribute can be
used on a` <th>` or `<td> `element
and indicates how many columns

#### Spanning Rows
You may also need entries in
a table to stretch down across
more than one row.
The rowspan attribute can be
used on a `<th> ` or ` <td> `element
to indicate how many rows a cell
should span down the table.


#### Long Tables
There are three elements that
help distinguish between the
main content of the table and
the first and last rows
 (which can contain different content).
These elements help people
who use screen readers and also
allow you to style these sections
in a different manner than the
rest of the table .
`<thead>`
The headings of the table should
sit inside the `<thead> `element.

`<tbody>`
The body should sit inside the
` <tbody> `element.

` <tfoot> `
The footer belongs inside the
` <tfoot> ` element.


#### Old Code: Width & Spacing
There are some outdated attributes which you should not
use on new websites. You may, however, come across some
of them when looking at older code, so I will mention them
here. All of these attributes have been replaced by the use of CSS.


#### Old Code: Border & Background

The border attribute was used on both the` <table> ` and `<td> ` elements to indicate the width of the border in pixels.

### Summary
TABLES
XX The` <table> ` element is used to add tables to a web
page.
XX A table is drawn out row by row. Each row is created
with the` <tr> `element.
XX Inside each row there are a number of cells
represented by the` <td> `element (or` <th> `if it is a
header).
XX You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.
XX For long tables you can split the table into a` <thead> `,
`<tbody> `, and` <tfoot> `.





## Summary

The` <table> `element is used to add tables to a web
page.
A table is drawn out row by row. Each row is created
with the` <tr> ` element.
Inside each row there are a number of cells
represented by the` <td> `element (or` <th> `if it is a
header).
You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.
For long tables you can split the table into a `<thead> `,
`<tbody> `, and` <tfoot> `.






# JAVASCRIPT 
### CHAPTER 3 (pp.106-144)
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRma0Ti2m7aWjp8FCDouQzw4458oDauWPpbEA&usqp=CAU) 


### UPDATING AD OBJECT
To update the value of properties , use dot or square brackets.
thay work on objects created using literal or constructor notation .
To delete a property , use the `Delete `keyword .


### CREATING MANY OBJECTS:

Sometimes you will want several objects to represent similar things.
Object constructors can use a function as a template for creating objects.
First, create the template with the object's properties and methods.

### ADDING AND REMOVING PROPERTIES

Once you have created an object
(using literal or constructor
notation), you can add new
properties to it.
You do this using the dot
notation that you saw for adding
properties to objects.


### RECAP: WAYS TO CREATE OBJECTS
RECAP: WAYS TO CREATE OBJECTS

In this examples, the object is created on
the first line of the code sample. The properties and
methods are then added to it afterwards.



`LITERAL NOTATION`
`var hotel = {}`
`hotel .name= 'Quay';`
`hotel .rooms = 40;`
`hotel.booked = 25;`
`hotel.checkAvailabil ity =function()`
`return this . rooms - this .booked;`
`} ;`



#### THIS (IT IS A KEYWORD)
The keyword this is commonly used inside functions and objects. Where the function is declared alters what this means. It always refers to one object, usually the object in which the function operates.

`A FUNCTION IN GLOBAL SCOPE`
When a function is created at the top level of a script
(that is, not inside another object or function), then it
is in the global scope or global context.

`GLOBAL VARIABLES`
All global variables also become properties of the
window object. so when a function is in the global
context, you can access global variables using the
window object, as well as its other properties.





#### RECAP: STORING DATA
In JavaScript, data is represented using name/value pairs. To organize your data, you can use an array or object to group a set of related values. In arrays and objects the name is also known as a key.

`VARIABLES`
A variable has just one key (the variable name)
and one va lue.

`ARRAYS`
Arrays can store multiple pieces of information.
Each piece of information is separated by a comma.
The order of the values is important because items
in an array are assigned a number (called an index).
![](https://samanthaming.gumlet.io/tidbits/76-converting-object-to-array.jpg.gz)

#### ARRAYS ARE OBJECTS 
it is a speacial type of object. they hold arelated set of key , but the key for each value is its index number.





#### WHAT ARE BUILT-IN OBJECTS?
![](https://i.imgur.com/J3ETg5D.png)

The first thing you need to do is get to know what tools are available. You can imagine that your new toolkit has three compartments.
 ###### 1) GLOBAL JAVASCRIPT OBJECTS
The global JavaScript objects
represent things that the JavaScript
language needs to create a model
of. For example, there is an
object that deals only with
dates and times.
###### 2)DOCUMENT OBJECT MODEL
The Document Object Model uses
objects to create a representation of
the current page. It creates a new
object for each element (and each
individual section of text)
within the page.
###### 3)BROWSER OBJECT MODEL
The Browser Object Model contains
objects that represent the current
browser window or tab. It contains
objects that model things like
browser history and the
device's screen.

### THE BROWSER OBJECT MODEL: THE WINDOW OBJECT
The window object represents the current
browser window or tab. It is the topmost object
in the Browser Object Model, and it contains
other objects that tell you about the browser.




#### USING THE BROWSER OBJECT MODEL

Child objects are stored as properties of t heir parent object. So dot notation is used to access
them, just like you would access any other property of that object.


##### The topmost object in the Document Object Model (or DOM) is the
document object. It represents the web page loaded into the current browser window or tab.

The topmost object in the Document Object Model (or DOM) is the document object. It represents the web page loaded into the current browser window or tab.

#### DATA TYPES REVISITED
In JavaScript there are six data types:
Five of them are described as simple (or primitive) data types.
The sixth is the object (and is referred to as a complex data type).

1. String
2. Number
3. Boolean
4. Undefined
5. Null
6. 0bject

## SUMMARY
`Functions allow you to group a set of related`
`statements together that represent a single task.`
Functions can take parameters (informatiorJ required
to do their job) and may return a value.
`An object is a series of variables and functions that`
`represent something from the world around you.`
In an object, variables are known as properties of the
object; functions are known as methods of the object.
`Web browsers implement objects that represent both`
`the browser window and the document loaded into the`
`browser window.`
JavaScript also has several built-in objects such as
String, Number, Math, and Date. Their properties and
methods offer functionality that help you write scripts.
`Arrays and objects can be used to create complex data`
`sets (and both can contain the other).`


