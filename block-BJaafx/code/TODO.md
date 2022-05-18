1. Using loops take 10 inputs from user and find the average of all the numbers.



```js


let sum = 0;
for (let i = 1; i <=10; i++) {
 let n = +prompt (`Enter a number`);
  sum += n;
}
alert (`Average of numbers is` + " " + sum/10);

```
 

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
println is not a valid method in JS, so the code will show reference error. 



3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.


```js
function getEvenSum (max = 10) {
  let sum = 0;
  for (let i = 0; i <= max; i++)
  if (i % 2 == 0) {
    sum += i;
  }
  return sum
}
```


4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

```js

function getOddSum (max = 10) {
  let sum = 0;
  for (let i = 0; i <= max; i++)
  if (i % 2 !== 0) {
    sum += i;
  }
  return sum
}

```


5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

```js


function getProductOfDigits (num) {

    let sDigits = String(num)
    let digits =  sDigits.split(``);
    let product = 1;
    for (let i = 0; i <= (digits.length - 1); i++) { //condition of i would be n-1 after split method

      if (num > 0) {
   product *= Number(digits[i]);


  } else {
    return `Not a valid input`
  } 
  
} return (product);
}

```


6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); //  'Bigger than 5' -- because if num > 5 is true and the first if condition is triggered
check(1); // 'Smaller than 5' -- because if num > 5 is false, it moves to the next condition in the code which is if num < 5 is true.Since the second condition is true, the second return statement is triggered condition is triggered.
check(5); // 5 -- In this case first and second conditions are false, so it returns the number value. 
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); 
getOutput('John'); // what will be the output
getOutput(); // what will be the output
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // 'Who are you` - because return statement for the function is set to this. But we would see 'You are arya' in the console.
getOutput('John'); // 'Who are you` - because return statement for the function is set to this. But we would see 'You are john' in the console.
getOutput(); // 'Who are you' - return statement is set to this
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

A function can have multiple return statements. These return points will act as the exit points for each condition. Note that even though there can be multiple return statements, once a return statement is executed,  the function would stop. 

Eg
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

Here there are three return statements for 3 conditions and the function exits as soon as one condition is met and output is returned. 





10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

For loop is ideally used when the counter is known. On the other hand, while loop is used when there is a condition to be met (exact number is not known until the user inputs) and until then the loop runs. 
```js
for (let i = 0; i<=5; i++) {
  console.log (i)
}

```

```js
let sum = 0;
let i = 0;

function sumNumbers (num) {
while (i < num){
  i++
  sum += i;
} return sum
}

```

