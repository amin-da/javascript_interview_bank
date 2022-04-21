# Welcome to JavaScript Interview Bank!

Hi! We are going to collect all useful javascript interview questions and exercises in here!

This repository is free to use and fork and anything you want!

Also it will be good if you make any useful changes in it and send pull request to publish.

As you probably guess this is not a regular text file and this is an **\*.md** file. To edit this kind of files you can anything you want but we recommend Github raw edit option (pencil symbol)

## Sections

All questions and exercises are in this single file.

You will find two main sections in here :

1. Questions

2. Exercises

## Questions :

**Level : Junior**

- what is JavaScript?
	- *Javascript.info* : JavaScript was initially created to “make web pages alive”. The programs in this language are called scripts. They can be written right in a web page’s HTML and run automatically as the page loads. Scripts are provided and executed as plain text. They don’t need special preparation or compilation to run. In this aspect, JavaScript is very different from another language called Java.
	- *MDN* : JavaScript is a scripting or programming language that allows you to implement complex features on web pages.
	- *W3Schools* : JavaScript is the Programming Language for the Web. Can update and change both HTML and CSS. Can calculate, manipulate and validate data
	- *Wikipedia* : JavaScript often abbreviated JS, is a programming language that is one of the core technologies of the World Wide Web, alongside HTML and CSS. Over 97% of websites use JavaScript on the client side for web page behavior, often incorporating third-party libraries.  All major web browsers have a dedicated JavaScript engine to execute the code on users' devices. JavaScript is a high-level, often just-in-time compiled language that conforms to the ECMAScript standard.  It has dynamic typing, prototype-based object-orientation, and first-class functions. It is multi-paradigm, supporting event-driven, functional, and imperative programming styles. It has application programming interfaces (APIs) for working with text, dates, regular expressions, standard data structures, and the Document Object Model (DOM). The ECMAScript standard does not include any input/output (I/O), such as networking, storage, or graphics facilities. In practice, the web browser or other runtime system provides JavaScript APIs for I/O.

- what is ECMAScript?
	- *Wikipedia* : ECMAScript (or ES) is a JavaScript standard meant to ensure the interoperability of web pages across different web browsers. It is standardized by Ecma International according to the document ECMA-262. ECMAScript is commonly used for client-side scripting on the World Wide Web, and it is increasingly being used for writing server applications and services using Node.js.
	- *IBM* : ECMAScript, also known as JavaScript, is a programming language adopted by the European Computer Manufacturer's Association as a standard for performing computations in Web applications.
	- *Educative.io* : ECMAScript is a general-purpose programming language that is implemented in Javascript and some other languages. It is the scripting language that formed the basis of browser-based Javascript and Node.js. ECMA is an acronym for European Computer Manufacturer’s Association, which develops standards for information technology and consumer electronics. Languages such as ECMAScript, Dart-lang, and C# were standardized by ECMA. Think of ECMAScript as Javascript without a host environment. Javascript has two major environments: browsers and Node.js. These environments add some APIs to the language. An example is the window object on Browsers and the fs module in Node.js. If you strip all external APIs from these environments, you get ECMAScript.

- what is NodeJs?
	- *Wikipedia* : Node.js is an open-source, cross-platform, back-end JavaScript runtime environment that runs on the V8 engine and executes JavaScript code outside a web browser. Node.js lets developers use JavaScript to write command line tools and for server-side scripting—running scripts server-side to produce dynamic web page content before the page is sent to the user's web browser. Consequently, Node.js represents a "JavaScript everywhere" paradigm, unifying web-application development around a single programming language, rather than different languages for server-side and client-side scripts. Node.js has an event-driven architecture capable of asynchronous I/O. These design choices aim to optimize throughput and scalability in web applications with many input/output operations, as well as for real-time Web applications (e.g., real-time communication programs and browser games). The Node.js distributed development project was previously governed by the Node.js Foundation, and has now merged with the JS Foundation to form the OpenJS Foundation, which is facilitated by the Linux Foundation's Collaborative Projects program.
	- *W3Schools* : Node.js is an free and open source server environment which can runs on various platforms. Node.js uses JavaScript on the server
	-	*MDN* : Node.js is a cross-platform JavaScript runtime environment that allows developers to build server-side and network applications with JavaScript.

- what is run time environment?
	- *CodeAcademy* : A runtime environment is where your program will be executed. It determines what global objects your program can access and it can also impact how it runs.
	- *Google* : In Apps Script and JavaScript, a runtime or runtime environment contains the JavaScript engine that parses and executes script code. The runtime provides rules for how memory is accessed, how the program can interact with the computer's operating system, and what program syntax is legal.
	- *Medium (gemma.stiles)* : The JavaScript runtime environment provides access to built-in libraries and objects that are available to a program so that it can interact with the outside world and make the code work. In the context of a browser this is comprised of the following elements: 
		- The JavaScript engine (which in turn is made up of the heap and the call stack)
		- Web APIs
		- The callback queue 
		- The event loop

	Its good to be mindful that the runtime environment can take on different forms based on the context, for example, the runtime environment in a browser is very different from that of Node.js. These differences are primarily at the implementation level, so most of the following concepts are still relevant.

- data types (programiz.com)?

|  Data Types | Description   |  Example  |
| :------------ | :------------ | :------------ |
|  String  | represents textual data	  | 'hello', "hello world!" etc  |
|  Number  |  an integer or a floating-point number | 3, 3.234, 3e-2 etc.  |
|  BigInt  | an integer with arbitrary precision	  |  900719925124740999n , 1n etc. |
|  Boolean  | Any of two values: true or false	  | true and false  |
| undefined   | a data type whose variable is not initialized  |  let a; |
|  null  |  denotes a null value	 |  let a = null; |
| Symbol   | data type whose instances are unique and immutable  | let value = Symbol('hello');  |
| Object   |  key-value pairs of collection of data	 |  let student = { }; |

- scope 
	- *dmitripavlutin.com* : Scope refers to the availability of variables and functions in certain parts of the code. The inner scope can access the variables of its outer scope. In JavaScript, a variable has two types of scope:
		- Global Scope
		- Module Scope (es2015)
		- Local Scope
			- Block level ( let , const)
			- Function level ( var )

- let , var , const 

|  Keyword  |  Scope  | Hoisting   | Can Be Reassigned  | Can Be Redeclared|
| :------------ | :------------ | :------------ | :------------ | :------------ |
|  var |  Function  |  Yes  |  Yes  | Yes |
|  let |  Block  |  No (but actually yes!)  | Yes   | Yes |
|  const | Block   | No (but actually yes!)   |  No  | Yes |

- null , undefined (flexiple.com)

| Keyword  | data type  | arithmetic operations  |  boolean value | comparing | description |
| ------------ | ------------ | ------------ | ------------ |------------ | ------------ |
| undefined  | undefined  |  undefined + 1 //NaN |  !!undefined //false | null == undefined //true | means a variable has been declared but has not yet been assigned a value |
|  null | object (but it considered as primitive)  | null + 1 // 0  | !!null //false  | null === undefined //false | It can be assigned to a variable as a representation of no value|


- hositing (medium.com/swlh/is-let-really-not-hoisted-abb75c38607e)
	- *MDN* : JavaScript Hoisting refers to the process whereby the interpreter appears to move the declaration of functions, variables or classes to the top of their scope, prior to execution of the code. Hoisting allows functions to be safely used in code before they are declared. Variable and class declarations are also hoisted, so they too can be referenced before they are declared. However JavaScript only hoists declarations, not initializations! This means that initialization doesn't happen until the associated line of code is executed, even if the variable was originally initialized then declared, or declared and initialized in the same line. Until that point in the execution is reached the variable has its default initialization (undefined for a variable declared using var, otherwise uninitialized) Note that doing so can lead to unexpected errors, and is not generally recommended.
	- *Medium (zeeshan.shamsuddeen)* : Technically, all JS variables are hoisted. Where let and cost differs from var in the hoisting process is in the initialization part.

- falsy values (MDN)

| boolean type  | values  |
| ------------ | ------------ |
| falsy  |  false , 0 , -0 , 0n (The BigInt zero) , "" , '' , null , undefined , NaN   |
|  truthy |  other values |

- operators (MDN)
	- Assignment operators
	- Comparison operators
	- Arithmetic operators
	- Bitwise operators
	- Logical operators
	- String operators
	- Conditional (ternary) operator
	- Comma operator
	- Unary operators
	- Relational operators

- logical operators (w3schools)

| Operator   | Description   | Comparing (x=5)   |  Returns  |
| :------------ | :------------ | :------------ | :------------ |
| ==  |  equal to | x == 5  |  true |
|  ===	 | equal value and equal type  |  	x === "5" | false  |
|  !=| not equal  | x != 5  | false  |
|!==   | not equal value or not equal type  | x !== "5"  | true  |
|  > | 	greater than  | x > 10  | false  |
| <  |  less than | x < 10  | true  |
| >=  |  greater than or equal to (same type) |  x >=10 | false  |
| <=  | less than or equal to (same type)  |  x<=10 |  true  |

- primitive and referenced types : 
	- *freecodecamp* : When you declare a primitive data type in JavaScript, it is stored on a stack. A stack is a simple data structure that the computer uses to store and retrieve data quickly.
	[![](https://www.freecodecamp.org/news/content/images/2022/01/Purple-Minimal-We-Are-Hiring-Twitter-Post--3-.png)](https://www.freecodecamp.org/news/content/images/2022/01/Purple-Minimal-We-Are-Hiring-Twitter-Post--3-.png)
	
	[![](https://www.freecodecamp.org/news/content/images/2022/01/Purple-Minimal-We-Are-Hiring-Twitter-Post--4-.png)](https://www.freecodecamp.org/news/content/images/2022/01/Purple-Minimal-We-Are-Hiring-Twitter-Post--4-.png)
	Reference data types, unlike primitive data types, are dynamic in nature. That is, they do not have a fixed size. Most of them are considered as objects, and therefore have methods. Examples of such data types include arrays, functions, collections, and all other types of objects. The difference comes in when the computer has to store a reference data type. When you create a variable and assign it a value that is a reference data type, the computer does not directly store that data type in that variable (as is the case with primitive types). What you have assigned to that variable is a pointer that points to the location of that data type in memory.
	[![](https://www.freecodecamp.org/news/content/images/2022/01/Purple-Minimal-We-Are-Hiring-Twitter-Post--5-.png)](https://www.freecodecamp.org/news/content/images/2022/01/Purple-Minimal-We-Are-Hiring-Twitter-Post--5-.png)
	
	[![](https://www.freecodecamp.org/news/content/images/2022/01/Purple-Minimal-We-Are-Hiring-Twitter-Post--6-.png)](https://www.freecodecamp.org/news/content/images/2022/01/Purple-Minimal-We-Are-Hiring-Twitter-Post--6-.png)


- what is JSON?

- what is "use strict"?

- arrays and methods (map , filter , find , reduce , some , every , indexOf , sort)

- objects

- array of objects

- ES6 features

- ES7 features

- spread operator

- rest operator

- object Destructuring 

- default parameters

- what is wrapper object?

- difference between POST and Get methods in Http requests.

- continue and break

**Level : Middle**

- sync vs async

- callback

- promise

- what is Microtasks?

- explain Promisification

- async/await

- eventLoop

- regular functions vs arrow functions

- this

- bind , call , apply

- higher order function

- what is First class citizen(Object)?

- prototype

- currying function

- memoization

- explain prototype chain

- what is Own Properties in objects ?
 
- closure

- recursion

- eval

- difference between req.params and req.query in Http requests.

- explain Nullish Coalescing 

- explain Logical OR 

- explain Logical AND

- explain Ternary operators

- explain Factory Function and Constructor functions 

- what is IIFE? What is it used for?

- explain Execution Contexts

- what is constructor method in calss ?

- what is the difference between freeze and seal methods in objects?

- what is Web components?


**Level : Senior**

- shat is body-parser?

- nodejs security mechanisms : Helmet (X-Frame-Options , XSS Protection , Strict Transport Security)

- event capturing vs event bubbling

- delegation

## Questions :

**Level : Junior**

- function that will return true if string is palindrome

  solution 1 :

  ```javascript
  function isPalindrome(str) {
    return str.split("").reverse().join("") === str;
  }
  ```

  solution 2 :

  ```javascript
  function isPalindrome(str) {
    return str
      .split("")
      .every((char, index) => char === str[str.length - index - 1]);
  }
  ```

- function that will return min and max number in an array

  solution 1 :

  ```javascript
  function getMinMax(arr) {
    return {
      min: Math.min(...arr),
      max: Math.max(...arr),
    };
  }
  ```

  solution 2 :

  ```javascript
  function getMinMax(arr) {
    const sortedArray = arr.sort((a, b) => a - b);
    return {
      min: sortedArray[0],
      max: sortedArray[sortedArray.length - 1],
    };
  }
  ```
  
  solution 3 :

  ```javascript
  function getMinMax(arr) {
    let min = arr[0];
    let max = arr[0];

    for (let current of arr) {
      if (current > max) {
        max = current;
      }

      if (current < min) {
        min = current;
      }
    }
    return {
      min,
      max,
    };
  }
  ```
  
- function that will verify if string has balanced parenthesis

  solution 1 :

  ```javascript
  function isBalanced(str) {
    const stack = [];

    for (let char of str) {
      if (char === "(") {
        stack.push(char);
      } else {
        const lastStackItem = stack.pop();
        if (lastStackItem !== "(") {
          return false;
        }
      }
    }
    if (stack.length != 0) return false;
    return true;
  }
  
  console.log(isBalanced("()()()"));
  //true
  console.log(isBalanced("()()))()"));
  //false
  ```
  
  solution 2 (previous solution refactored) :

  ```javascript
  function isBalanced(str) {
    const stack = [];

    for (let char of str) {
      if (char === "(") {
        stack.push(char);
      } else if (stack.pop() !== "(") {
        return false;
      }
    }
    return stack.length != 0 ? false : true;
  }
  
  console.log(isBalanced("()()()"));
  //true
  console.log(isBalanced("()()))()"));
  //false
  ```
