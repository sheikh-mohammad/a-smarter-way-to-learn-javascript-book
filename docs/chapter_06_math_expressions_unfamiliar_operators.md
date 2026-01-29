# Chapter 06: Math expressions: Unfamiliar operators

There are several specialized math expressions you need to know. Here's the first one.

```javascript
num++;
```

This is a short way of writing...

```javascript
num = num + 1;
```

It increments the variable by 1.

You decrement using minuses instead of pluses.

```javascript
num--;
```

You can use these expressions in an assignment. But the result may surprise you.

```javascript
var num = 1;
var newNum = num++;
```

In the example above, the original value of num is assigned to `newNum`, and `num` is
incremented afterward. If `num` is originally assigned 1 in the first statement, the second
statement boosts its value to 2. `newNum` gets the original value of num, 1.

If you place the pluses before the variable, you get a different result.

```javascript
var num = 1;
var newNum = ++num;
```

In the statements above, both `num` and `newNum` wind up with a value of 2.

If you put the minuses after the variable, the new variable is assigned the original value,
and the first variable is decremented.

```javascript
var num = 1;
var newNum = num--;
```

`num` is decremented to 0, and `newNum` gets the original value of `num`, 1.

But if you put the minuses before the variable, `newNum` is assigned the decremented, not
the original, value. Both `num` and `newNum` wind up with a value of 0.

```javascript
var num = 1;
var newNum = --num;
```