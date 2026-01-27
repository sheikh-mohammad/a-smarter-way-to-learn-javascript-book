# Chapter 1: Alerts

An alert is a box that pops up to give the user a message. Here's code for an alert that
displays the message "Thanks for your input!"

```javascript
alert("Thanks for your input!");
```

`alert` is a keyword—that is, a word that has special meaning for JavaScript. It means,
"Display, in an alert box, the message that follows." Note that alert isn't capitalized. If you
capitalize it, the script will stop.

The parentheses are a special requirement of JavaScript, one that you'll soon get used to.
You'll be typing parens over and over again, in all kinds of JavaScript statements.

In coding, the quoted text "Thanks for your input!" is called a text string or simply a
string. The name makes sense: it's a string of characters enclosed in quotes. Outside the coding
world, we'd just call it a quotation.

Note that the opening parenthesis is jammed up against the keyword, and the opening
quotation mark is hugging the opening parenthesis. Since JavaScript ignores spaces (except in
text strings), you could write...

```javascript
alert("Thanks for your input!");
```

But I want you to know the style conventions of JavaScript, so I'll ask you to always omit
spaces before and after parentheses.    

In English, a careful writer ends every declarative sentence with a period. In scripting, a
careful coder ends every statement with a semicolon. (Sometimes complex, paragraph-like
statements end with a curly bracket instead of a semicolon. That's something I'll cover in a
later chapter.) A semicolon isn't always necessary, but it's easier to end every statement with a
semicolon, rather than stop to figure out whether you need one. In this training, I'll ask you to
end every statement (that doesn't end with a curly bracket) with a semicolon.

> ## CODING ALTERNATIVES TO BE AWARE OF

- Some coders write `window.alert` instead of, simply, `alert`. This is a highly formal but
perfectly correct way to write it. Most coders prefer the short form. We'll stick to the
short form in this training.
- In the example above, some coders would use single rather than double quotation marks.
This is legal, as long as it's a matching pair. But in a case like this, I'll ask you to use
double quotation marks.
