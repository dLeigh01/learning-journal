# Dynamic Web Pages With JavaScript
## How Do I Write Script for a Web Page?
### How HTML CSS & JavaScript Fit Together
When coding a site, there are three main languages that will build on top of each other to create the site. These should be confined to their own files to keep them separate whenever possible.
* Content Layer -.html files
    * This is where the content of the page lives and the structure is defined
* Presentation Layer -.css files
    * This creates rules telling the HTML page how to look
* Behavior Layer -.js files
    * This changes how the page behaves and adds interactivity
### Progressive Enhancement
With more and more different devices in existence it is hard to be sure your site will work for everyone, so you should design it in order.
* HTML only
    * Allows you to focus on the content of the site at the start and should be accessible to most users
* HTML + CSS
    * Adding css in a separate file keeps the rules away from the page itself and the same sheet can be used for the whole site, making it easier to maintain
* HTML + CSS + JavaScript
    * JS is added last as a way to enhance the usability of the page. Keeping it separate means the page will still function without it.
### How to Use Objects & Methods
`document.write('Good afternoon!');` is known as calling a method of an object. `document` refers to the whole page and is the object, `.` is a member operator, allowing you to access members of the object, `write()` is the method of the document object which allows new content to be written where the `<script>` command is, and `'Good afternoon!'` is the parameter, letting the write() method know what to put on the page.
### JavaScript runs where it is Found in the HTML
When the browser encounters a `<script>` element, it stops to load it.
## Basic JavaScript Instructions
### Statements
A script is a series of instructions that a computer can follow one-by-one. Each individual instruction is called a statement.
### Comments
You should write comments to explain what your code does. it makes it easier to understand by yourself and others
### What is a Variable?
A variable is a way for scripts to temporarily store data. They can be declared using the command `var /name/;` and once it has been created you can assign it a value using the command `/name/ = /content/`
### Data Types
JavaScript distinguishes between numbers, strings, and booleans.
* Numeric data handles numbers.
* String data consists of letters and other characters between apostrophes.
* Boolean data can have a value of either true or false.
### Changing the Value of a Variable
Once a value has been assigned, you can change that value later in the same script using the variable name, equals sign, and the new value.
### Rules for Naming Variables
* The name must begin with a letter, dollar sign, or underscore
* The name can only contain letters, dollar signs, or underscores
* You cannot use keywords or reserved words
* All variables are case sensitive
* Use a name that describes the information being stored
* If there is more than one word in the name, use camelBack

[back](README.md)