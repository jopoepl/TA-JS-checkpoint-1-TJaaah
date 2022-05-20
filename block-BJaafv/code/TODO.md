1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
The first function has an output of a + b which we can store in a variable as memory is allocated to the output which can be called later.
The second function only prints the output in the console but it cannot be stored in a variable. 


2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

value of first will be the returned value of a + b,
but value of second will be undefined

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

The first and second parameters are defined so, it will take a = 12 and b = 24, while 35 will be ignored. 
So answer will be 36 (12 + 24).

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

Yes, since function is also an expression it can be stored in a variable (function expression).

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

//

function sayHello (name) {
  return `Hello ${name}`;
  
}

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}



showMessage();

'Hello, John'

// Because it does not accept any parameters and will always return Hello + username. Here username is already defined to John, so it will always output `Hello, John`
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); //  John

showMessage(); // 'Hello, John'


alert(userName); // John
```

8. What is a Anonymous Function give example of three functions.

Anonymous functions are functions without any names. They can be used as arguments for a variable. We can use Anonymous functions while writing function expressions.
Eg - var anonFunction1 = function (name) {
alert (name)
}
let anonFunction2 = function (a,b) {
return (a + b)
}
let anonFunction3 = function (color) {
return (color == `red`)
}


9. Can function declaration be a Anonymous Function? Explain

Yes. Whenever we are defining a function expression, we can use anonymous function which does not have a name associated with it. 
We can call this function using the variable associated with it. 
eg let anonFunction = function (a,b) {
  return a + b
} 

Here function (a,b) is the anonymous function. 



10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

calcSquare (n) --> calculates the square of the number
checkGreaterThan (a, b) --> checks if a is greater than b
calcSum (a, b) --> gets or calculates the sum of a and b
getEvenNum (n) --> gets the first n even numbers
sayHello (name) -->  says Hello to the user



```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
