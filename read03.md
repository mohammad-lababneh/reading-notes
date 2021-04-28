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