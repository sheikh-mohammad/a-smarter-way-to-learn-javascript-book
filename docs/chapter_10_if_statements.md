# Chapter 10: if statements

Suppose you code a prompt that asks, "Where does the Pope live?"
If the user answers correctly, you display an alert congratulating him.
This is the code.

```javascript
var x = prompt("Where does the Pope live?");
if (x === "Vatican") {
    alert("Correct!");
}
```

If the user enters "Vatican" in the prompt field, the congratulations alert displays. If he
enters something else, nothing happens. (This simplified code doesn't allow for other correct
answers, like "The Vatican." I don't want to get into that now.)

There's a lot to take in here. Let's break it down.

An *if* statement always begins with `if`. The space that separates it from the parenthesis is
new to you. I've taught you to code alerts and prompts with the opening parenthesis running up
against the keyword: `alert("Hi");` Now I'm asking you not to do that in an *if* statement. It's
purely a matter of style, but common style rules sanction this inconsistency.

Following the `if` keyword-plus-space is the condition that's being tested—does the
variable that's been assigned the user's response have a value of "Vatican"?
The condition is enclosed in parentheses.

If the condition tests true, something happens. Any number of statements might execute. In
this case, only one statement executes: a congratulatory alert displays.

The first line of an *if* statement ends with an opening curly bracket. An entire *if* statement
ends with a closing curly bracket on its own line. Note that this is an exception to the rule that a statement ends with a semicolon. It's common to omit the semicolon when it's a complex
statement that's paragraph-like and ends in a curly bracket.

But what about that triple equal sign? You might think that it should just be an equal sign,
but the equal sign is reserved for assigning a value to a variable. If you're testing a variable for a value, you can't use the single equal sign.

If you forget this rule and use a single equal sign when you should use the triple equal
sign, the code won't run properly.

As you might expect, you can use a variable instead of a string in the example code.

```javascript
var correctAnswer = "Vatican";
if (x === correctAnswer) {
    alert("Correct!");
}
```

When a condition is met, you can have any number of statements execute.

```javascript
var correctAnswer = "Vatican";
if (x === correctAnswer) {
    score++;
    userIQ = "genius";
    alert("Correct!");
}
```

> ## CODING ALTERNATIVES TO BE AWARE OF

- Some coders write simple if statements without curly brackets, which is legal. Some put the opening curly bracket on its own line. Some put the whole *if* statement, if it's simple, on a single line. I find it easiest not to have to make case-by-case decisions, so I format all *if* statements the same way, as shown in the example. In the exercises, I'll ask you to follow these style rules for all *if* statements.

- In most cases, a double equal sign `==` is just as good as a triple equal sign `===`. However, there is a slight technical difference, which you may never need to know. Again, to keep things simple, I always use the triple equal sign.