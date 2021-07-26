# Function
# Prerequisite
- basic functions
- if else 

# Content
- Returning Boolean Values from Functions
- Return Early Pattern for Functions
- Counting Cards


[1.Returning Boolean Values from Functions](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/returning-boolean-values-from-functions)
```js
function isLess(a, b) {
  // Only change code below this line
return a < b;
  // Only change code above this line
}

isLess(10, 15);

```

[2.Return Early Pattern for Functions](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/return-early-pattern-for-functions)
```js
// Setup
function abTest(a, b) {
  // Only change code below this line
if (a < 0 || b < 0) {
  return undefined;
}


  // Only change code above this line

  return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
}

abTest(2,2);

```

# Application
[1.Counting Cards](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/counting-cards)
```js
var count = 0;

function cc(card) {
  switch(card) {
    case 2:
    case 3:
    case 4:
    case 5:
    case 6:
      count++;
      break;
    case 10:
    case "J":
    case "Q":
    case "K":
    case "A":
      count--;
      break;
  }

  var betornot = 'Hold'
  if (count > 0) {
    betornot = 'Bet'
  }

  return count + " " + betornot;

}


cc(2); cc('K'); cc(10); cc('K'); cc('A');
console.log(cc(4))

```