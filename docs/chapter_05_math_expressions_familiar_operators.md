# Chapter 05: Math expressions: Familiar operators

Wherever you can use a number, you can use a math expression. For example, you're
familiar with this kind of statement.

```javascript
var popularNumber = 4;
```

But you can also write this.

```javascript
var popularNumber = 2 + 2;
```

You can also write:

```javascript
alert(2 + 2);
```

This displays the messge "4" in an alert box.

When it sees a math expression, JavaScript always does the math and delivers the result.

Here's a statement that subtracts 24 from 12, assigning -12 to the variable.

```javascript
var popularNumber = 12 - 24;
```

This one assigns the product of 3 times 12, 36, to the variable.

```javascript
var popularNumber = 3 * 12;
```

In this one, the number 10 is assigned to a variable. Then 1 is added to the variable, and
the sum, 210, is assigned to a second variable.

As usual, you can mix variables and numbers.

```javascript
var num = 10;
var popularNumber = num + 200;
```

You can also use nothing but variables.

```javascript
var num = 10;
var anotherNum = 1;
var popularNumber = num + anotherNum;
```

The arithmetic operators I've been using, +, -, *, and /, are undoubtedly familiar to you.

This one may not be:

```javascript
var whatsLeftOver = 10 % 3;
```

**%** is the modulus operator. It doesn't give you the result of dividing one number by
another. It gives you the remainder when the division is executed.

If one number divides evenly into another, the modulus operation returns 0. In the
following statement, 0 is assigned to the variable.

```javascript
var whatsLeftOver = 9 % 3;
```