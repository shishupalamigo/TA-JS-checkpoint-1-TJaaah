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
Ans: 'return" is a statement that allows a function to output a value back to where it was called. console.log is a function that lets us inspect values for debugging purposes. In the above code the
1st `sum` function has a return statement hence will output the result of `a + b` when executed with required parameters. 
On the other hand the 2nd `sum` function has `console.log` function which will log the sum of a and b 
in the browser's console and will not give any output. 

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

Ans: The value of `first` will be the sum of parameter value of a and b.
The value of `second` will be undefined because the value from the second `sum` function will only be 
console logged and will not be assigned to the variable `second` as the function dosen't have a return statement. 


3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

Ans: The Output will be `36` that is the sum of 1st 2 parameters that has been declared  while declaration of the function. The 3rd argument will be ignored by JavaScript as it has not been declared. 

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

Ans: Yes we can store the first `sum` function in a variable named `add` because a function is an `expression` not 
a `statement` and hence can be stored as a value of any variable. 

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

```js
function sayHello(name) {
  return `Hello ${name}`
}

```

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```

Ans: The output of the above function will  be "Hello John" because the variable `userName` has been assigned the value `John` before  the declaraation of function. The function sayHello will search for `userName` within the function 1st and 
when that is not found inside the function it will  look outside the function for variable named `userName` and will return result when it finds the value.

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // John 

showMessage(); // "Hello, John"

alert(userName); // John
```

8. What is a Anonymous Function give example of three functions.

Ans: Anonymous functions are functions which are declared without a name. 
Examples - 
```js
//Example 1
let addNumbers = function (a, b) {
  return a + b;
}
//Example 2
let fullName = (firstName, lastName) => firstName + " " + lastName;

//Example 3 
let substactNum = function (a, b) {
    return a - b;
};

```


9. Can function declaration be a Anonymous Function? Explain

Ans: The Function declaration can not be a an anonymous function. When a function is declared  without a name it is assigned to  variable and it becomes a `function Expression` not a declartion. 

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

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
```js

//Example 1 
function fullName(firstName,  lastName) {
  return firstName + " " + lastName;
}
//Example 2 
function addNumbers(numA, numB) {
  return numA + numB;
}
//Example 3 
function isAdult (age) {
  return age > 18;
}
//Example 4 
function getRemainder (n, p) {
  return n % p;
}
//Example 5 
function daysInMonth (month){
  let days = '';
}