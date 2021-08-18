# Exercises from an Introduction to Loops and Iteration

Below are some exercises that build on the material from the [presentation](../presentation/iteration.html).

Some of these exercises are tricky! Congratulations if you manage them all! But please do email steve@glowkeeper.uk and ask for help if you need it

- - -

# Prerequisites

You will need an editor to write your javascript. If you are not using an editor already, [CodeSandbox](https://codesandbox.io/) is a good solution for these exercises as it allows you to easily share your work and get help.

- - -

# Template

Below is a template _index.html_ you should use for the exercises:

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

# Start at the End

The [presentation](../presentation/iteration.html) showed `forEach` outputting the elements of an _array_:

```javascript
const coffee = ['Water', 'Kettle', 'Grind', 'Carafe', 'Brew', 'Pour', 'Enjoy'];
coffee.forEach(element => console.log(element));
```

How could you make that log to the console in reverse order? Bonus points go to anyone who outputs the text to the main browser window, instead of the console.

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

It's your chance to save the world! Change the loop so that it only iterates while the ice caps are _not_ melting and so we end up with 100 polar bears, rather than none! You should also change the messages that get output to something more appropriate. Again, bonus points go to anyone who outputs the text to the main browser window, instead of the console.

- - -

# Optional Exercise

The [presentation](../presentation/iteration.md) mentioned that the structure of a `for` loop can appear quite challenging on first view. Indeed, the advice was that when you start your programming journey, you might want to avoid using `for` altogether. This exercise is all about avoiding a `for` loop!

```javascript
let total = 0;
for (let i = 1; i <= 5; i++) {
  total += i;
}
console.log(total);
```

That script sums (adds up) all the numbers from 1 to 5 inclusive. But actually, you can find the sum of all the numbers up to any given number without using a loop! Please write some loop-free code that writes the sum of 100 to the console.

- - -
