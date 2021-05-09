# chapter 10 ERROR HANDLING & DEBUGGING 
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS_ISuGsITDkBrQf-6B_uFmI-vjiJHXBgfU6Q&usqp=CAU);
`JavaScript can be hard to learn and everyone makes`
`mistakes when writing it. This chapter will help you learn`
`how to find the errors in your code. It will also teach you` `how to write scripts that deal with potential errors ``gracefully`


###### THE CONSOLE & DEV TOOLS
Tools built into the browser that help you hunt for errors.

###### COMMON PROBLEMS
Common sources of errors, and how to solve them.

###### HANDLING ERRORS
How code can deal with potential errors gra cefully.



## ORDER OF EXECUTION
To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

### EXECUT.ION CONTEXTS
The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope.


### EXECUTION CONTEXT & HOISTING
Each time a script enters a new execution context, there are two phases of activity:

1: PREPARE
• The new scope is created
• Variables, functions, and arguments are created
• The value of the this keyword is determined

2: EXECUTE
• Now it can assign values to variables
• Reference functions and run their code
• Execute statements

### UNDERSTANDING SCOPE
In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's v a ri ables object.


### UNDERSTANDING ERRORS
If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code.




### ERROR OBJECTS
Error objects can help you find where your mistakes are
and browsers have tools to help you read them.



### EvalError
`INCORRECT USE OF eval() FUNCTION`
The eval() function evaluates text through the interpreter and runs it as code (it is not discussed
in this book). It is rare that you would see this type of error, as browsers often throw other errors when
they are supposed to throw an Eva 1 Error.


#### URI Error
`INCORRECT USE OF URI FUNCTIONS`
If these characters are not escaped in URls, they will
cause an error: / ? & I : ;

#### Type Error
VALUE IS UNEXPECTED DATA TYPE
This is often caused by trying to use an object or
method that does not exist.


#### RangeError
NUMBER OUTSIDE OF RANGE
If you call a function using numbers outside of its
accepted range.



#### HOW TO DEAL WITH ERRORS
Now that you know what an error is and how the browser treats them, there are two things you can do with the errors.


1: DEBUG THE SCRIPT TO FIX ERRORS
If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.
You will find that the developer tools available in
every major modern browser will help you with
this task. In this chapter, you will learn about the
developer tools in Chrome and Firefox. (The tools in
Chrome are identical to those in Opera.)



2: HANDLE ERRORS GRACEFULLY
You can handle errors gracefully using try, catch,
throw, and f i na 1 ly statement s.
Sometimes, an error may occur in the script for a
reason beyond your control. For example, you might
request data from a third party, and their server
may not respond. In such cases, it is particularly
important to write error-handling code.



### A DEBUGGING WORKFLOW
Debugging is about deduction: eliminating potential causes of an error. Here is a workflow for techniques you will meet over the next 20 pages.
Try to narrow down where the problem might be, then look for clues.


##### WHAT EXACTLY IS THE PROBLEM?
Once you think that you might know the rough area
in which your problem is located, you can then try to
find the actual line of code that is causing the error.
1. When you have set breakpoints, you can see if the
variables around them have the values you would
expect them to. If not, look earlier in the script.
2. Break down I break out parts of the code to test
smaller pieces of the functionality.



#### BROWSER DEV TOOLS & JAVASCRIPT CONSOLE
The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.

### CHROME/ OPERA
On a PC, press the F12 key or:
1. Go to the options menu (or three line menu icon)
2. Select Toots or More tools.
3. Select JavaScript Console or Developer Tools
On a Mac press Alt + Cmd + J. Or:
4. Go to the View menu.
5. Select Developer.
6. Open the JavaScript Console or Developer Tools
option and select Console.


### INTERNET EXPLORER
Press the F12 key or:
1. Go to the settings menu in the top-right.
2. Select developer tools.


### HOW TO LOOK AT ERRORS IN CHROME
The console will show you when there is an
error in your JavaScript. It also displays the line
where it became a problem for the interpreter.


#### LOGGING DATA TO THE CONSOLE
`This example shows several uses`
`of the console . log () method.`
1. The first line is used to indicate
the script is running.
2. Next an event handler waits
for the user leaving a text input,
and logs the va lue that they
entered into that form field.

`When the user submits the form,`
`four values are displayed:`
3. That the user clicked submit
4. The value in the width input
5. The value in the height input
6. The value of the area variable
They help check that you are
getting the values you expect.

The console . log() method
can write several values to the
console at the same t ime, each
separated by a comma, as shown
when displaying the height (5).
You should always remove this
kind of error handling code from
your script before you use it on
a live site.

#### MORE CONSOLE METHODS
To differentiate between the
types of messages you write
to the console, you can use
three different methods. They
use various colors and icons to
distinguish them.
1. conso1e.info() can be used
for general information
2. console.warn() can be used
for warnings
3. console.error () can be used
to hold errors


#### GROUPING MESSAGES
1. If you want to write a set of
related data to the console, you
can use the console. group ()
method to group the messages
together. You can then expand
and contract the results.

2. When you have finished
writing out the results for the
group, to indicate the end of the
group the console .groupEnd ()
method is used.


#### WRITING TABULAR DATA
In browsers that support it, the
console. table () method lets
you output a table showing:
• objects
• arrays that contain other objects or arrays

#### WRITING ON A CONDITION
Using the console. assert()
method, you can test if a
condition is met, and write to the
console only if the expression
evaluates to false.

1. Below, when users leave an
input, the code checks to see if
they entered a value that is 10
or higher. If not, it will write a
message to the screen.

2. The second check looks to
see if the calculated area is a
numeric value. If not, then the
user must have entered a value
that was not a number.


### STEPPING THROUGH CODE
If you set multiple breakpoints, you can step
through them one-by-one to see where values
change and a problem might occur.

#### CONDITIONAL BREAKPOINTS
You can indicate that a breakpoint should be
triggered only if a condition that you specify is
met. The condition can use existing variables.


#### DEBUGGER KEYWORD
You can create a breakpoint
in your code using just the
debugger keyword. When the
developer tools are open, this
will automatically create a
breakpoint.

### HANDLING EXCEPTIONS
`TRY`
First, you specify the code
that you t hink might throw an
exception within the try block.
`CATCH`
If the try code block throws an
exception, catch steps in with an
alternative set of code.
`FINALLY`
The contents of the fi na 11 y
code block will run either
way - whether the try block
succeeded or failed.

### THROWING ERRORS
If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.


#### THROW ERROR FOR NaN
If you try to use a string in a mathematical operation (other
than in addition), you do not get an error, you get a special value called NaN (not a number).


#### DEBUGGING TIPS
Here are a selection of practical tips that you
can try to use when debugging your scripts.


`ANOTHER BROWSER`
Some problems are browserspecific.
Try the code in another browser to see which ones are
causing a problem.
`ADD NUMBERS`
Write numbers to the console so you can see which the items
get logged. It shows how far your code runs before errors stop it.
`STRIP IT BACK`
Remove parts of code, and strip it down to the minimum you
need. You can do this either by removing the code altogether.


#### COMMON ERRORS
Here is a list of common errors you might find with your scripts.

`GO BACK TO BASICS`
JavaScript is case sensitive so
check your capitalization.
If you did not use var to declare
the variable, it will be a global
variable, and its value could be
overwritten elsewhere (either in
your script or by another script
that is included in the page).

`MISSED/ EXTRA CHARACTERS`
Every statement should end in a semicolon.
Check that there are no missing closing braces } or
parentheses ) .
Check that there are no commas inside a , } or , ) by accident.


## SUMMARY
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQy9NbA-Zt-phR7EyXXam4uUnQNTGCr7uS5cQ&usqp=CAU)
`If you understand execution contexts (which have two`
`stages) and stacks, you are more likely to find the error`
`in your code.`
Debugging is the process of finding errors. It involves a
process of deduction.
`The console helps narrow down the area in which the`
`error is located, so you can try to find the exact error.`
JavaScript has 7 different types of errors. Each creates
its own error object, which can tell you its line number
and gives a description of the error.
`If you know that you may get an error, you can handle`
`it gracefully using the try, catch, finally statements.`
`Use them to give your users helpful feedback.`







