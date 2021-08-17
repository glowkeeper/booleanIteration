# Exercises from an Introduction to Loops and Iteration

Below are some exercises that build on the material presented in the [presentation](../presentation/iteration.html). Some of these exercises are tricky -  congratulations if you manage them all! But please do email steve@glowkeeper.uk and ask for help if you need it!

- - -

# Prerequisites

You will need an editor to write your javascript. If you are not using an editor already, [CodeSandbox](https://codesandbox.io/) is a good solution for these exercises, since you'' be able to easily share your work and get help.
- - -

# Template

Below is a template `html` you should use for the exercises:

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

- - -

# Start at the End

During the [presentation](../presentation/iteration.html), `for` loops were introduced. They take the form _{initialisation; condition; increment}_, and the following `for` loop was shown:

```javascript
const coffee = ['Water', 'Kettle', 'Grind', 'Carafe', 'Brew', 'Pour', 'Enjoy'];
for (let i = 0; i < coffee.length; i++) {
  console.log(coffee[i]);
}
```

How would you rewrite the loop so it outputs the list in reverse order (hint: you can _decrement_ as well)? 

Bonus points go to anyone who outputs the console text to the main browser window, instead (**hint**: the presentation outputs to the browser window, so you could get some ideas from there).

- - -

# Start at the End (cont'd)

The [presentation](../presentation/iteration.html) also showed a `forEach` version of the _array_ on the previous slide:

```javascript
const coffee = ['Water', 'Kettle', 'Grind', 'Carafe', 'Brew', 'Pour', 'Enjoy'];
coffee.forEach(element => console.log(element));
```

How could you make _that_ output in reverse order (**hint**: [Array.prototype.reverse](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)).

- - -

# Save the World!

The [presentation](../presentation/iteration.html) came to the rather depressing conclusion that we're doomed:

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
console.log(`The ice caps have melted. The polar bears are gone. WE. ARE. DOOMED :(`);
```

It's your chance to save the world! Change the loop so that it only iterates while the ice caps are _not_ melting and so we end up with 100 polar bears, rather than none! You should also change the messages that get output to something more appropriate. Bonus points go to anyone who outputs the text to the main browser window, instead of the console.

- - -

# Bonus Exercise

The [presentation](../presentation/iteration.md) demonstrated a `for` loop that sums (adds up) all the numbers between 1 and 5:

```javascript
let total = 0;
for (let i = 1; i <= 5; i++) {
  total += i;
}
console.log(total);
```

But actually, you can find the sum of all the numbers up to any given number without using a loop. Please write some loop-free code that writes the sum of 100 to the console.

- - -
