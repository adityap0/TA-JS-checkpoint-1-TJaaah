1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
let sum =0;
for (i=0; i<=10; i++)
{
  sum = sum + Number(prompt(`Enter the Number`));
}
let avg = sum/ 10;
console.log(`The average of the entered numbers are ${avg}`);
```
2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
hi
hi
hi
2
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
function getEvenSum(max =10)
{
  let sum =0;
  for (let i =0; i<=max; i++)
  {
    if(i%2==0)
    {
      sum = sum + i;
    }
  }
  return sum;
}
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
function getOddSum(max =10)
{
  let sum =0;
  for (let i =0; i<=max; i++)
  {
    if(i%2!=0)
    {
      sum = sum + i;
    }
  }
  return sum;
}
```
5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.
```js
function getProductOfDigits(num)
{
  if(num>0)
  {
  let count =0;
  let count_check = num;
  let prod =1;
  while(count_check>1)
  {
    count ++;
    count_check = count_check/10;
  }
for(let i = 1; i<=count; i++)
{
let rem = num%10;
num = num - rem;
num = num/10;
prod = prod*rem;
}
return prod;
}
else {return `Not valid`;}
}
```
- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

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

check(10); // "Bigger than 5" as 10>5
check(1); // "Smaller than 5" as 1<5
check(5); // 5 as no condition is true
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // You are arya, 1st condition true
getOutput('John'); // You are john, 2nd condition true
getOutput(); // Who are you, default return.
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // You are arya, 1st condition true
getOutput('John'); // You are john, 2nd condition true
getOutput(); // Who are you, default return.
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
yes a function can have multiple return statements but only one return can be compiled. for example
```js
function getOutput(name) {
  if (name === 'Arya') return'You are Arya';
  else if (name === 'John') return'You are John';
  else return 'Who are you';
}
```

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
Ans - in for loop there are three conditions that needs to be satisfied whereas in while loop only one condition and increment is needed. 

