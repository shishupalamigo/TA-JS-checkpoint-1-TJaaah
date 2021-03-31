1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
let sumOfNumbers = 0;
for (let i = 1; i <= 10; i++ ) {
  let num = +prompt(`Enter number ${i}`);
  sumOfNumbers = sumOfNumbers + num;
}
let average = sumOfNumbers / 10;
alert(`The average of all enterd number ${average}`);
```
2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
- Output: println is not defined.

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

```js
function getEvenSum (max = 10) {
let sum  = 0;
  for (let i = 0; i <= max; i++) {
    if (i % 2 == 0 ) {
      sum = sum + i;
    } 
  } return sum;
}
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

```js
function getOddSum (max = 10) {
let sum  = 0;
  for (let i = 0; i <= max; i++) {
    if (i % 2 != 0 ) {
      sum = sum + i;
    } 
  } return sum;
}
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

```js 
function getProductOfDigits (num) {
  let product = 1;
  if (num < 0 ) {
    return `Not a valid input`;
  } else {
    while (num > 0) {
      let digit = num % 10;
      product *= digit; 
      num = Math.floor(num / 10);
    }
  } return product;
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

check(10); // 'Bigger than 5' Because 10 fulfills the 1st `if` condition >> return from function.
check(1); // 'Smaller than 5' Because 1 fulfills the 2nd `if` condition. >> return from function.
check(5); // 5 It does  not satisfy the above two conditions. >> return from function.
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya' >> return from function.
getOutput('John'); // 'You are john' >> return from function.
getOutput(); // 'Who are you' >> return from function.
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // 'you are arya' logged in the console,  and 'Who are you' >> return from function.
getOutput('John'); // 'you are john' logged in the console,  and 'Who are you' >> return from function.
getOutput(); // 'Who are you' >> return from function.
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

Ans: A function in JavaScript can not have multiple return statement. Although we use multiple return statement in if else statements and switch cases, only one return statement is executed when the condition is satisfied.


10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

Ans: 	The 'for' loop is used only when we already knew the number of iterations. On the other hand the 'while' loop is used only when the number of iteration are not exactly known.
