# Exercises from an Introduction to Loops and Iteration

Some exercises that build on the material presented in the [presentation](../presentation/iteration.html).

- - -

# Prerequisites

You will need an editor to write your javascript. If you are not using an editor already, I recommend trying [Visual Studio Code](https://code.visualstudio.com/).

- - -

# Template

Below is a template you can use for running any of the code you write when solving the exercises below:

```html
<html>
  <head>
    <title>Exercises</title>
  </head>
  <body>
    <h1>Exercises</h1>
    <script>
      // Your javascript code goes in here
    </script>
  </body>
</html>
```

- - -

# Start at the End

During the [presentation](../presentation/iteration.html), `for` loops were introduced. They take the form _{initialisation; condition; increment}_, and the following `for` loop was shown:

```javascript
const coffee = ['Water', 'Kettle', 'Grind', 'Carafe', 'Brew', 'Pour', 'Enjoy'];
for (let i = 0; i < coffee.length; i++) {
  console.log(coffee);
}
```

How would you rewrite the loop so it outputs the list in reverse order (hint: you can _decrement_ as well)? Bonus points go to anyone who outputs the console text to the main browser window (as `<p>` tags), instead.

- - -

# Start at the End (cont'd)

The [presentation](../presentation/iteration.html) also showed a `forEach` version of the _array_ on the previous slide:

```javascript
const coffee = ['Water', 'Kettle', 'Grind', 'Carafe', 'Brew', 'Pour', 'Enjoy'];
coffee.forEach(element => console.log(element));
```

How could you make _that_ output in reverse order?

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
    console.log("There are no polar bears left :(");
    break;
  }
}
console.log(`The ice caps have melted. The polar bears are gone. We're doomed :(`);
```

It's your chance to save the world! Change the loop so that we end up with 100 polar bears, rather than none! Bonus points go to anyone who outputs the console text to the main browser window (as `<h2>` tags), instead.

- - -

# Bonus Exercise

The [presentation](../presentation/iteration.md) demonstrated the following `for` loop:

```javascript
let total = 0;
for (let i = 1; i <= 5; i++) {
  total += i;
}
console.log(total);
```

...which sums (adds up) all the numbers between 1 and 5. But actually, you can find the answer without using a loop. How?

- - -
