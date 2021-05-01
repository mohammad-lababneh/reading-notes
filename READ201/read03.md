
# HTML 
## ch3 Lists
###### Ordered Lists
The ordered list is created with the ```<ol>``` element.
Each item in the list is placed between an opening *li* tag
and a closing ```</li>``` tag. (The li stands for list item.)

###### unOrdered Lists
The unordered list is created with the ```<ul>``` element.
Each item in the list is placed between an opening *li* tag
and a closing``` </li>``` tag. (The li stands for list item.)

###### Definition Lists
The definition list is created with the ```<dl>``` element and usually consists of a series of terms and their definitions.

```<dt>```
This is used to contain the term being defined (the definition
term).

```<dd>```
This is used to contain the definition.

note : There are three t XX ypes of HTML lists: ordered,
unordered, and definition.
Ordered lists use numbers.
Unordered lists use bullets.

## ch13 Boxes 
using this command you can creat a boxe with any color ```  div.box { height: 300px;```
width: 300px;
background-color: #bbbbaa;}
p {
height: 75%; width: 75%;
background-color: #0088dd;} 

###### Border Width
The border-width property is used to control the width
of a border. The value of this property can either be given
in pixels or using one of the following values:

using these commands
``` <p class="one"> </p>```
```<p class="two"> </p>```
```<p class="three"> </p> ..... to eight ```
*** css ***
to git a style
p.one {border-style: solid;}
p.two {border-style: dotted;}
p.three {border-style: dashed;}
p.four {border-style: double;}
p.five {border-style: groove;}
p.six {border-style: ridge;}
p.seven {border-style: inset;}
p.eight {border-style: outset;}

 ###### Border Color
  ```p.one {```
```border-color: #0088dd;}```
```p.two {border-color: #bbbbaa #111111 #ee3e80 #0088dd;} ```
 using this command you can choose any color

 #### notes 
 CSS treats each HTML e XX lement as if it has its own box.
XX You can use CSS to control the dimensions of a box.
It is possible to hide elements using the display and
visibility properties.
CSS3 has introduced the ability to create image
borders and rounded borders.




## javascript 
### chapter 2
#### CHANGING THE VALUE OF A VARIABLE
Once you have assigned a value to a variable, you can then change what is stored in the variable later in the same script. Once the variable has been created, you do not need to
use the var keyword to assign it a new value. You just use the variable name, the equals sign (also known as the assignment operator), and the new va lue for that attribute.


#### RULES FOR NAMING VARIABLES
Here are six rules you must always follow when giving a variable a name:

1) The name must begin with a letter, dollar sign ($),or an underscore (_). It must not start
with a number.
2) The name can contain letters, numbers, dollar sign ($), or an
underscore (_). Note that you must not use a dash(-) or a period (.) in a variable name.
3) You cannot use keywords or reserved words. Keywords are special words that tell the
interpreter to do something. For example, var is a keyword used
to declare a variable. Reserved words are ones that may be used in a future version of JavaScript.
4) All variables are case sensitive, so score and Score would be
different variable names, but it is bad practice to create two
variables that have the same name using different cases.
5) Use a name that describes the kind of information that the
variable stores. For example, fi rstName might be used to
store a person's first name, l astNarne for their last name, and age for their age.
6) If your variable name is made up of more than one word, use a
capital letter for the first letter of every word after the first word.
For example, f i rstName rather than fi rstnarne (this is referred
to as camel case). You can also use an underscore between each
word (you cannot use a dash).



### ARRAYS
An array is a special type of variable. It doesn't just store one value; it stores a list of values. You should consider using an array whenever you are working
with a list or a set of values that are related to each other.
Arrays are especially helpful when you do not know how
many items a list will contain because, when you create the
array, you do not need to specify how many values it will hold.

### CREATING AN ARRAY
You create an array and give it a name just like you would any
other variable (using the var keyword followed by the name of
the array). The values are assigned to the
array inside a pair of square brackets, and each value is
separated by a comma. The values in the array do not need
to be the same data type, so you can store a string, a number and
a Boolean all in the same array.

#### VALUES IN ARRAYS
Values in an array are accessed as if they are in a numbered list. It is important to know that the
numbering of this list starts at zero (not one).

##### NUMBERING ITEMS IN AN ARRAY
Each item in an array is
automatically given a number
called an index. This can be used
to access specific items in the
array.

##### ACCESSING ITEMS IN AN ARRAY
To retrieve the third item on the
list, the array name is specified
along with the index number in
square brackets.

##### NUMBER OF ITEMS IN AN ARRAY
Each array has a property called length, which holds the number
of items in the array.

##### ACCESSING & CHANGING VALUES IN AN ARRAY
To access a value from an array, after the array name you specify
the index number for that value inside square brackets.
You can change the value of an item an array by selecting it and
assigning it a new value just as you would any other variable
(using the equals sign and the new value for that item).



# chapter 4
## SWITCH STATEMENTS
A switch statement starts with a variable called the switch value.
Each case indicates a possible value for this variable and the
code that should run if the variable matches that value.

#### IF ... ELSE
• There is no need to provide an el se option. (You can just use an if statement.)
• With a series of if statements, they are all checked even if a match has been found (so it performs more slowly than switch).

#### SWITCH
• You have a default option that is run if none of the cases match.
• If a match is found, that code is run; then
the break statement stops the rest of the switch statement running (providing better performance than multiple i f
statements).



### TYPE COERCION & WEAK TYPING
If you use a data type JavaScript did not expect,
it tries to make sense of the operation rather
than report an error.
JavaScript can convert data types behind the scenes to
complete an operation. This is known as type coercion.

** JavaScript is said to use weak 
typing because the data type
for a value can change. Some
other languages require that you
specify what data type
each variable will be. They are
said to use strong typing.** 


### TRUTHY & FALSY VALUES
Due to type coercion, every value in JavaScript can be treated as if it were true or false; and this has some interesting side effects.
**Falsy** values are treated as if they
are false. also be treated as the number 0 .

**Truthy**values are treated as if they are true. Almost everything that is not in the falsy table can
be treated as if it were true. Truthy va lues can also be treated as the number 1.


#### CHECKING EQUALITY & EXISTENCE
Because the presence of an object or array can
be considered truthy, it is often used to check
for the existence of an element within a page.


#### SHORT CIRCUIT VALUES
Logical operators are processed left to right. They short-circuit (stop) as soon as they have a result - but they return the value that stopped the processing (not necessarily true or fa 1 se).
Logical operators will not always return true or false, because:
• They return the value that stopped processing.
• That va lue might have been
treated as truthy or fa lsy although it was not a Boolean.

#### loops 
loops check a condition . if it return true, a code block will run. 
then the condition will be checked a gain and if i still retun true .
the code block will run a gain. it repeats until the condition returns false .
 there are three command types of loops :
 1 ) for 
 2 ) while 
 3 ) do while
### loop counter
 In computer programming a loop counter is the variable that controls the iterations of a loop

 ### KEY LOOP CONCEPTS
Here are three points to consider when you are working with loops. Each is illustrated in examples on the following three pages.

**LOOPS & ARRAYS**
Loops are very helpful when dealing with arrays if you want to run the same code for each item
in the array.
For example, you might want
to write the value of each item
stored in an array into the page.
You may not know how many
items will be in an array when
writing a script, but. when the
code runs, it can check the total
number of items in a loop. That
figure can then be used in the
counter to control how many
times a set of statements is run.


### USING FOR LOOPS
A for loop is often used to loop
through the items in an array.
In this example, the scores for
each round of a test are stored in
an array called scores.
The total number of items in
the array is stored in a variable
called arrayl ength. This
number is obtained using the
l ength property of the array.

### USING WHILE LOOPS
This loop will continue to run
for as long as the condition in
the parentheses is true.


### USING DO WHILE LOOPS.
The key difference between a whi 1 e loop and a do whi 1 e
loop is that the statements in the code block come before the
condition. This means that those statements are run once whether or not the condition is met.