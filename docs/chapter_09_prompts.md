# Chapter 09: Prompts

A prompt box asks the user for some information and provides a response field for her
answer.

This code asks the user the question "Your species?" and provides a default answer in the
response field, "human". She can change the response. Whether she leaves the default response
as-is or changes it to something else, her response is assigned to the variable.

```javascript
var spec = prompt("Your species?", "human");
```

Prompt code is like alert code, with two differences.

- In a prompt, you need a way to capture the user's response. That means you need to start
by declaring a variable, followed by an equal sign.

- In a prompt, you can specify a second string. This is the default response that appears in
the field when the prompt displays. If the user leaves the default response as-is and just
clicks **OK**, the default response is assigned to the variable. It's up to you whether you
include a default response.

As you might expect, you can assign the strings to variables, then specify the variables
instead of strings inside the parentheses.

```javascript
var question = "Your species?";
var defaultAnswer = "human";
var spec = prompt(question, defaultAnswer);
```

The user's response is a text string. Even if the response is a number, it comes back as a
string. For example, consider this code.

```javascript
var numberOfCats = prompt("How many cats?");
var tooManyCats = numberOfCats + 1;
```

Since you're asking for a number, and the user is presumably entering one, you might
expect the math in the second statement to work. For example, if the user enters 3, the variable `tooManyCats` should have a value of 4, you might think. But no such luck. All responses to prompts come back as strings. When the string, "3", is linked with a plus to the number, 1, JavaScript converts the 1 to a string and concatenates. So the value of `tooManyCats` winds up being not 4 but "31". You'll learn how to solve this problem in a subsequent chapter.

If the user enters nothing and clicks **OK**, the variable is assigned an empty string: "". 

If the user clicks **Cancel**, the variable is assigned a special value, **null**.

> ## ***CODING ALTERNATIVES TO BE AWARE OF***

- Some coders write `window.prompt` instead of, simply, `prompt`. This is a highly formal
but perfectly correct way to write it. Most coders prefer the short form. We'll stick to the
short form in this training.

- In the example above, some coders would use single rather than double quotation marks.
This is legal, as long as it's a matching pair. But in a case like this, I'll ask you to use
double quotation marks.