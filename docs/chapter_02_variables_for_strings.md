# Chapter 02: Variables for Strings

Please memorize the following facts.

- My name is Mark.
- My nationality is U.S.

Now that you've memorized my name and nationality, I won't have to repeat them,
literally, again. If I say to you, "You probably know other people who have my name," you'll
know I'm referring to "Mark."

If I ask you whether my nationality is the same as yours, I won't have to ask, "Is your
nationality the same as U.S.?" I'll ask, "Is your nationality the same as my nationality?" You'll remember that when I say "my nationality," I'm referring to "U.S.", and you'll compare your nationality to "U.S.", even though I haven't said "U.S." explicitly.

In these examples, the terms "my name" and "my nationality" work the same way JavaScript variables do. My name is a term that refers to a particular value, "Mark." In the same way, a variable is a word that refers to a particular value.

A variable is created when you write var (for variable) followed by the name that you
choose to give it. It takes on a particular value when you assign the value to it. This is a
JavaScript statement that creates the variable name and assigns the value "Mark" to it.

```javascript
var name = "Mark";
```

Now the variable `name` refers to the text string "Mark".

Note that it was my choice to call it `name`. I could have called it `myName`, `xyz`, `lol`, or
something else. It's up to me how to name my variables, within limits.

With the string "Mark" assigned to the variable `name`, my JavaScript code doesn't have to
specify "Mark" again. Whenever JavaScript encounters `name`, JavaScript knows that it's a
variable that refers to "Mark".

For example, if you ask JavaScript to print `name`, it remembers the value that `name` refers
to, and prints...

Mark

The value that a variable refers to can change.

Let's get back to the original examples, the facts I asked you to memorize. These facts can
change, and if they do, the terms my name and my nationality will refer to new values.

I could go to court and change my name to Ace. Then my name is no longer Mark. If I want you to address me correctly, I'll have to tell you that my name is now Ace. After I tell you
that, you'll know that my name doesn't refer to the value it used to refer to (Mark), but refers to a new value (Ace).

If I transfer my nationality to U.K., my nationality is no longer U.S. It's U.K. If I want you
to know my nationality, I'll have to tell you that it is now U.K. After I tell you that you'll know that my nationality doesn't refer to the original value, "U.S.", but now refers to a new value.

JavaScript variables can also change.

If I code...

```javascript
var name = "Mark";
```

`name` refers to "Mark". Then I come along and code the line...

```javascript
name = "Ace";
```

Before I coded the new line, if I asked JavaScript to print `name`, it printed...

Mark

But that was then.

Now if I ask JavaScript to print `name`, it prints...

Ace

A variable can have any number of values, but only one at a time.

You may be wondering why, in the statement above that assigns "Ace" to `name`, the
keyword `var` is missing. It's because the variable was declared earlier, in the original
statement that assigned "Mark" to it. Remember, `var` is the keyword that creates a variable the keyword that declares it. Once a variable has been declared, you don't have to declare it
again. You can just assign the new value to it.

You can declare a variable in one statement, leaving it undefined. Then you can assign a
value to it in a later statement, without declaring it again.

```javascript
var nationality;
nationality = "U.S.";
```

In the example above, the assignment statement follows the declaration statement
immediately. But any amount of code can separate the two statements, as long as the
declaration statement comes first. In fact, there's no law that says you have to ever define a
variable that you've declared.

JavaScript variable names have no inherent meaning to JavaScript.

In English, words have meaning. You can't use just any word to communicate. I can say,
"My name is Mark," but, if I want to be understood, I can't say, "My floogle is Mark." That's
nonsense.

But with variables, JavaScript is blind to semantics. You can use just any word (as long
as it doesn't break the rules of variable-naming). From JavaScript's point of view...

```javascript
var floogle = "Mark";
```

...is just as good as...

```javascript
var name = "Mark";
```

If you write...

```javascript
var floogle = "Mark";
```

...then ask JavaScript to print floogle, JavaScript prints...

Mark

Within limits, you can name variables anything you want, and JavaScript won't care.

```javascript
var lessonAuthor = "Mark";
var guyWhoKeepsSayingHisOwnName = "Mark";
var x = "Mark";
```

JavaScript's blindness to meaning notwithstanding, when it comes to variable names,
you'll want to give your variables meaningful names, because it'll help you and other coders
understand your code.

Again, the syntactic difference between variables and text strings is that variables are
never enclosed in quotes, and text strings are always enclosed in quotes.

It's always...

```javascript
var lastName = "Smith";
var cityOfOrigin = "New Orleans";
var aussieGreeting = "g'Day";
```

If it's an alphabet letter or word, and it isn't enclosed in quotes, and it isn't a keyword that has special meaning for JavaScript, like `alert`, it's a variable.

If it's some characters enclosed in quotes, it's a text string.

If you haven't noticed, let me point out the spaces between the variable and the equal sign,
and between the equal sign and the value.

```javascript
var nickname = "Bub";
```

These spaces are a style choice rather than a legal requirement. But I'll ask you to include
them in your code throughout the practice exercises.

In the last chapter you learned to write...

```javascript
alert("Thanks for your input!");
```

When the code executes, a message box displays saying "Thanks for your input!"

But what if you wrote these two statements instead:

```javascript
var thanx = "Thanks for your input!"
alert(thanx);
```

Instead of placing a text string inside the parentheses of the alert statement, the code
above assigns the text string to a variable. Then it places the variable, not the string, inside the parentheses. Because JavaScript always substitutes the value for the variable, JavaScript displays—not the variable name thanx but the text to which it refers, "Thanks for your input!"

That same alert, "Thanks for your input!" displays.
