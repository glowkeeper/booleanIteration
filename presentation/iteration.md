# An Introduction to Loops and Iteration

Dr Steve Huckle

steve@glowkeeper.uk

August 2021

- - -

# Lecture Overview

+ Loops and iteration
+ Javascript loops
+ Exercises

- - -

# Goals

1. Introduce iteration and looping
2. Javascript loops
3. The **overarching** aim is to encourage you to begin your programming journey by _writing some code_!

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
  // maybe do something else
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

`for` statements are a form of _count control_ loop, which are useful when you need to iterate a specific number of times.

1. Set the total to 0
2. for a count from 1 to 5
    1. Add the count to the total
3. Output the total (the sum of all numbers between 1 and 5)

- - -

# Count Control Loops (cont'd)

Javascript `for` loops have a control structure of the form _{initialisation; condition; increment}_

```javascript
let total = 0;
for (let i = 1; i <= 5; i++) {
  total += i;
}
console.log(total);
```

The control structure of a `for` loop can appear quite challenging at first.

- - -

# forEach

When you want to _do something to each element of an array_, `forEach` might be a better choice.

1. `forEach`

```javascript
const coffee = ['Water', 'Kettle', 'Grind', 'Carafe', 'Brew', 'Pour', 'Enjoy'];
coffee.forEach(forEach => console.log(element));
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

A conditional loop iterates _while_ (or _until_) a condition is met.

```javascript
let hasTime = true;
do {
  // drink coffee
  // contemplate my day until hasTime = false
} while (hasTime);
```

- - -

# Conditional Loops (cont'd)

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
console.log(`The ice caps have melted. The polar bears are gone. We're doomed :(`);
```

**Note**: Be careful using conditional loops because if the condition is never satisfied, they might loop forever.

- - -

# Example

```html
<html>
  <head>
    <title>Console Demo</title>
  </head>
  <body>
    <h1>Climate Change!</h1>
    <script>
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
      console.log(`The ice caps have melted. The polar bears are gone. We're doomed :(`);
    </script>
  </body>
</html>
```

- - -

# Recap

+ An introduction to loops and iteration
+ Javascript loops `for`, `while` and `do`
+ Example (`console.log` is your friend)

- - -

# Exercises

[Exercises](../exercises/exercises.md)



- - -

# Useful Resources

+ [MDN Web Docs - Loops and iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)
+ [DigitalOcean - Using While Loops and Do...While Loops in JavaScript](https://www.digitalocean.com/community/tutorials/using-while-loops-and-do-while-loops-in-javascript)
+ [BBC Bitesize - Iteration in Programming](https://www.bbc.co.uk/bitesize/guides/z3khpv4/revision/7)

- - -

# Thank-you

Dr Steve Huckle

steve@glowkeeper.uk
