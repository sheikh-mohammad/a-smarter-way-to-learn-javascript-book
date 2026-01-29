# Chapter 04: Variable Names Legal and Illegal

You've already learned three rules about naming a variable: You can't enclose it in
quotation marks. The name can't be a number or start with a number. It can't be any of
JavaScript's keywords—the special words that act as programming instructions, like `alert`
and `var`.

Here are the rest of the rules:

- A variable name can't contain any spaces.

- A variable name can contain only letters, numbers, dollar signs, and underscores.

- Though a variable name can't be any of JavaScript's keywords, it can contain keywords.   
For example, `userAlert` and `myVar` are legal.

- Capital letters are fine, but be careful. Variable names are case sensitive. A rose is not a
`Rose`. If you assign the string "Floribundas" to the variable `rose`, and then ask JavaScript
for the value assigned to Rose, you'll come up empty.

- I teach the camelCase naming convention. Why "camelCase"? Because there is a hump or
two (or three) in the middle if the name is formed by more than one word. A camelCase
name begins in lower case. If there's more than one word in the name, each subsequent
word gets an initial cap, creating a hump. If you form a variable name with only one
word, like `response`, there's no hump. It's a camel that's out of food. Please adopt the
camelCase convention. It'll make your variable names more readable, and you'll be less
likely to get variable names mixed up.

Examples:

```javascript
userResponse
userResponseTime
userResponseTimeLimit
```

- Make your variable names descriptive, so it's easier to figure out what your code means
when you or someone else comes back to it three weeks or a year from now. Generally,
`userName` is better than `x`, and `faveBreed` is better than `favBrd`, though the shorter names are perfectly legal. You do have to balance readability with conciseness, though.
`bestSupportingActressInADramaOrComedy` is a model of clarity, but may be too much
for most of us to type or read. I'd shorten it.