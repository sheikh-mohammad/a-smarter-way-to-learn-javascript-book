# Chapter 08: Concatenating text strings

In Chapter 1 you learned to display a message in an alert, coding it this way.

```javascript
alert("Thanks for your input!");
```

Or you could code it this way.

```javascript
var message = "Thanks for your input!";
alert(message);
```

But suppose you wanted to personalize a message. In another part of your code you've
asked the user for her name and assigned the name that she entered to a variable, `userName`.

(You don't know how to do this yet. You'll learn how in a subsequent chapter.)

```javascript
var userName = "Susan";
```

Now, you want to combine her name with a standard "Thanks" to produce an alert that
says, for example, "Thanks, Susan!"

When the user provided her name, we assigned it to the variable `userName`. This is the
code.

```javascript
alert("Thanks, " + userName + "!");
```

Using the plus operator, the code combines—concatenates—three elements into the
message: the string "Thanks, " plus the string represented by the variable `userName` plus the
string "!"

Note that the first string includes a space. Without it, the alert would read,
"Thanks,Susan!".

You can concatenate any combination of strings and variables, or all strings or all
variables. For example, I can rewrite the last example this way.

```javascript
var message = "Thanks, ";
var banger = "!";
alert(message + userName + banger);
```

Here it is, with three strings.

```javascript
alert("Thanks, " + "Susan" + "!");
```

You can assign a concatenation to a variable.

```javascript
var message = "Thanks, ";
var userName = "Susan";
var banger = "!";
var customMess = message + userName + banger;
alert(customMess);
```

If you put numbers in quotes, JavaScript concatenates them as strings rather than adding
them. This code...

```javascript
alert("2" + "2");
```
...displays the message "22".

If you mix strings and numbers...

```javascript
alert("2 plus 2 equals " + 2 + 2);
```
...JavaScript automatically converts the numbers to strings, and displays the message "2
plus 2 equals 22".