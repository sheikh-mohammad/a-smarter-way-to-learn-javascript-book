# Chapter 03: Variables for Numbers

A string isn't the only thing you can assign to a variable. You can also assign a number.

```javascript
var weight = 150;
```

Having coded the statement above, whenever you write `weight` in your code, JavaScript
knows you mean 150. You can use this variable in math calculations.

If you ask JavaScript to add 25 to `weight`...

```javascript
weight + 25
```

...JavaScript, remembering that `weight` refers to 150, will come up with the sum 175.
Unlike a string, a number is not enclosed in quotes. That's how JavaScript knows it's a
number that it can do math on and not a text string, like a ZIP code, that it handles as text.
But then, since it's not enclosed in quotes, how does JavaScript know it's not a variable?
Well, because a number, or any combination of characters starting with a number, can't be used
as a variable name. If it's a number, JavaScript rejects it as a variable. So it must be a number.

If you enclose a number in quotation marks, it's a string. JavaScript can't do addition on it.

It can do addition only on numbers not enclosed in quotes.

Now look at this code.

```javascript
var originalNum = 23;
var newNum = originalNum + 7;
```

In the second statement in the code above, JavaScript substitutes the number 23 when it
encounters the variable `originalNum`. It adds 7 to 23. And it assigns the result, 30, to the
variable `newNum`.

JavaScript can also handle an expression made up of nothing but variables. For
example...

```javascript
var originalNum = 23;
var numToBeAdded = 7;
var newNum = originalNum + numToBeAdded;
```

A variable can be used in calculating its own new value.

```javascript
var originalNum = 90;
originalNum = originalNum + 10;
```

If you enclose a number in quotation marks and add 7...

```javascript
var originalNum = "23";
var newNum = originalNum + 7;
```

...it won't work, because JavaScript can't sum a string and a number. JavaScript interprets
"23" as a word, not a number. In the second statement, it doesn't add 23 + 7 to total 30. It does something that might surprise you. I'll tell you about this in a subsequent chapter. For now, know that a number enclosed by quotation marks is not a number, but a string, and JavaScript can't do addition on it.

Note that any particular variable name can be the name of a number variable or string
variable. From JavaScript's point of view, there's nothing in a name that denotes one kind of
variable or another. In fact, a variable can start out as one type of variable, then become
another type of variable.

Did you notice what's new in...

```javascript
var originalNumber = 23;
var newNumber = originalNumber + 7;
```

The statement assigns to the variable `newNumber` the result of a mathematical operation.
The result of this operation, of course, is a number value.

The example mixes a variable and a literal number in a math expression. But you could
also use nothing but numbers or nothing but variables. It's all the same to JavaScript.

I've told you that you can't begin a variable name with a number. The statement...

```javascript
var 1stPresident = "Washington";
```

...is illegal, thanks to that initial "1" in the variable name.

But you can include numbers in variable names, as long as none of them come first. The
statement...

```javascript
var prezWhoCame1st = "Washington";
```

...is legal.

Conveniently, if you specify a number instead of a string as an alert message...

```javascript
alert(144);
```

...or if you specify a variable that represents a number as an alert message...

```javascript
var caseQty = 144;
alert(caseQty);
```

...JavaScript automatically converts it to a string and displays it.