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

- what is NodeJs?
	- *Wikipedia* : Node.js is an open-source, cross-platform, back-end JavaScript runtime environment that runs on the V8 engine and executes JavaScript code outside a web browser. Node.js lets developers use JavaScript to write command line tools and for server-side scripting—running scripts server-side to produce dynamic web page content before the page is sent to the user's web browser. Consequently, Node.js represents a "JavaScript everywhere" paradigm, unifying web-application development around a single programming language, rather than different languages for server-side and client-side scripts. Node.js has an event-driven architecture capable of asynchronous I/O. These design choices aim to optimize throughput and scalability in web applications with many input/output operations, as well as for real-time Web applications (e.g., real-time communication programs and browser games). The Node.js distributed development project was previously governed by the Node.js Foundation, and has now merged with the JS Foundation to form the OpenJS Foundation, which is facilitated by the Linux Foundation's Collaborative Projects program.
	- *W3Schools* : Node.js is an free and open source server environment which can runs on various platforms. Node.js uses JavaScript on the server
	-	*MDN* : Node.js is a cross-platform JavaScript runtime environment that allows developers to build server-side and network applications with JavaScript.

- what is "use strict"?


- what is run time environment?

- what is JSON?

- what is Falsy values?

- what is Logical operators?

- what is DOM?

- data types?

- what is wrapper object?

- difference between primitive and referenced types?

- let , var , const

- null , undefined

- == , ===

- difference between POST and Get methods in Http requests.

- arrays and methods (map , filter , find , reduce , some , every , indexOf , sort)

- objects

- array of objects

- scope

- explain some Feature in ES6

- explain spread operator

- explain Object Destructuring 

- explain Default Parameters

- what is continue operator?

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
