# Regex Tutorial

In this tutorial I will be breaking down the regex code to verify if a user has input a valid email address.

## Summary

The regex code I will be summarizing is `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` . This tutorial will break down all of the characters and symbols to teach you what they mean in chunks/single fashion.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)

## Regex Components

### Anchors

A regex expression always begins and ends with anchors. These anchors are how you will be able to tell when the regex starts and stops. In this regex expression the beginning anchor is `^` and the ending anchor is `$`.

### Quantifiers

Quantifiers specifiy the number of instances a character or group can occur. This regex expression has 2 unique greedy quantifiers in it. The 2 unique greedy quantifiers are `+`, and `{2,6}`. The `+` quantifier allows the engine to match on eor more of the token that it quantifies, while the `{2,6}` quantifier is matching the previous token between 2 and 6 times. 

### Grouping Constructs

Grouping takes the entire expression and breaks it down into the different strings. `()` are used to indicate when a group starts, and stops. In this expression, there is 3 different groups.

Group #1 is `([a-z0-9_\.-]+)`. This is the username of the email account.
Group #2 is `([\da-z\.-]+)`. This is the email service of the domain being used.
Group #3 is `([a-z\.]{2,6})`. This is the extention of the domain being used, like .com, .net, or .gov

### Bracket Expressions

Bracket expressions are inputed to determine what is allowed to be put into the field when creating something using a regex expression and are marked with `[]`. For example the first bracket expression in this regex expressions is `[a-z0-9_\.-]`. This tells us that the user can use characters a-z, numbers 0-9, underscores, periods, and hyphens in this field. The second bracket expression in this regex expression is `[\da-z\.-]`. This tells us that the user can use numbers, characters a-z, periods, and hyphens in this field. The third bracket expression in this regex expression is `[a-z\.]`. This tells us that the user can use characters a-z and periods in this field.


### Character Classes

Character classes are used to match one out of several characters. Character classes are found inside of `[]` called bracket expressions. Examples of character classes would be [a-z] [0-9] and you can find a few of them in this regex expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Author

This was written by me, Nolan Bish. I am working on getting into the web development field and appreciate you taking your time to read my break down! My profile can be found at https://github.com/nolshark .
