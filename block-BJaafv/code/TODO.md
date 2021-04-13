1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}
Ans - in the Above function the sum of a+b will be returned.
// second
function sum(a, b) {
  console.log(a + b);
}
Ans - in the Above function the sum of a+b will be logged.
```
2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
`first` -- a+b. AND `second` -- undefined.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
it will add 12 and 24 and log 36, as it will take the values of a and b, and leave the rest values passed.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
Yes we can store the value of first 'sum' into a variable named add, as we can store the value of one variable (first) into another variable (second)

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
```js
function sayHello(name)
{
  return `Hello ${name}`;
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
Output - "Hello, John", as the function can take values from outside the function therefore username would be assigned as 'John' and Hello John would be printed.
7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // John (alert)

showMessage(); // "Hello, John"

alert(userName); // John (alert)
```

8. What is a Anonymous Function give example of three functions.
Anonymous functions are those that do not have a name, they just have a function definition.  
Example : 
```js
1. let show = function () {
    console.log('Anonymous function');
};
show();
```
2. Using anonymous functions as arguments of other functions
We often use anonymous functions as arguments of other functions. For example:
```js
setTimeout(function () {
    console.log('Execute later after 1 second')
}, 1000);
```
```js
3. (function () {
    console.log(`${person.firstName} ${person.lastName}`);
    })(person);
```

9. Can function declaration be a Anonymous Function? Explain
yess function expressions can be anonymous if we are storing the value of the function in a variable. 
ex : let show = function () {
    console.log('Anonymous function');
};
show();
Here function does not have a name (hence anonymous) but its logging a value and that is being stored in 'show', now if we call 'show' then the value would be logged, behaving just as a normal function would.

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
