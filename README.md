# Welcome to JavaScript Interview Bank!

Hi! We are going to collect all useful javascript interview questions and exercises in here!

This repository is free to use and fork and anything you want!

Also it will be good if you make any useful changes in it and send pull request to publish.

As you probably guess this is not a regular text file and this is an **\*.md** file. To edit this kind of files you can anything you want but we recommend [StackEdit](https://stackedit.io/)

## Sections

All questions and exercises are in this single file.

You will find two main sections in here :

1. Questions

2. Exercises

## Questions :

**Level : Junior**

- what is NodeJs?

- what is run time environment?

- what is JSON?

- data types?

- difference between primitive and referenced types?

- let , var , const

- null , undefined

- == , ===

- difference between POST and Get methods in Http requests.

- arrays and methods (map , filter , find , reduce , some , every , indexOf , sort)

- objects

- array of objects

- scope

**Level : Middle**

- sync vs async

- callback

- promise

- async/await

- eventLoop

- regular functions vs arrow functions

- this

- bind , call , apply

- higher order function

- prototype

- currying function

- memoization

- prototype

- closure

- recursion

- eval

- difference between req.params and req.query in Http requests.

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
