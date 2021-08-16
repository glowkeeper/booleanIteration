# An Introduction to Loops and Iteration

Dr Steve Huckle

steve@glowkeeper.uk

August 2021

- - -

# Lecture Overview

+ Loops and iteration
+ Javascript loops
+ Some examples
+ Exercise
+ Useful resources

- - -

# Goals

1. Introduce iteration and Javascript loops
2. The **overarching** aim is to encourage you to begin your programming journey by _writing some code_!

- - -

# What is Iteration?

Iteration is the process of repeating steps. For example, I conduct an iterative ritual each morning:

1. Put water in a kettle and switch it on
2. Meanwhile, grind coffee beans and put the ground coffee in a carafe
3. Put boiling water in the carafe and replace the lid
4. Wait 4 minutes for the coffee to brew, then gently push the plunger all the way down
5. Pour the coffee
6. Repeat from step 1 until I feel ready to go about my day

- - -

# Loops

In programming, iteration is often referred to as _looping_, because when a program iterates, it _loops_ through steps. Programming languages implement iteration using statements like `for` and `while`.

```javascript
let done = false;
while (true) {
  // do something that might set done to true
  if (done) {
    break;
  }
}
```

- - -

# Javascript Loops

Javascript has three basic looping statements:

1. `for`
2. `while`
3. `do`

- - -

# Count Control Loops

`for` statements are a form of _count control_ loop, which are useful when it is necessary to iterate a specific number of times.

1. Set the total to 0
2. Repeat this section five times
    1. Generate a single-digit number
    2. Add the number to the total
3. Go back to step 2
4. Output the total

- - -

# Count Control Loops (cont'd)

```javascript
let total = 0;
for (let i = 0; i < 5; i++) {
  total += Math.floor(Math.random() * 10); 
}
console.log(total);
```

- - -

# An Opinionated Viewpoint

**Where possible, use the array method `forEach`, not `for`**

The `for` loop has its origins in early computer languages like _Fortran_ and _C_, and its control structure, `{initialisation; condition; increment}` can be a little daunting on first view. Besides, often that control structure is _too much detail_.

When you want to _do something to each element of a list_, `forEach` is often a better choice than `for`.

- - -

# An Opinionated Viewpoint (cont'd)

1. `forEach`

```javascript
const coffee = ['Water', 'Kettle', 'Grind', 'Carafe', 'Brew', 'Pour', 'Enjoy'];
coffee.forEach(element => console.log(element));
```

2. `for`

```javascript
const coffee = ['Water', 'Kettle', 'Grind', 'Carafe', 'Brew', 'Pour', 'Enjoy'];
for (let i = 0; i < coffee.length; i++) {
  console.log(coffee);
}
```

- - -

# Conditional Loops

A conditional loop continues _while_ (or _until_) a condition is met.

```javascript
do {
  // drink coffee
  // contemplate my day
} while (hasTime);
```

- - -

# Conditional Loops - A Note of Caution

Be careful using conditional loops because if the condition is never met, they might loop forever.

```javascript
const iceCapsAreMelting = true;
let polarBears = 5;

// Initiate (possible) infinite loop
while (iceCapsAreMelting) {
  console.log(`There are ${polarBears} polar bears.`);
  polarBears--;
  // Terminate the loop if the following condition is true
  if (polarBears === 0) {
    console.log("There are no polar bears left.");
    break;
  }
}
```

- - -

# Examples

[https://github.com/glowkeeper](https://github.com/glowkeeper)

...and there is some more example code in the next section...

- - -

# Hello (World)

```javascript
//code goes here
```

- - -

# Recap

+ An introduction to loops and iteration
+ Javascript loops `for`, `while` and `do`
+ Some examples

- - -

# Exercise

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration

- - -

# Useful Resources

+ [https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)
+ [https://www.digitalocean.com/community/tutorials/using-while-loops-and-do-while-loops-in-javascript](https://www.digitalocean.com/community/tutorials/using-while-loops-and-do-while-loops-in-javascript)

- - -

# Thank-you

Dr Steve Huckle

steve@glowkeeper.uk
