# Chapter 07: Math expressions: Eliminating ambiguity

Complex arithmetic expressions can pose a problem, one that you may remember from
high school algebra. Look at this example and tell me what the value of `totalCost` is.

```javascript
var totalCost = 1 + 3 * 4;
```

The value of `totalCost` varies, depending on the order in which you do the arithmetic. If
you begin by adding 1 + 3, then multiply the sum by 4, `totalCost` has the value of 16. But if
you go the other way and start by multiplying 3 by 4, then add 1 to the product, you get 13.

In JavaScript as in algebra, the ambiguity is cleared up by precedence rules. As in
algebra, the rule that applies here is that multiplication operations are completed before
addition operations. So `totalCost` has the value of 13.

But you don't have to memorize JavaScript's complex precedence rules. You can finesse
the issue by using parentheses to eliminate ambiguity. Parens override all the built-in
precedence rules. They force JavaScript to complete operations enclosed by parens before
completing any other operations.

When you use parens to make your intentions clear to JavaScript, it also makes your code
easier to grasp, both for other coders and for you when you're trying to understand your own
code a year down the road. In this statement, the parentheses tell JavaScript to first multiply 3 by 4, then add 1. The result: 13.

```javascript
var totalCost = 1 + (3 * 4);
```

If I move the parentheses, the arithmetic is done in a different order. In this next statement, the placement of the parens tells JavaScript to first add 1 and 3, then multiply by 4. The result is 16.

```javascript
var totalCost = (1 + 3) * 4;
```

Here's another example.

```javascript
var resultOfComputation = (2 * 4) * 4 + 2;
```

By placing the first multiplication operation inside parentheses, you've told JavaScript to
do that operation first. But then what? The order could be..

1. Multiply 2 by 4.

2. Multiply that product by 4.

3. Add 2 to it.

...giving `resultOfComputation` a value of 34.

Or the order could be...

1. Multiply 2 by 4.

2. Multiply that product by the sum of 4 and 2.

...giving `resultOfComputation` a value of 48.

The solution is more parentheses.

If you want the second multiplication to be done before the 2 is added, write this...

```javascript
resultOfComputation = ((2 * 4) * 4) + 2;
```

But if you want the product of 2 times 4 to be multiplied by the number you get when you
total 4 and 2, write this...

```javascript
resultOfComputation = (2 * 4) * (4 + 2);
```
