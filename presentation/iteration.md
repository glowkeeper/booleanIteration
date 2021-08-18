# An Introduction to Loops and Iteration

Dr Steve Huckle

steve@glowkeeper.uk

August 2021

- - -

# Lecture Overview

+ Loops and iteration
+ Javascript loops
+ Examples

- - -

# Goals

At the end of this lecture, I hope that you will:

1. Have an understanding of iteration
2. Have a grasp of three types of Javascript loop
3. _Write some code using those loops_!

- - -

# What is Iteration?

Iteration is the process of repeating steps. 

For example, I conduct an iterative ritual each morning:

1. Put water in a kettle and switch it on
2. Meanwhile, grind coffee beans and put the ground coffee in a carafe
3. Put boiling water in the carafe and replace the lid
4. Wait 4 minutes for the coffee to brew, then gently push the plunger all the way down
5. Pour the coffee
6. Repeat from step 1 until I feel ready to go about my day

- - -

# Loops

In programming, iteration is often referred to as _looping_, because when a program iterates, it _loops_ through steps.

- - -

# Javascript Loops

Javascript has three basic looping statements:

1. `for`
2. `while`
3. `do`

- - -

# Count Control Loops

Javascript `for` statements are a form of _count control_ loop, which are useful when you need to iterate a specific number of times.

# for

Javascript `for` statements have a control structure of the form _{initialisation; condition; increment}_

```javascript
const coffee = ['Water', 'Kettle', 'Grind', 'Carafe', 'Brew', 'Pour', 'Enjoy'];
for (let i = 0; i < coffee.length; i++) {
  console.log(coffee[i]);
}
```

The control structure of a `for` loop can appear quite challenging (at first).

- - -

# forEach

When you want to _do something to each element of an array_, `forEach` is probably a better choice.

`forEach`

```javascript
const coffee = ['Water', 'Kettle', 'Grind', 'Carafe', 'Brew', 'Pour', 'Enjoy'];
coffee.forEach(element => console.log(element));
```

- - -

# Conditional Loops

A conditional loop iterates _while_ (or _until_) a condition is met.

# while

```javascript
let done = false;
while (true) {
  // do something that might set done to true
  if (done) {
    break;
  }
  // maybe do something else
}
// do something after the loop
```

# do

```javascript
let hasTime = true;
do {
  // drink coffee
  // contemplate my day until hasTime = false
} while (hasTime);
// do something after the loop
```

- - -

# Example

```javascript
const iceCapsAreMelting = true;
let polarBears = 5;

// Initiate (possible) infinite loop
while (iceCapsAreMelting) {
  console.log(`There are ${polarBears} polar bears.`);
  polarBears--;
  // Terminate the loop if the following condition is true
  if (polarBears === 0) {
    console.log("There are no polar bears left. Boo");
    break;
  }
}
console.log("The ice caps have melted. The polar bears are gone. WE. ARE. DOOMED :(");
```

**Note**: Be careful using conditional loops because if the condition is never satisfied, they might loop forever.

- - -

# Putting it All Together

The html:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Boolean Exercises</title>
    <meta charset="UTF-8" />
    <script src="src/index.js"></script>
  </head>

  <body>
    <h1>Exercises</h1>
    <p id="bears"></p>
    <h2 id="result"></h2>
  </body>
</html>
  ```

# Putting it All Together (cont'd)

The Javascript:

```javascript
const bears = document.getElementById("bears");
const result = document.getElementById("result");

const noBears = "There are no polar bears left. Boo\n";
const doomed = "The ice caps have melted. The polar bears are gone. WE. ARE. DOOMED :(";

const iceCapsAreMelting = true;
let polarBears = 5;

// Initiate (possible) infinite loop
while (iceCapsAreMelting) {
  const numBears = `There are ${polarBears} polar bears`;
  bears.innerText += numBears + "\n";
  console.log(numBears);

  polarBears--;
  // Terminate the loop if the following condition is true
  if (polarBears === 0) {
    bears.innerText += noBears;
    console.log(numBears);
    break;
  }
}

result.innerText += doomed;
console.log(doomed);
```

- - -

# Recap

+ An introduction to loops and iteration
+ Javascript loops `forEach` (`for`), `while` and `do`
+ An example that runs in the browser

- - -

# Exercises

Some [exercises](../exercises/exercises.html)...

- - -

# Slides

+ Presentation - [https://github.com/glowkeeper/booleanIteration/blob/main/exercises/exercises.md](https://github.com/glowkeeper/booleanIteration/blob/main/presentation/iteration.md)
+ Exercises [https://github.com/glowkeeper/booleanIteration/blob/main/exercises/exercises.md](https://github.com/glowkeeper/booleanIteration/blob/main/exercises/exercises.md)

# Useful Resources

+ [MDN Web Docs - Loops and iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)
+ [DigitalOcean - Using While Loops and Do...While Loops in JavaScript](https://www.digitalocean.com/community/tutorials/using-while-loops-and-do-while-loops-in-javascript)
+ [BBC Bitesize - Iteration in Programming](https://www.bbc.co.uk/bitesize/guides/z3khpv4/revision/7)

- - -

# Thank-you

Dr Steve Huckle

steve@glowkeeper.uk
