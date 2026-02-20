# Chapter 12: if...else and else if statements

The *if* statements you've coded so far have been all-or-nothing. If the condition tested
true, something happened. If the condition tested false, nothing happened.

```javascript
var x = prompt("Where does the Pope live?");
if (x === "Vatican") {
    alert("Correct!");
}
```

Quite often, you want something to happen either way. For example:

```javascript
var x = prompt("Where does the Pope live?");
if (x === "Vatican") {
    alert("Correct!");
}
if (x !== "Vatican") {
    alert("Wrong answer");
}
```

In this example, we have two *if* statements, one testing for "Vatican," and another testing
for not-"Vatican". So all cases are covered, with one alert or another displaying, depending on
what the user has entered.

The code works, but it's more verbose than necessary. The following code is more
concise and, as a bonus, more readable.

```javascript
if (x === "Vatican") {
    alert("Correct!");
}
else {
    alert("Wrong answer");
}
```

In the style convention I follow, the else part has exactly the same formatting as the *if* part.
As in the *if* part, any number of statements can execute within the else part.

```javascript
var correctAnswer = "Vatican";
if (x === correctAnswer) {
    alert("Correct!");
}
else {
    score--;
    userIQ = "problematic";
    alert("Incorrect");
}
```

*else if* is used *if* all tests above have failed and you want to test another condition.

```javascript
var correctAnswer = "Vatican";
if (x === correctAnswer) {
    alert("Correct!");
}
else if (x === "Rome") {
    alert("Incorrect but close");
}
else {
    alert("Incorrect");
}
```

In a series of *if* tests, JavaScript stops testing whenever a condition tests true.

> ## CODING ALTERNATIVES TO BE AWARE OF

- There are so many ways to format *if* statements and their variations that the range of possibilities is almost endless. I'm partial to the format I've showed you, because it's easy to learn and produces readable code. I'll ask you to stick to this format throughout the exercises.
