**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=embed-javascript-code-in-an-html-file)**

**Javascript**

**What You Can Do with JavaScript**

There are lot more things you can do with JavaScript.

- You can modify the content of a web page by adding or removing elements.
  - You can change the style and position of the elements on a web page.
    - You can monitor events like mouse click, hover, etc. and react to it.
- You can perform and control transitions and animations.
  - You can create alert pop-ups to display info or warning messages to the user.
- You can perform operations based on user inputs and display the results.
  - You can validate user inputs before submitting it to the server.

**Adding JavaScript to Your Web Pages**

There are typically three ways to add JavaScript to a web page:

- Embedding the JavaScript code between a pair of <script> and </script> tag.
  - Creating an external JavaScript file with the .js extension and then load it within the page through the src attribute of the <script> tag.
    - Placing the JavaScript code directly inside an HTML tag using the special tag attributes such as onclick , onmouseover , onkeypress , onload , etc.

The following sections will describe each of these procedures in detail:

**Embedding the JavaScript Code**

You can embed the JavaScript code directly within your web pages by placing it between the <script> and </script> tags. The <script> tag indicates the browser that the contained statements are to be interpreted as executable script and not HTML. Here's an example:

<!DOCTYPE html>![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.001.png)

<html lang="en">

<head>

<meta charset="UTF-8">

<title>Embedding JavaScript</title>

</head>

<body>

<script>

let greet = "Hello World!"; document.write(greet); // Prints: Hello World! </script>

</body>

</html>

The JavaScript code in the above example will simply prints a text message on the web page. You will learn what each of these JavaScript statements means in upcoming chapters.

**Note:**The type attribute for <script> tag (i.e. <script type="text/javascript"> ) is no longer required since HTML5. JavaScript is the default scripting language for HTML5.![ref1]

**Calling an External JavaScript File**

You can also place your JavaScript code into a separate file with a .js extension, and then call that file in your document through the src attribute of 

the <script> tag, like this:

<scriptsrc="js/hello.js"></script>

This is useful if you want the same scripts available to multiple documents. It saves you from repeating the same task over and over again, and makes your website much easier to maintain.

Well, let's create a JavaScript file named "hello.js" and place the following code in it:

// A function to display a message ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.003.png)function sayHello() {

alert("Hello World!");

}

// Call function on click of the button document.getElementById("myBtn").onclick = sayHello;

Now, you can call this external JavaScript file within a web page using the <script> tag, like this:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=call-an-external-javascript-file-in-a-html-document)**

<!DOCTYPE html>![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.004.png)

<html lang="en">

<head>

<meta charset="UTF-8"> <title>Including External JavaScript File</title> </head>

<body>

<button type="button" id="myBtn">Click Me</button> <script src="js/hello.js"></script>

</body>

</html>

**Note:**Usually when an external JavaScript file is downloaded for first time, it is stored in the browser's cache (just like images and style sheets), so it won't need to be downloaded multiple times from the web server that makes the web pages load more quickly.![ref1]

**Placing the JavaScript Code Inline**

You can also place JavaScript code inline by inserting it directly inside the HTML tag using the special tag attributes such as onclick , onmouseover , onkeypress , onload , 

Ja vascr ipt 3

etc.

However, you should avoid placing large amount of JavaScript code inline as it clutters up your HTML with JavaScript and makes your JavaScript code difficult to maintain. Here's an example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=insert-javascript-code-inside-html-tag)**

<!DOCTYPE html>![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.005.png)

<html lang="en">

<head>

<meta charset="UTF-8">

<title>Inlining JavaScript</title>

</head>

<body>

<button onclick="alert('Hello World!')">Click Me</button></bo dy>

</html>

The above example will show you an alert message on click of the button element.

**Tip:**You should always keep the content and structure of your web page (i.e. HTML separate out from presentation CSS, and behavior JavaScript).![ref1]

**Positioning of Script inside HTML Document**

The <script> element can be placed in the <head> , or <body> section of an HTML document. But ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.006.png)ideally, scripts should be placed at the end of the body section, just before the closing </body> tag, it will make your web pages load faster, since it prevents obstruction of initial page rendering.

Each <script> tag blocks the page rendering process until it has fully downloaded and executed the JavaScript code, so placing them in the head section 

(i.e. <head> element) of the document without any valid reason will significantly impact your website performance.

Ja vascr ipt 4

**Tip:**You can place any number of <script> element in a single document. However, they are processed in the order in which they appear in the document, from top to bottom.![ref1]

**Difference Between Client-side and Server-side Scripting**

Client-side scripting languages such as JavaScript, VBScript, etc. are interpreted and executed by the web browser, while server-side scripting languages such as PHP, ASP, Java, Python, Ruby, etc. runs on the web server and the output sent back to the web browser in HTML format.

Client-side scripting has many advantages over traditional server-side scripting approach. For example, you can use JavaScript to check if the user has entered invalid data in form fields and show notifications for input errors accordingly in real-time before submitting the form to the web-server for final data validation and further processing in order to prevent unnecessary network bandwidth usages and the exploitation of server system resources.

Also, response from a server-side script is slower as compared to a client-side script, because server-side scripts are processed on the remote computer not on the user's local computer.

You can learn more about server-side scripting inPHP tutor[ialsection. ](https://www.tutorialrepublic.com/php-tutorial/)**JavaScript Syntax**

In this tutorial you will learn how to write the JavaScript code.

**Understanding the JavaScript Syntax**

The syntax of JavaScript is the set of rules that define a correctly structured JavaScript program.

A JavaScript consists of JavaScript statements that are placed within the ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.007.png)<script> </script> HTML tags in a web page, or within the external JavaScript file ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.008.png)

having .js extension.

The following example shows how JavaScript statements look like: **Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=statements)**

let x = 5;![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.009.png)

let y = 10;

let sum = x + y;

document.write(sum); // Prints variable value

You will learn what each of these statements means in upcoming chapters.![ref1]

**Case Sensitivity in JavaScript**

JavaScript is case-sensitive. This means that variables, language keywords, function names, and other identifiers must always be typed with a consistent capitalization of letters.

For example, the variable myVar must be typed myVar not MyVar or myvar . Similarly, the method name![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.010.png) getElementById() must be typed with the exact case not 

as getElementByID() .

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=case-sensitivity)**

let myVar = "Hello World!"; ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.011.png)console.log(myVar); console.log(MyVar); console.log(myvar);

If you checkout the browser console by pressing the f12 key on the keyboard, you'll see a line something like this: "Uncaught ReferenceError: MyVar is not defined".![ref2]

**JavaScript Comments**

A comment is simply a line of text that is completely ignored by the JavaScript interpreter. Comments are usually added with the purpose of providing extra information pertaining to source code. It will not only help you understand your code when you look after a period of time but also others who are working with you on the same project.

JavaScript support single-line as well as multi-line comments. Single-line comments begin with a double forward slash ( // ), followed by the comment text. Here's an example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=single-line-comment)**

// This is my first JavaScript program ![ref3]document.write("Hello World!");

Whereas, a multi-line comment begins with a slash and an asterisk ( /\* ) and ends with an asterisk and slash ( \*/ ). Here's an example of a multi-line comment.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=multi-line-comment)**

/\* This is my first program![ref4]

in JavaScript \*/ document.write("Hello World!");

**JavaScript Variables**

In this tutorial you will learn how to create variables to store data in JavaScript.

**What is Variable?**

Variables are fundamental to all programming languages. Variables are used to store data, like string of text, numbers, etc. The data or value stored in the variables can be set, updated, and retrieved whenever needed. In general, variables are symbolic names for values.

There are three ways to declare variables in JavaScript: var , let and const . The var keyword is the older way of declaring variables, whereas 

the let and const keywords are introduced inJavaScr[ipt ES6. The main](https://www.tutorialrepublic.com/javascript-tutorial/javascript-es6-features.php) ![ref5]difference between them is the variables declared with 

the let and const keywords are**block scoped**( {} ), that means they will only be ![ref5]

available inside the code blocks ([functions,loopsand](https://www.tutorialrepublic.com/javascript-tutorial/javascript-functions.php)[conditions](https://www.tutorialrepublic.com/javascript-tutorial/javascript-loops.php))[ where they ar](https://www.tutorialrepublic.com/javascript-tutorial/javascript-if-else-statements.php)e declared and it sub-blocks, whereas the variables declared with the var keyword are**function scoped**or**globally scoped**, depending on whether they are declared within a function or outside of any function.

We'll learn more about them in upcoming chapters. Now let's take a look at the following example where we've created some variables with the let keyword, and simply used the assignment operator ( = ) to assign values to them, like this: let ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.016.png)

varName = value; ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.017.png)

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=create-variables)**

let name = "Peter Parker"; ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.018.png)let age = 21;

let isMarried = false;

**Tip:**Always give meaningful names to your variables. Additionally, for naming the variables that contain multiple words, camelCase is commonly used. In this convention all words after the first should have uppercase first letters, 

e.g. myLongVariableName .

In the above example we have created three variables, first one has assigned with a string value, the second one has assigned with a number, whereas the last one assigned with a boolean value. Variables can hold different types of data, we'll learn about them in later chapter.

In JavaScript, variables can also be declared without having any initial values assigned to them. This is useful for variables which are supposed to hold values like user inputs.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=declare-variables)**

// Declaring Variable ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.019.png)let userName;

// Assigning value userName = "Clark Kent";

**Note:**In JavaScript, if a variable has been declared, but has not been assigned a value explicitly, is automatically assigned the value undefined .

The const keyword works exactly the same as let , except that variables declared using const keyword cannot be reassigned later in the code. Here's an example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=declare-constants)**

// Declaring constant ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.020.png)const PI = 3.14; console.log(PI); // 3.14

// Trying to reassign PI = 10; // error

**Note:**The let and const keywords are not supported in older browsers like IE10. IE11 support them ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.021.png)partially. See theJS [ES6 featureschapter t](https://www.tutorialrepublic.com/javascript-tutorial/javascript-es6-features.php)o know how to start using ES6 today.![ref1]

**Declaring Multiple Variables at Once**

In addition, you can also declare multiple variables and set their initial values in a single statement. Each variable are separated by commas, as demonstrated in the following example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=declare-multiple-variables)**

// Declaring multiple Variables![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.022.png)

let name = "Peter Parker", age = 21, isMarried = false;

/\* Longer declarations can be written to span multiple lines to improve the readability \*/ let name = "Peter Parker",

age = 21,

isMarried = false;![ref2]

**Naming Conventions for JavaScript Variables**

These are the following rules for naming a JavaScript variable:

- A variable name must start with a letter, underscore ( \_ ), or dollar sign ( $ ).
  - A variable name cannot start with a number.
    - A variable name can only contain alpha-numeric characters ( A-z , 0-9 ) and underscores.
- A variable name cannot contain spaces.
  - A variable name cannot be a JavaScript keyword or aJavaScript[ reserved word.](https://www.tutorialrepublic.com/javascript-reference/javascript-reserved-keywords.php)

**Note:**Variable names in JavaScript are case sensitive, it 

means $myvar and $myVar are two different variables. So be careful while defining variable names.

**JavaScript Generating Output**

In this tutorial you will learn how to generate outputs in JavaScript.

**Generating Output in JavaScript**

There are certain situations in which you may need to generate output from your JavaScript code. For example, you might want to see the value of variable, or write a message to browser console to help you debug an issue in your running JavaScript code, and so on.

In JavaScript there are several different ways of generating output including writing output to the browser window or browser console, displaying output in dialog boxes, writing output into an HTML element, etc. We'll take a closer look at each of these in the following sections.

**Writing Output to Browser Console**

You can easily outputs a message or writes data to the browser console using the console.log() method. This is a simple, but very powerful method for generating detailed output. Here's an example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=write-into-the-browser-console)**

// Printing a simple text message ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.023.png)console.log("Hello World!"); // Prints: Hello World!

// Printing a variable value let x = 10;

let y = 20;

let sum = x + y; console.log(sum); // Prints: 30

**Tip:**To access your web browser's console, first pressF12key on the keyboard to open the*developer tools*then click on the console tab. It looks something like the[screenshot here.](https://www.tutorialrepublic.com/lib/images/chrome-browser-console.png)![ref1]

**Displaying Output in Alert Dialog Boxes**

You can also use alert dialog boxes to display the message or output data to the user. An alert dialog box is created using the alert() method. Here's is an example:![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.024.png)

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=write-into-an-alert-dialog-box)**

// Displaying a simple text message ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.025.png)alert("Hello World!"); // Outputs: Hello World!

// Displaying a variable value let x = 10;

let y = 20;

let sum = x + y;

alert(sum); // Outputs: 30![ref2]

**Writing Output to the Browser Window**

You can use the document.write() method to write the content to the current document only while that document is being parsed. Here's an example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=write-into-the-browser-window)**

// Printing a simple text message ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.026.png)document.write("Hello World!"); // Prints: Hello World!

// Printing a variable value

let x = 10;

let y = 20;

let sum = x + y; document.write(sum); // Prints: 30

If you use the document.write() method method after the page has been loaded, it will overwrite all the existing content in that document. Check out the following example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=problem-with-document-write-method)**

<h1>This is a heading</h1><p>This is a paragraph of text.</p> ![ref4]<button type="button" onclick="document.write('Hello Worl d!')">Click Me</button>![ref1]

**Inserting Output Inside an HTML Element**

You can also write or insert output inside an HTML element using the

element's innerHTML property. However, before writing the output first we need to[select the elementusing](https://www.tutorialrepublic.com/javascript-tutorial/javascript-dom-selectors.php) a method such as getElementById() , as demonstrated in the following example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=write-into-an-html-element)**

<p id="greet"></p><p id="result"></p><script> ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.027.png)// Writing text string inside an element

document.getElementById("greet").innerHTML = "Hello World!";![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.028.png)

// Writing a variable value inside an element

let x = 10;

let y = 20;

let sum = x + y; document.getElementById("result").innerHTML = sum; </script>

**JavaScript Data Types**

In this tutorial you will learn about the data types available in JavaScript. **Data Types in JavaScript**

Data types basically specify what kind of data can be stored and manipulated within a program.

There are six basic data types in JavaScript which can be divided into three main categories: primitive (or*primary*),*composite*(or*reference*), and*special*data types. String, Number, and Boolean are primitive data types. Object, Array, and Function (which are all types of objects) are composite data types. Whereas Undefined and Null are special data types.

Primitive data types can hold only one value at a time, whereas composite data types can hold collections of values and more complex entities. Let's discuss each one of them in detail.

**The String Data Type**

The*string*data type is used to represent textual data (i.e. sequences of characters). Strings are created using single or double quotes surrounding one or more characters, as shown below:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=string-data-type)**

let a = 'Hi there!';  // using single quotes ![ref3]let b = "Hi there!";  // using double quotes

You can include quotes inside the string as long as they don't match the enclosing quotes.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=include-quotes-inside-the-string)**

let a = "Let's have a cup of coffee."; // single quote inside double quotes![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.029.png)

let b = 'He said "Hello" and left.';  // double quotes inside single quotes

let c = 'We\'ll never give up.';     // escaping single quote with backslash

You will learn more about the strings inJav[aScript stringschapter.](https://www.tutorialrepublic.com/javascript-tutorial/javascript-strings.php)![ref1]

**The Number Data Type**

The*number*data type is used to represent positive or negative numbers with or without decimal place, or numbers written using exponential notation e.g. 1.5e-4 (equivalent to 1.5104.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=number-data-type)**

let a = 25;         // integer![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.030.png)

let b = 80.5;       // floating-point number

let c = 4.25e+6;    // exponential notation, same as 4.25e6 o r 4250000

let d = 4.25e-6;    // exponential notation, same as 0.000004 25

The Number data type also includes some special values which are: Infinity , ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.031.png)- Infinity and NaN . Infinity represents the mathematical Infinity ∞ , which is greater than any number. Infinity is the result of dividing a nonzero number by 0, as demonstrated below:![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.032.png)

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=infinity)**

alert(16 / 0);  // Output: Infinity ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.033.png)alert(-16 / 0); // Output: -Infinity alert(16 / -0); // Output: -Infinity

While NaN represents a special*Not-a-Number*value. It is a result of an invalid or an undefined mathematical operation, like taking the square root of 1 or dividing 0 by 0, etc.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=not-a-number)**

alert("Some text" / 2);       // Output: NaN ![ref4]alert("Some text" / 2 + 10);  // Output: NaN alert(Math.sqrt(-1));         // Output: NaN

You will learn more about the numbers inJavaScr[ipt numberschapter.](https://www.tutorialrepublic.com/javascript-tutorial/javascript-numbers.php)![ref1]

**The Boolean Data Type**

The Boolean data type can hold only two values: true or false . It is typically used to store values like yes ( true ) or no ( false ), on ( true ) or off ( false ), etc. as demonstrated below:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=boolean-data-type)**

let isReading = true;   // yes, I'm reading![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.034.png)

let isSleeping = false; // no, I'm not sleeping

Boolean values also come as a result of comparisons in a program. The following example compares two variables and shows the result in an alert dialog box:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=comparisons)**

let a = 2, b = 5, c = 10;![ref6]

alert(b > a) // Output: true ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.036.png)alert(b > c) // Output: false

You will learn more about the comparisons inJavaScr[ipt if/elsechapter.](https://www.tutorialrepublic.com/javascript-tutorial/javascript-if-else-statements.php)![ref1]

**The Undefined Data Type**

The undefined data type can only have one value-the special value undefined . If a variable has been declared, but has not been assigned a value, has the

value undefined .

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=undefined-data-type)**

let a;![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.037.png)

let b = "Hello World!";

alert(a) // Output: undefined alert(b) // Output: Hello World!![ref2]

**The Null Data Type**

This is another special data type that can have only one value-the null value. A null value means that there is no value. It is not equivalent to an empty string ( "" ) or 0, it is simply nothing.

A variable can be explicitly emptied of its current contents by assigning it the null value.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=null-data-type)**

let a = null;![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.038.png)

alert(a); // Output: null

let b = "Hello World!";

alert(b); // Output: Hello World!

b = null;![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.039.png)

alert(b) // Output: null![ref1]

**The Object Data Type**

The object is a complex data type that allows you to store collections of data.

An object contains properties, defined as a key-value pair. A property key (name) is always a string, but the value can be any data type, like strings, numbers, booleans, or complex data types like arrays, function and other objects. You'll learn more about objects in upcoming chapters.

The following example will show you the simplest way to create an object in JavaScript.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=object-data-type)**

let emptyObject = {};![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.040.png)

let person = {"name": "Clark", "surname": "Kent", "age": "3 6"};

// For better reading let car = {

"modal": "BMW X3", "color": "white", "doors": 5

}

You can omit the quotes around property name if the name is a valid JavaScript name. That means quotes are required around "first-name" but are optional around firstname . So the car object in the above example can also be written as:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=object-properties-names-without-quotes)**

let car = {![ref6]

modal: "BMW X3", color: "white",

doors: 5![ref7]

}

You will learn more about the objects inJavaScr[ipt objectschapter.](https://www.tutorialrepublic.com/javascript-tutorial/javascript-objects.php)![ref1]

**The Array Data Type**

An array is a type of object used for storing multiple values in single variable. Each value (also called an element) in an array has a numeric position, known as its index, and it may contain data of any data type-numbers, strings, booleans, functions, objects, and even other arrays. The array index starts from 0, so that the first array element is arr[0] not arr[1] .

The simplest way to create an array is by specifying the array elements as a comma-separated list enclosed by square brackets, as shown in the example below:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=array-data-type)**

let colors = ["Red", "Yellow", "Green", "Orange"]; ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.042.png)let cities = ["London", "Paris", "New York"];

alert(colors[0]);   // Output: Red alert(cities[2]);   // Output: New York

You will learn more about the arrays inJav[aScript arrayschapter.](https://www.tutorialrepublic.com/javascript-tutorial/javascript-arrays.php)![ref2]

**The Function Data Type**

The function is callable object that executes a block of code. Since functions are objects, so it is possible to assign them to variables, as shown in the example below:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=function-data-type)**

let greeting = function(){![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.043.png)

return "Hello World!";

}![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.044.png)

// Check the type of greeting variable alert(typeof greeting) // Output: function alert(greeting());     // Output: Hello World!

In fact, functions can be used at any place any other value can be used. Functions can be stored in variables, objects, and arrays. Functions can be passed as arguments to other functions, and functions can be returned from functions. Consider the following function:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=function-passed-as-argument-to-other-function)**

function createGreeting(name){![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.045.png)

return "Hello, " + name;

}

function displayGreeting(greetingFunction, userName){

return greetingFunction(userName);

}

let result = displayGreeting(createGreeting, "Peter"); alert(result); // Output: Hello, Peter

You will learn more about the functions inJavaScr[ipt functionschapter.](https://www.tutorialrepublic.com/javascript-tutorial/javascript-functions.php)![ref1]

**The typeof Operator**

The typeof operator can be used to find out what type of data a variable or operand contains. It can be used with or without parentheses ( typeof(x) or ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.046.png)typeof x ).![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.047.png)

The typeof operator is particularly useful in the situations when you need to process the values of different types differently, but you need to be very careful, because it may produce unexpected result in some cases, as demonstrated in the following example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=typeof-operator)**

// Numbers![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.048.png)

typeof 15;  // Returns: "number"

typeof 42.7;  // Returns: "number"

typeof 2.5e-4;  // Returns: "number"

typeof Infinity;  // Returns: "number"

typeof NaN;  // Returns: "number". Despite being "Not-A-Numbe r"

// Strings

typeof '';  // Returns: "string"

typeof 'hello';  // Returns: "string"

typeof '12';  // Returns: "string". Number within quotes is t ypeof string

// Booleans

typeof true;  // Returns: "boolean" typeof false;  // Returns: "boolean"

// Undefined

typeof undefined;  // Returns: "undefined"

typeof undeclaredVariable; // Returns: "undefined"

// Null

typeof Null;  // Returns: "object"

// Objects

typeof {name: "John", age: 18};  // Returns: "object" // Arrays

typeof [1, 2, 4];  // Returns: "object"

// Functions

typeof function(){};  // Returns: "function"

As you can clearly see in the above example when we test the null value using the typeof operator (*line no-22*), it returned "object" instead of "null".

This is a long-standing bug in JavaScript, but since lots of codes on the web written around this behavior, and thus fixing it would create a lot more problem, so idea of fixing this issue was rejected by the committee that design and maintains JavaScript.

**JavaScript Events**

In this tutorial you will learn how to handle events in JavaScript.

**Understanding Events and Event Handlers**

An event is something that happens when user interact with the web page, such as when he clicked a link or button, entered text into an input box or textarea, made selection in a select box, pressed key on the keyboard, moved the mouse pointer, submits a form, etc. In some cases, the Browser itself can trigger the events, such as the page load and unload events.

When an event occur, you can use a JavaScript event handler (or an event listener) to detect them and perform specific task or set of tasks. By convention, the names for event handlers always begin with the word "on", so an event handler for the click event is called onclick , similarly an event handler for the load event is called onload , event handler for the blur event is called onblur , and so on.

There are several ways to assign an event handler. The simplest way is to add them directly to the start tag of the HTML elements using the special event - handler attributes. For example, to assign a click handler for a button element, we can use onclick attribute, like this:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=attaching-event-handlers-inline)**

<button type="button" onclick="alert('Hello World!')">Click M e![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.049.png)</button>

However, to keep the JavaScript seperate from HTML, you can set up the event handler in an external JavaScript file or within the <script> and </script> tags, like 

this:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=attaching-event-handlers-in-an-external-file)**

<button type="button" id="myBtn">Click Me</button>![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.050.png)

<script>

function sayHello() {

alert('Hello World!');

}

document.getElementById("myBtn").onclick = sayHello; </script>

**Note:**Since HTML attributes are case-insensitive so onclick may also be written as onClick , OnClick or ONCLICK . But its*value*is case-sensitive.![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.051.png)

In general, the events can be categorized into four main groups —mouse [events,k](https://www.tutorialrepublic.com/javascript-tutorial/javascript-events.php#mouse-events)[eyboard events,form](https://www.tutorialrepublic.com/javascript-tutorial/javascript-events.php#keyboard-events) [eventsand](https://www.tutorialrepublic.com/javascript-tutorial/javascript-events.php#form-events)[document/window events. There are ](https://www.tutorialrepublic.com/javascript-tutorial/javascript-events.php#document-and-window-events)many other events, we will learn about them in later chapters. The following section will give you a brief overview of the most useful events one by one along with the real life practice examples.

**Mouse Events**

A mouse event is triggered when the user click some element, move the mouse pointer over an element, etc. Here're some most important mouse events and their event handler.

**The Click Event (onclick)**

Ja vascr ipt 22

The click event occurs when a user clicks on an element on a w these are form elements and links. You can handle a click e

an onclick event handler.

The following example will show you an alert message when y elements.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-click-event)**

eb page. Often, vent with 

ou click on the 

Ja vascr ipt 

<button type="button" onclick="alert('You have clicked a butt on!'![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.052.png));">Click Me</button>

<a href="#" onclick="alert('You have clicked a link!');">Clic k Me</a>

**The Contextmenu Event (oncontextmenu)**

Ja vascr ipt 

The contextmenu event occurs when a user clicks the r element to open a context menu. You can handle a cont an oncontextmenu event handler.

The following example will show an alert message when y elements.

ight mouse button on an extmenu event with 

ou right-click on the 

Ja vascr ipt 

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-contextmenu-event)**

<button type="button" oncontextmenu="alert('You have right-cl icked a button!');![ref8]">Right Click on Me</button>

<a href="#" oncontextmenu="alert('You have right-clicked a li nk!');">Right Click on Me</a>

**The Mouseover Event (onmouseover)**

The mouseover event occurs when a user moves the mouse pointer over an element.

You can handle the mouseover event with the onmouseover event handler. The following example will show you an alert message when you place mouse over the elements.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-mouseover-event)**

<button type="button" onmouseover="alert('You have placed mou se pointer over a button!'![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.054.png));">Place Mouse Over Me</button>

<a href="#" onmouseover="alert('You have placed mouse pointer over a link!'![ref9]);">Place Mouse Over Me</a>

**The Mouseout Event (onmouseout)**

The mouseout event occurs when a user moves the mouse pointer outside of an element.

You can handle the mouseout event with the onmouseout event handler. The following example will show you an alert message when the mouseout event occurs.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-mouseout-event)**

<button type="button" onmouseout="alert('You have moved out o f the button!'![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.056.png));">Place Mouse Inside Me and Move Out</button> <a href="#" onmouseout="alert('You have moved out of the lin k!');">Place Mouse Inside Me and Move Out</a>![ref10]

**Keyboard Events**

A keyboard event is fired when the user press or release a key on the keyboard. Here're some most important keyboard events and their event handler.

**The Keydown Event (onkeydown)**

The keydown event occurs when the user presses down a key on the keyboard.

You can handle the keydown event with the onkeydown event handler. The following example will show you an alert message when the keydown event occurs.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-keydown-event)**

<input type="text" onkeydown="alert('You have pressed a key i nside text input!'![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.058.png))">

<textarea onkeydown="alert('You have pressed a key inside tex tarea!'![ref7])"></textarea>

**The Keyup Event (onkeyup)**

The keyup event occurs when the user releases a key on the keyboard.

You can handle the keyup event with the onkeyup event handler. The following example will show you an alert message when the keyup event occurs.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-keyup-event)**

<input type="text" onkeyup="alert('You have released a key in side text input!'![ref8])">

<textarea onkeyup="alert('You have released a key inside text area!')"></textarea>

**The Keypress Event (onkeypress)**

The keypress event occurs when a user presses down a key on the keyboard that has a character value associated with it. For example, keys like Ctrl, Shift, Alt, Esc, Arrow keys, etc. will not generate a keypress event, but will generate a keydown and keyup event.

You can handle the keypress event with the onkeypress event handler. The following example will show you an alert message when the keypress event occurs.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-keypress-event)**

<input type="text" onkeypress="alert('You have pressed a key inside text input!')![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.059.png)">

<textarea onkeypress="alert('You have pressed a key inside te xtarea!')"></textarea>![ref1]

**Form Events**

A form event is fired when a form control receive or loses focus or when the user modify a form control value such as by typing text in a text input, select any option in a select box etc. Here're some most important form events and their event handler.

**The Focus Event (onfocus)**

The focus event occurs when the user gives focus to an element on a web page. You can handle the focus event with the onfocus event handler. The following 

example will highlight the background of text input in yellow color when it receives the focus.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-focus-event)**

<script>![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.060.png)

function highlightInput(elm){

elm.style.background = "yellow";

}

</script>

<input type="text" onfocus="highlightInput(this)"> <button type="button">Button</button>

**Note:**The value of this keyword inside an event handler refers to the element which has the handler on it (i.e. where the event is currently being delivered).

**The Blur Event (onblur)**

The blur event occurs when the user takes the focus away from a form element or a window.

You can handle the blur event with the onblur event handler. The following example will show you an alert message when the text input element loses focus.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-blur-event)**

<input type="text" onblur="alert('Text input loses focus!')"> ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.061.png)<button type="button">Submit</button>

To take the focus away from a form element first click inside of it then press the tab key on the keyboard, give focus on something else, or click outside of it.

**The Change Event (onchange)**

The change event occurs when a user changes the value of a form element.

You can handle the change event with the onchange event handler. The following example will show you an alert message when you change the option in the select box.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-change-event)**

<select onchange="alert('You have changed the selection!');"> <![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.062.png)option>Select</option>

<option>Male</option>

<option>Female</option>

</select>

**The Submit Event (onsubmit)**

The submit event only occurs when the user submits a form on a web page.

You can handle the submit event with the onsubmit event handler. The following example will show you an alert message while submitting the form to the server.![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.063.png)

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-submit-event)**

<form action="action.php" method="post" onsubmit="alert('Form data will be submitted to the server!'![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.064.png));">

<label>First Name:</label>

<input type="text" name="first-name" required><input type="su

bmit" value="Submit"> </![ref9]form>![ref1]

**Document/Window Events**

Events are also triggered in situations when the page has loaded or when user resize the browser window, etc. Here're some most important document/window events and their event handler.

**The Load Event (onload)**

The load event occurs when a web page has finished loading in the web browser.

You can handle the load event with the onload event handler. The following example will show you an alert message as soon as the page finishes loading.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-load-event)**

<body onload="window.alert('Page is loaded successfully!');"> ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.065.png)<h1>This is a heading</h1>

<p>This is paragraph of text.</p>

</body>

**The Unload Event (onunload)**

The unload event occurs when a user leaves the current web page.

You can handle the unload event with the onunload event handler. The following example will show you an alert message when you try to leave the page.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-unload-event)**

<body onunload="alert('Are you sure you want to leave this pa ge?'![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.066.png));">

<h1>This is a heading</h1>

<p>This is paragraph of text.</p> </![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.067.png)body>

**The Resize Event (onresize)**

The resize event occurs when a user resizes the browser window. The resize event also occurs in situations when the browser window is minimized or maximized.

You can handle the resize event with the onresize event handler. The following example will show you an alert message when you resize the browser window to a new width and height.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=handling-the-resize-event)**

<p id="result"></p><script>![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.068.png)

function displayWindowSize() {

let w = window.outerWidth;

let h = window.outerHeight;

let txt = "Window size: width=" + w + ", height=" + h;

document.getElementById("result").innerHTML = txt;

}

window.onresize = displayWindowSize;

</script>

**JavaScript Array Reference**

This chapter contains a brief overview of the properties and method of the global array object.

**The JavaScript Array Object**

The JavaScript Array object is a global object that is used in the construction of arrays. An array is a special type of variable that allows you to store multiple 

values in a single variable.

To learn more about Arrays, please check out theJavaScr[ipt arraychapter. ](https://www.tutorialrepublic.com/javascript-tutorial/javascript-arrays.php)**Array Properties**

The following table lists the standard properties of the Array object.



|Property|Description|
| - | - |
|length![ref11]|Sets or returns the number of elements in an array.|
|prototype![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.070.png)|Allows you to add new properties and methods to an Array object.|

**Note:**Every object in JavaScript has a constructor property that refers to the constructor function that was used to create the instance of that object.![ref1]

**Array Methods**

The following table lists the standard methods of the Array object.



|Method|Description|
| - | - |
|concat()![ref12]|Merge two or more arrays, and returns a new array.|
|copyWithin()![ref13]|Copies part of an array to another location in the same array and returns it.|
|entries()![ref14]|Returns a key/value pair Array Iteration Object.|
|every()![ref15]|Checks if every element in an array pass a test in a testing function.|
|fill()![ref16]|Fill the elements in an array with a static value.|
|filter()![ref17]|Creates a new array with all elements that pass the test in a testing function.|
|find()![ref18]|Returns the value of the first element in an array that pass the test in a testing function.|
|findIndex()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.078.png)|Returns the index of the first element in an array that pass the test in a testing function.|
|forEach()![ref19]|Calls a function once for each array element.|
|from()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.080.png)|Creates an array from an object.|



|includes()![ref20]|Determines whether an array includes a certain element.|
| - | - |
|indexOf()![ref21]|Search the array for an element and returns its first index.|
|isArray()![ref22]|Determines whether the passed value is an array.|
|join()![ref23]|Joins all elements of an array into a string.|
|keys()![ref24]|Returns a Array Iteration Object, containing the keys of the original array.|
|lastIndexOf()![ref25]|Search the array for an element, starting at the end, and returns its last index.|
|map()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.087.png)|Creates a new array with the results of calling a function for each array element.|
|pop()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.088.png)|Removes the last element from an array, and returns that element.|
|push()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.089.png)|Adds one or more elements to the end of an array, and returns the array's new length.|
|reduce()![ref26]|Reduce the values of an array to a single value (from left-to-right).|
|reduceRight()![ref27]|Reduce the values of an array to a single value (from right-to-left).|
|reverse()![ref22]|Reverses the order of the elements in an array.|
|shift()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.092.png)|Removes the first element from an array, and returns that element.|
|slice()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.093.png)|Selects a part of an array, and returns the new array.|
|some()![ref16]|Checks if any of the elements in an array passes the test in a testing function.|
|sort()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.094.png)|Sorts the elements of an array.|
|splice()![ref26]|Adds/Removes elements from an array.|
|toString()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.095.png)|Converts an array to a string, and returns the result.|
|unshift()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.096.png)|Adds new elements to the beginning of an array, and returns the array's new length.|
|values()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.097.png)|Returns a Array Iteration Object, containing the values of the original array.|

**JavaScript Boolean Reference**

This chapter contains a brief overview of the properties and method of the global Boolean object.

**The JavaScript Boolean Object**

The Boolean object is an object wrapper around the boolean value true or false . This Boolean object type exists primarily to provide a toString() method to convert boolean values to strings.

To learn more about the Boolean, please check out theJavaScript[ data typeschapt](https://www.tutorialrepublic.com/javascript-tutorial/javascript-data-types.php#boolean)er.

**Boolean Properties**

The following table lists the standard properties of the Boolean object.



|Property|Description|
| - | - |
|prototype![ref14]|Allows you to add new properties and methods to a Boolean object.|

**Note:**Every object in JavaScript has a constructor property that refers to the constructor function that was used to create the instance of that object.![ref2]

**Boolean Methods**

The following table lists the standard methods of the Boolean object.



|Method|Description|
| - | - |
|toString()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.098.png)|Converts a Boolean value to a string, and returns the result.|
|valueOf()![ref19]|Returns the primitive value of a Boolean object.|

**JavaScript Date Reference**

This chapter contains a brief overview of the properties and method of the global Date object.

**The JavaScript Date Object**

The JavaScript Date object is a global object that is used to work with dates and times. The Date objects are based on a time value that is the number of

milliseconds since January 1, 1970 UTC.

To learn more about the Date, please check out theJavaScript[ date and time](https://www.tutorialrepublic.com/javascript-tutorial/javascript-date-and-time.php)chapter.

**Date Properties**

The following table lists the standard properties of the Date object.



|Property|Description|
| - | - |
|prototype![ref14]|Allows you to add new properties and methods to a Date object.|

**Note:**Every object in JavaScript has a constructor property that refers to the constructor function that was used to create the instance of that object.![ref2]

**Date Methods**

The following table lists the standard methods of the Date object.



|Method|Description|
| - | - |
|getDate()![ref14]|Returns the day of the month (from 131.|
|getDay()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.099.png)|Returns the day of the week (from 06.|
|getFullYear()![ref25]|Returns the year (four digits).|
|getHours()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.100.png)|Returns the hour (from 023.|
|getMilliseconds()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.101.png)|Returns the milliseconds (from 0999.|
|getMinutes()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.102.png)|Returns the minutes (from 059.|
|getMonth()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.103.png)|Returns the month (from 011.|
|getSeconds()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.104.png)|Returns the seconds (from 059.|
|getTime()![ref14]|Returns the number of milliseconds since midnight Jan 1, 1970.|
|getTimezoneOffset()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.105.png)|Returns the time difference between UTC time and local time, in minutes.|
|getUTCDate()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.106.png)|Returns the day of the month, according to universal time (from 1 31.|



|getUTCDay()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.107.png)|Returns the day of the week, according to universal time (from 0 6.|
| - | :- |
|getUTCFullYear()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.108.png)|Returns the year, according to universal time.|
|getUTCHours()![ref28]|Returns the hour, according to universal time (from 023.|
|getUTCMilliseconds()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.110.png)|Returns the milliseconds, according to universal time (from 0999|
|getUTCMinutes()![ref29]|Returns the minutes, according to universal time (from 059.|
|getUTCMonth()![ref30]|Returns the month, according to universal time (from 011.|
|getUTCSeconds()![ref31]|Returns the seconds, according to universal time (from 059.|
|getYear()|Deprecated.Use the getFullYear() method instead.|
|now()![ref32]|Returns the number of milliseconds since midnight Jan 1, 1970.|
|parse()![ref15]|Parses a date string and returns the number of milliseconds since Jan 1, 1970.|
|setDate()![ref22]|Sets the day of the month of a date object.|
|setFullYear()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.115.png)|Sets the full year of a date object.|
|setHours()![ref20]|Sets the hours of a date object.|
|setMilliseconds()![ref33]|Sets the milliseconds of a date object.|
|setMinutes()![ref13]|Set the minutes of a date object.|
|setMonth()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.117.png)|Sets the month of a date object.|
|setSeconds()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.118.png)|Sets the seconds of a date object.|
|setTime()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.119.png)|Sets a date to a specified number of milliseconds after/before Jan 1, 1970.|
|setUTCDate()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.120.png)|Sets the day of the month of a date object, according to universal time.|
|setUTCFullYear()![ref34]|Sets the year of a date object, according to universal time.|
|setUTCHours()![ref30]|Sets the hours of a date object, according to universal time.|
|setUTCMilliseconds()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.122.png)|Sets the milliseconds of a date object, according to universal time.|
|setUTCMinutes()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.123.png)|Set the minutes of a date object, according to universal time.|
|setUTCMonth()![ref27]|Sets the month of a date object, according to universal time.|
|setUTCSeconds()![ref35]|Set the seconds of a date object, according to universal time.|
|setYear()![ref36]|Deprecated.Use the setFullYear() method instead.![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.126.png)|



|toDateString()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.127.png)|Converts the date portion of a Date object into a human readable form.|
| - | :- |
|toGMTString()![ref30]|Deprecated.Use thetoUTCString()method instead|
|toISOString()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.128.png)|Returns the date as a string, formatted according to ISO standard.|
|toJSON()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.129.png)|Returns the date as a string, formatted as a JSON date.|
|toLocaleDateString()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.130.png)|Returns the date portion of a Date object as a locally formatted string.|
|toLocaleTimeString()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.131.png)|Returns the time portion of a Date object as a locally formatted string.|
|toLocaleString()![ref34]|Converts a Date object to a locally formatted string.|
|toString()![ref37]|Converts a Date object to a string.|
|toTimeString()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.133.png)|Converts the time portion of a Date object to a string.|
|toUTCString()![ref38]|Converts a Date object to a string, according to universal time.|
|UTC()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.135.png)|Returns the number of milliseconds in a Date object since January 1, 1970, 000000 (midnight), universal time.|
|valueOf()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.136.png)|Returns the primitive value of a Date object.|

**JavaScript Math Reference**

This chapter contains a brief overview of the properties and method of the global Math object.

**The JavaScript Math Object**

The JavaScript Math object is used to perform mathematical tasks. The Math object is a static built-in object, so you won't need to instantiate it, all its properties and methods can be accessed directly.

To learn more about Math, please check out theJavaScr[ipt math operationschapt](https://www.tutorialrepublic.com/javascript-tutorial/javascript-math-operations.php)er.

**Math Properties**

The following table lists the standard properties of the Math object.



|Property|Description|
| - | - |
|E![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.137.png)|Returns Euler's number, the base of natural logarithms, e , approximately 2.718![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.138.png)|
|LN2![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.139.png)|Returns the natural logarithm of 2, approximately 0.693|
|LN10![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.140.png)|Returns the natural logarithm of 10, approximately 2.302|
|LOG2E![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.141.png)|Returns the base 2 logarithm of e , approximately 1.442![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.142.png)|
|LOG10E![ref23]|Returns the base 10 logarithm of e , approximately 0.434![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.143.png)|
|PI![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.144.png)|Returns the ratio of the circumference of a circle to its diameter (i.e. π ). The approximate value of PI is 3.14159|
|SQRT1\_2![ref39]|Returns the square root of 1/2, approximately 0.707|
|SQRT2![ref40]|Returns the square root of 2, approximately 1.414|

**Note:**The Math object is just a collection of static functions and constants. The Math object is different from other built-in objects (e.g. Date, Array, String, etc.), because it has no constructor, so there is no way to create an instance of Math.![ref2]

**Math Methods**

The following table lists the standard methods of the Math object.



|Method|Description|
| - | - |
|abs()![ref40]|Returns the absolute value of a number.|
|acos()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.147.png)|Returns the arccosine of a number, in radians.|
|acosh()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.148.png)|Returns the hyperbolic arccosine of a number.|
|asin()![ref18]|Returns the arcsine of a number, in radians|
|asinh()![ref41]|Returns the hyperbolic arcsine of a number.|
|atan()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.150.png)|Returns the arctangent of a number, in radians.|
|atan2(y, x)![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.151.png)|Returns the arctangent of the quotient of its arguments.|
|atanh()![ref39]|Returns the hyperbolic arctangent of a number.|
|cbrt()![ref42]|Returns the cube root of a number.|
|ceil()![ref11]|Returns the next integer greater than or equal to a given number (rounding up).|



|cos()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.153.png)|Returns the cosine of the specified angle. The angle must be specified in radians.|
| - | :- |
|cosh()![ref42]|Returns the hyperbolic cosine of a number.|
|exp(x)![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.154.png)|Returns e x , where x is the argument, and e is Euler's number (also known as Napier's constant), the base of the natural logarithms.![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.155.png)|
|floor()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.156.png)|Returns the next integer less than or equal to a given number (rounding down).|
|log()![ref40]|Returns the natural logarithm (base e ) of a number.|
|max(x, y, ...)|Returns the highest-valued number in a list of numbers.|
|min(x, y, ...)|Returns the lowest-valued number in a list of numbers.|
|pow(x, y)![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.157.png)|Returns the base to the exponent power, that is, x y .![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.158.png)|
|random()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.159.png)|Returns a random number between 0 and 1 (including 0, but not 1.|
|round()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.160.png)|Returns the value of a number rounded to the nearest integer.|
|sin()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.161.png)|Returns the sign of a number (given in radians).|
|sinh()![ref18]|Returns the hyperbolic sine of a number.|
|sqrt()![ref42]|Returns the square root of a number.|
|tan()![ref32]|Returns the tangent of a number.|
|tanh()![ref24]|Returns the hyperbolic tangent of a number.|
|trunc(x)![ref43]|Returns the integer part of a number by removing any fractional digits.|

**JavaScript Number Reference![ref44]![ref44]**

This chapter contains a brief overview of the properties and method of the global Number object.

**The JavaScript Number Object**

The JavaScript Number object acts as a wrapper for primitive numeric values. JavaScript has only one kind of number data type and it doesn't distinguish between integers and floating-point values.

To learn more about Number, please check out theJavaScript[ numberschapter.](https://www.tutorialrepublic.com/javascript-tutorial/javascript-numbers.php)

**Number Properties**

The following table lists the standard properties of the Number object.



|Property|Description|
| - | - |
|MI N\_SAFE\_I NTEGER![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.164.png)|Represents the maximum safe integer in JavaScript 253  1.|
|MAX\_VALUE![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.165.png)|Returns the largest numeric value representable in JavaScript, approximately 1.79E308. Values larger than MAX\_VALUE are represented as![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.166.png) Infinity .![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.167.png)|
|MI N\_SAFE\_I NTEGER![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.168.png)|Represents the minimum safe integer in JavaScript 253  1.|
|MI N\_VALUE![ref22]|Returns the smallest positive numeric value representable in JavaScript, approximately 5e-324. It is closest to 0, not the most negative number. Values smaller than MIN\_VALUE are converted to 0.![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.169.png)|
|NEGATIVE\_INFINITY![ref33]|Represents the negative infinity value.|
|NaN![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.170.png)|Represents "Not-ANumber" value.|
|POSITIVE\_INFINITY![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.171.png)|Represents the infinity value.|
|prototype![ref36]|Allows you to add new properties and methods to a Number object.|

**Note:**Every object in JavaScript has a constructor property that refers to the constructor function that was used to create the instance of that object.![ref10]

**Number Methods**

The following table lists the standard methods of the Number object.



|Method|Description|
| - | - |
|isFinite()![ref20]|Checks whether the passed value is a finite number.|
|isInteger()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.172.png)|Checks whether the passed value is an integer.|
|isNaN()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.173.png)|Checks whether the passed value is NaN and its type is Number.|
|isSafeInteger()![ref29]|Checks whether a value is a safe integer.|
|toExponential()![ref35]|Converts a number to exponential notation.|
|toFixed()![ref45]|Formats a number using fixed-point notation.|
|toPrecision()![ref38]|Returns a string representing the number to the specified precision.|



|toString()![ref20]|Converts a number to a string.|
| - | - |
|valueOf()![ref21]|Returns the primitive value of a Number object.|

**JavaScript String Reference**

This chapter contains a brief overview of the properties and method of the global String object.

**The JavaScript String Object**

The JavaScript String object is a global object that is used to store strings. A string is a sequence of letters, numbers, special characters and arithmetic values or combination of all.

To learn more about String, please check out theJavaScr[ipt stringschapter. ](https://www.tutorialrepublic.com/javascript-tutorial/javascript-strings.php)**String Properties**

The following table lists the standard properties of the String object.



|Property|Description|
| - | - |
|length![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.175.png)|Returns the length of a string.|
|prototype![ref21]|Allows you to add new properties and methods to an String object.|

**Note:**Every object in JavaScript has a constructor property that refers to the constructor function that was used to create the instance of that object.![ref2]

**String Methods**

The following table lists the standard methods of the String object.



|Method|Description|
| - | - |
|charAt()![ref43]|Returns the character at the specified index.|
|charCodeAt()![ref13]|Returns the Unicode of the character at the specified index.|
|concat()![ref17]|Joins two or more strings, and returns a new string.|



|endsWith()![ref20]|Checks whether a string ends with a specified substring.|
| - | - |
|fromCharCode()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.176.png)|Converts Unicode values to characters.|
|includes()![ref37]|Checks whether a string contains the specified substring.|
|indexOf()![ref14]|Returns the index of the first occurrence of the specified value in a string.|
|lastIndexOf()![ref25]|Returns the index of the last occurrence of the specified value in a string.|
|localeCompare()![ref31]|Compares two strings in the current locale.|
|match()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.177.png)|Matches a string against a regular expression, and returns an array of all matches.|
|repeat()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.178.png)|Returns a new string which contains the specified number of copies of the original string.|
|replace()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.179.png)|Replaces the occurrences of a string or pattern inside a string with another string, and return a new string without modifying the original string.|
|search()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.180.png)|Searches a string against a regular expression, and returns the index of the first match.|
|slice()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.181.png)|Extracts a portion of a string and returns it as a new string.|
|split()![ref41]|Splits a string into an array of substrings.|
|startsWith()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.182.png)|Checks whether a string begins with a specified substring.|
|substr()![ref12]|Extracts the part of a string between the start index and a number of characters after it.|
|substring()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.183.png)|Extracts the part of a string between the start and end indexes.|
|toLocaleLowerCase()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.184.png)|Converts a string to lowercase letters, according to host machine's current locale.|
|toLocaleUpperCase()![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.185.png)|Converts a string to uppercase letters, according to host machine's current locale.|
|toLowerCase()![ref28]|Converts a string to lowercase letters.|
|toString()![ref20]|Returns a string representing the specified object.|
|toUpperCase()![ref27]|Converts a string to uppercase letters.|
|trim()![ref42]|Removes whitespace from both ends of a string.|
|valueOf()![ref45]|Returns the primitive value of a String object.|

**JavaScript Functions**

In this tutorial you will learn how to define and call a function in JavaScript.

**What is Function?**

A function is a group of statements that perform specific tasks and can be kept and maintained separately form main program. Functions provide a way to create reusable code packages which are more portable and easier to debug. Here are some advantages of using functions:

- **Functions reduces the repetition of code within a program**  Function allows you to extract commonly used block of code into a single component. Now you can perform the same task by calling this function wherever you want within your script without having to copy and paste the same block of code again and again.
  - **Functions makes the code much easier to maintain**  Since a function created once can be used many times, so any changes made inside a function automatically implemented at all the places without touching the several files.
    - **Functions makes it easier to eliminate the errors**  When the program is subdivided into functions, if any error occur you know exactly what function causing the error and where to find it. Therefore, fixing errors becomes much easier.

The following section will show you how to define and call functions in your scripts.

**Defining and Calling a Function**

The declaration of a function start with the function keyword, followed by the name of the function you want to create, followed by parentheses i.e. () and finally place your function's code between curly brackets {} . Here's the basic syntax for declaring a function:

functionfunctionName() {// Code to be executed} Here is a simple example of a function, that will show a hello message:

Ja vascr ipt 41

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=define-and-call-a-function)**

// Defining function![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.186.png)

function sayHello() {

alert("Hello, welcome to this website!"); }

// Calling function

sayHello(); // 0utputs: Hello, welcome to this website!

Once a function is defined it can be called (invoked) from anywhere in the document, by typing its name followed by a set of parentheses, like sayHello() in the example above.

**Note:**A function name must start with a letter or underscore character not with a number, optionally followed by the more letters, numbers, or underscore characters. Function names are case sensitive, just like variable names.![ref1]

**Adding Parameters to Functions**

You can specify parameters when you define your function to accept input values at run time. The parameters work like placeholder variables within a function; they're replaced at run time by the values (known as argument) provided to the function at the time of invocation.

Parameters are set on the first line of the function inside the set of parentheses, like this:

functionfunctionName(*parameter1*,*parameter2*,*parameter3*) {// Code to be executed}

The displaySum() function in the following example takes two numbers as arguments, simply add them together and then display the result in the browser.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=add-parameters-to-a-function)**

// Defining function![ref46]

function displaySum(num1, num2) {

let total = num1 + num2; ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.188.png)alert(total);

}

// Calling function

displaySum(6, 20); // 0utputs: 26 displaySum(-5, 17); // 0utputs: 12

You can define as many parameters as you like. However for each parameter you specify, a corresponding argument needs to be passed to the function when it is called, otherwise its value becomes undefined . Let's consider the following example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=pass-arguments-to-a-function)**

// Defining function![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.189.png)

function showFullname(firstName, lastName) {

alert(firstName + " " + lastName);

}

// Calling function

showFullname("Clark", "Kent"); // 0utputs: Clark Kent showFullname("John"); // 0utputs: John undefined![ref1]

**Default Values for Function Parameters ES6**

With ES6, now you can specify default values to the function parameters. This means that if no arguments are provided to function when it is called these default parameters values will be used. This is one of the most awaited features in JavaScript. Here's an example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=es6-function-with-default-parameter-values)**

function sayHello(name = 'Guest') {![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.190.png)

alert('Hello, ' + name);

}

sayHello(); // 0utputs: Hello, Guest sayHello('John'); // 0utputs: Hello, John

While prior to ES6, to achieve the same we had to write something like this: **Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=setting-default-values-for-function-parameters-in-older-versions)**

function sayHello(name) {![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.191.png)

let name = name || 'Guest'; alert('Hello, ' + name);

}

sayHello(); // 0utputs: Hello, Guest sayHello('John'); // 0utputs: Hello, John

To learn about other ES6 features, please check out theJavaScript [ES6 featureschapt](https://www.tutorialrepublic.com/javascript-tutorial/javascript-es6-features.php)er.![ref1]

**Returning Values from a Function**

A function can return a value back to the script that called the function as a result using the return statement. The value may be of any type, including arrays and objects.

The return statement usually placed as the last line of the function before the closing curly bracket and ends it with a semicolon, as shown in the following example.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=return-a-value-from-a-function)**

// Defining function![ref46]

function getSum(num1, num2) {

let total = num1 + num2; ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.192.png)return total;

}

// Displaying returned value alert(getSum(6, 20)); // 0utputs: 26 alert(getSum(-5, 17)); // 0utputs: 12

A function*can not*return multiple values. However, you can obtain similar results by returning anar[rayof v](https://www.tutorialrepublic.com/javascript-tutorial/javascript-arrays.php)alues, as demonstrated in the following example.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=return-multiple-values-from-a-function)**

// Defining function![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.193.png)

function divideNumbers(dividend, divisor){ let quotient = dividend / divisor;

let arr = [dividend, divisor, quotient]; return arr;

}

// Store returned value in a variable let all = divideNumbers(10, 2);

// Displaying individual values alert(all[0]); // 0utputs: 10 alert(all[1]); // 0utputs: 2 alert(all[2]); // 0utputs: 5![ref1]

**Working with Function Expressions**

The syntax that we've used before to create functions is called function declaration. There is another syntax for creating a function that is called a function expression.

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=function-expression)**

Ja vascr ipt 45
**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=function-declaration-vs-function-expression)**

// Function Declaration ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.194.png)function getSum(num1, num2) {

let total = num1 + num2; return total;

}

// Function Expression

let getSum = function(num1, num2) { let total = num1 + num2;

return total;

};

Once function expression has been stored in a variable, the variable can be used as a function:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=assign-a-function-to-a-variable)**

let getSum = function(num1, num2) { ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.195.png)let total = num1 + num2;

return total;

};

alert(getSum(5, 10)); // 0utputs: 15

let sum = getSum(7, 25); alert(sum); // 0utputs: 32

**Note:**There is no need to put a semicolon after the closing curly bracket in a function declaration. But function expressions, on the other hand, should always end with a semicolon.

**Tip:**In JavaScript functions can be stored in variables, passed into other functions as arguments, passed out of functions as return values, and constructed at run- time.

The syntax of the*function declaration*and*function expression*looks very similar, but they differ in the way they are evaluated, check out the following example:

declaration(); // Outputs: Hi, I'm a function declaration! ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.196.png)function declaration() {

alert("Hi, I'm a function declaration!");

}

expression(); // Uncaught TypeError: undefined is not a funct ion

let expression = function() {

alert("Hi, I'm a function expression!");

};

As you can see in the above example, the function expression threw an exception when it was invoked before it is defined, but the function declaration executed successfully.

JavaScript parse declaration function before the program executes. Therefore, it doesn't matter if the program invokes the function before it is defined because JavaScript has[hoisted the functionto the t](https://www.tutorialrepublic.com/javascript-tutorial/javascript-hoisting.php)op of the current scope behind the scenes. The function expression is not evaluated until it is assigned to a variable; therefore, it is still undefined when invoked.

ES6 has introduced even shorter syntax for writing function expression which is calledar[row function, ple](https://www.tutorialrepublic.com/javascript-tutorial/javascript-es6-features.php#arrow-functions)ase check out theJavaScr[ipt ES6 featureschapter to ](https://www.tutorialrepublic.com/javascript-tutorial/javascript-es6-features.php)learn more about it.![ref1]

**Understanding the Variable Scope**

However, you can declare the variables anywhere in JavaScript. But, the location of the declaration determines the extent of a variable's availability within the JavaScript program i.e. where the variable can be used or accessed. This accessibility is known as*variable scope*.

By default, variables declared within a function have*local scope*that means they cannot be viewed or manipulated from outside of that function, as shown in the example below:

// Defining function![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.197.png)

function greetWorld() {

let greet = "Hello World!"; alert(greet);

}

greetWorld(); // Outputs: Hello World!

alert(greet); // Uncaught ReferenceError: greet is not define d

However, any variables declared in a program outside of a function has*global scope*i.e. it will be available to all script, whether that script is inside a function or outside. Here's an example:

**Example[Try this code»**](https://www.tutorialrepublic.com/codelab.php?topic=javascript&file=global-variable)**

let greet = "Hello World!"; ![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.198.png)// Defining function

function greetWorld() {

alert(greet);

}

greetWorld();  // Outputs: Hello World!

alert(greet); // Outputs: Hello World! example for arrow function

<!DOCTYPE html> <html lang="en"> <head>![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.199.png)

`    `<meta charset="utf-8">

Ja vascr ipt 48

`    `<title>JavaScript ES6 Arrow Functions</title> </head>![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.200.png)

<body>

`    `<script>

`    `// Function Expression     var sum = function(a, b) {         return a + b;

}

`    `document.write(sum(2, 3)); // 5

`    `document.write("<br>");

`    `// Arrow function     var sum = (a, b) => a + b;     document.write(sum(2, 3)); // 5     </script>

</body>

</html>

example of anonymous function

<!DOCTYPE html>![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.201.png)

<html lang="en">

<head>

<meta charset="utf-8"> <title>JavaScript Construct Closure Using Function Expression Sy </head>

<body>

<script>

// Anonymous function expression

let myCounter = (function() {

let counter = 0;

// Nested anonymous function

return function() {                 counter += 1;

return counter;

Ja vascr ipt 49

} })();![](Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.202.png)

`        `document.write(myCounter() + "<br>"); // Prints: 1         document.write(myCounter()); // Prints: 2

</script>

</body>

</html>
Ja vascr ipt 50

[ref1]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.002.png
[ref2]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.012.png
[ref3]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.013.png
[ref4]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.014.png
[ref5]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.015.png
[ref6]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.035.png
[ref7]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.041.png
[ref8]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.053.png
[ref9]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.055.png
[ref10]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.057.png
[ref11]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.069.png
[ref12]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.071.png
[ref13]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.072.png
[ref14]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.073.png
[ref15]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.074.png
[ref16]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.075.png
[ref17]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.076.png
[ref18]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.077.png
[ref19]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.079.png
[ref20]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.081.png
[ref21]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.082.png
[ref22]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.083.png
[ref23]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.084.png
[ref24]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.085.png
[ref25]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.086.png
[ref26]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.090.png
[ref27]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.091.png
[ref28]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.109.png
[ref29]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.111.png
[ref30]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.112.png
[ref31]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.113.png
[ref32]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.114.png
[ref33]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.116.png
[ref34]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.121.png
[ref35]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.124.png
[ref36]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.125.png
[ref37]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.132.png
[ref38]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.134.png
[ref39]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.145.png
[ref40]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.146.png
[ref41]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.149.png
[ref42]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.152.png
[ref43]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.162.png
[ref44]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.163.png
[ref45]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.174.png
[ref46]: Aspose.Words.4ecbbb8f-5836-4e4d-890e-c8a7d101a663.187.png
