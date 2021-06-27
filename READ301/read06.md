# Node.js
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQi-DkfxsdUNsrEDMIPIaqvCnxoDxkLtZxvVw&usqp=CAU)
## Things I want to know more about

#### What Is Node.js?
Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.

`Node Is Built on Google Chrome’s V8 JavaScript Engine`
The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi. It was designed with performance in mind and is responsible for compiling JavaScript directly to native machine code that your computer can execute.

However, when we say that Node is built on the V8 engine, we don’t mean that Node programs are executed in a browser. They aren’t. Rather, the creator of Node (Ryan Dahl) took the V8 engine and enhanced it with various features, such as a file system API, an HTTP library, and a number of operating system–related utility methods.

This means that Node.js is a program we can use to execute JavaScript on our computers. In other words, it’s a JavaScript runtime.

#### How Do I Install Node.js?
In this next section, we’ll install Node and write a couple of simple programs. We’ll also look at npm, a package manager that comes bundled with Node.


#### Node Binaries vs Version Manager
Many websites will recommend that you head to the official Node download page and grab the Node binaries for your system. While that works, I would suggest that you use a version manager instead. This is a program that allows you to install multiple versions of Node and switch between them at will. There are various advantages to using a version manager. For example, it negates potential permission issues when using Node with npm and lets you set a Node version on a per-project basis.

If you fancy going the version manager route, please consult our quick tip: Install Multiple Versions of Node.js using nvm. Otherwise, grab the correct binaries for your system from the link above and install those.


**“Hello, World!” the Node.js Way**
You can check that Node is installed on your system by opening a terminal and typing node -v. If all has gone well, you should see something like v12.14.1 displayed. This is the current LTS version at the time of writing.


#### Node.js Has Excellent Support for Modern JavaScript

As can be seen on this compatibility table, Node has excellent support for ECMAScript 2015 (ES6) and beyond. As you’re only targeting one runtime (a specific version of the V8 engine), this means that you can write your JavaScript using the latest and most modern syntax. It also means that you don’t generally have to worry about compatibility issues — as you would if you were writing JavaScript that would run in different browsers.

To illustrate the point, here’s a second program that makes use of several modern JavaScript features, such as tagged template literals, object destructuring and Array.prototype.flatMap().

#### Introducing npm, the JavaScript Package Manager
As I mentioned earlier, Node comes bundled with a package manager called npm. To check which version you have installed on your system, type npm -v.

In addition to being the package manager for JavaScript, npm is also the world’s largest software registry. There are over 1,000,000 packages of JavaScript code available to download, with billions of downloads per week. Let’s take a quick look at how we would use npm to install a package.


**Installing a Package Globally**
Open your terminal and type the following:
`npm install -g jshint`

**This will install the jshint package globally on your system. We can use it to lint the index.js file from the previous example:**
`jshint index.js`

You should now see a number of ES6-related errors. If you want to fix them up, add ``/* jshint esversion: 6 */`` to the top of the index.js file, re-run the command and linting should pass.

**Installing a Package Locally**
We can also install packages locally to a project, as opposed to globally, on our system. Create a test folder and open a terminal in that directory. Next type this:

``npm init -y``
This will create and auto-populate a package.json file in the same folder. Next, use npm to install the lodash package and save it as a project dependency:

`npm install lodash --save`

Create a file named test.js and add the following:
`const _ = require('lodash');`
`const arr = [0, 1, false, 2, '', 3];`
`console.log(_.compact(arr));`

Finally, run the script using `node test.js`. You should see [ 1, 2, 3 ] output to the terminal.

#### What Is Node.js Used For?
Now that we know what Node and npm are and how to install them, we can turn our attention to the first of their common uses: installing (via npm) and running (via Node) various build tools — designed to automate the process of developing a modern JavaScript application.

These build tools come in all shapes and sizes, and you won’t get far in a modern JavaScript landscape without bumping into them. They can be used for anything from bundling your JavaScript files and dependencies into static assets, to running tests, or automatic code linting and style checking.


#### What Are the Advantages of Node.js?
Aside from speed and scalability, an often-touted advantage of using JavaScript on a web server — as well as in the browser — is that your brain no longer needs to switch modes. You can do everything in the same language, which, as a developer, makes you more productive (and hopefully, happier). For example, you can easily share code between the server and the client.

Another of Node’s big pluses is that it speaks JSON. JSON is probably the most important data exchange format on the Web, and the lingua franca for interacting with object databases (such as MongoDB). JSON is ideally suited for consumption by a JavaScript program, meaning that when you’re working with Node, data can flow neatly between layers without the need for reformatting. You can have one syntax from browser to server to database.

## Conclusion
JavaScript is everywhere, and Node is a vast and expansive subject. Nonetheless, I hope that in this article I’ve offered you the beginner-friendly, high-level look at Node.js and its main paradigms that I promised at the beginning. I also hope that when you re-read the definitions we looked at previously, things will make a lot more sense.

Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.

# Pair Programming
#### How does pair programming work?
While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

#### Why pair program?
While learning to code, developers likely study several programming languages. Similar to a foreign language class, there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful

Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

During a five-hour paired lab session, Code Fellows students work on all four of these language-specific skills. The abilities they foster will serve them well in completing assignments, in their own communication and learning, in interviews, and in readiness for a job at a company that utilizes this agile practice.

**1. Greater efficiency**
It is a common misconception that pair programming takes a lot longer and is less efficient. In reality, when two people focus on the same code base, it is easier to catch mistakes in the making. Research indicates that pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging (let alone exposing users to a broken product). So, in the long-run, it’s often actually more efficient than two people working on separate features. When coming up with ideas and discussing solutions out loud, two programmers may come to a solution faster than one programmer on their own. Also, when the pair is stuck, both programmers can research the problem and reach a solution faster. Researches also identified pairing enhances technical skills, team communication, and even enjoyability of coding in the workplace.

**2. Engaged collaboration**
When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone. It is harder to procrastinate or get off track when someone else is relying on you to complete the work. Popping open your Facebook timeline is just that less enticing when someone else is looking at your screen.

Another important aspect of learning to program is knowing when to ask for help. We advise our students to spend no more than fifteen minutes stuck on a problem before asking a teaching assistant or instructor for help. When developers pair program, they rely more on each other and can often find a solution together without needing to ask for additional help. Ultimately, this boosts overall confidence.

**3. Learning from fellow students**
Everyone has a different approach to problem solving; working with a teammate can expose developers to techniques they otherwise would not have thought of. If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution.

Often times, the developers in a pairing have different skill sets. If one programmer is more experienced in a certain skill, they can teach a student who is less familiar with that area. The less experienced developer benefits from the experienced developer’s knowledge and guidance, and the latter benefits from explaining the topic in their own words, further solidifying their own understanding.

**4. Social skills**
Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities. Pair programming not only improves programming skills, but can also help programmers develop their interpersonal skills. When just grabbing the keyboard and taking over isn’t an option, getting good at finding the right words is a skill unto itself.

This has long-term career impacts. As much as employers want strong programmers, they know it’s essential to hire people who can work well with others.

**5. Job interview readiness**
A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen. They will carry out exercises together, such as code challenges, building a project or feature, or debugging an existing code base. By doing so, companies can get a better feel for how an applicant will fit into the team and their collaboration style.

For most roles, the ability to work with and learn from others and stellar communication skills are as (or more!) important to a company than specific technical skills. Pair programming strengthens all of those skills.

**6. Work environment readiness**
Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.