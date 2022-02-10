# Title regexSummary

This document will provide a short summary of what Regex are, what they are used for, and how they function. Specifically I will be focusing on email validation.

## Summary
Regex (shorthand for regular expression)allows you to create search patterns that match, find, and manage text using a string of text. An example code snippet of regex could appear like the following:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This regular expression represents what could be used to match an e-mail address
The command line can also provide usage with Regular expressions, they can be used as within text-editors to find text located in a file.
## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

the '^' is known as a caret and which functions as the primary anchor that matches the beginning of the string or the start of a line if the multiline flag (m) has been enabled. Secondly, the '@' caret is plays the role of  the @ symbol that is seen in a typical e-mail address. Third is the '$' caret which matches the end of a string or the end of a line if the multiline flag (m) has been enabled.


### Quantifiers

A quantifier is a symbol that is used to match one or more preceding character(s) or token(s). Some examples of quanitifers include symbols such as, '+'. ([a-z0-9_\.-]+) the '+' here will match a hyphen if there is one. Quantifiers can also appear as ranges set inside of two curly braces {}. Close to the end of the code snippet appears the quanitifer {2,6} which means there can be a minimum of two or maximum of six characters including and between a - z.

### Grouping Constructs

Grouping constructs function to disconnect portions of characters that are in connection to each other. Standard group constructs are paraenthesis. () the account name is contained within the first () -> ([a-z0-9_\.-]+). the Website is located within the second set of grouping constructs ([\da-z\.-]+). and the final portion of the website usually, '.com', is located within the final grouping construct ([a-z\.]{2,6})

### Bracket Expressions

Bracket expressions are what are used to help define character sets. They look like, '[]'. Inside of these brackets is defined as a character set and used to determine parameters for valid characters.

### Character Classes

Character classes include characters that can be found throughout our example code snippet above.

A 'Literal Character' is any character that does not have ^,-, ], or \. the _ in [a-z0-9_\.-] matches an _ character if it is included in the string.

A 'Backslash' works around special characters to nullify their any unique connitation or special meaning. In this segment of code [a-z0-9_\.-] the escaped character of . nullifies the meaning located outside of a bracket expression and lets it to be passed in with the string.

A 'Range' is defined as using a hyphen between two tokens that each specificy a single character. These ranges can include the two tokens that are used as limits. [a-z0-9_\.-] a-z matches a character between a and z. Whereas the 0-9 range matches any character within that range.

\d displayed ([\da-z\.-]+) matches any digit from 0-9.

### The OR Operator

'+' , '*'. In this code snippet the OR operator '+' means it will match one or more of the bracketed character sets. ([a-z0-9_\.-]+

### Flags

In our example code snippet there are no use of any flags. Flags are tokens that can be used to alter the action of searches. They are completely optional. For instance, instead of stopping at the first match the g flag searches for all matches of a given expression inside of a string.

### Character Escapes

In the example code snippet the \ functions to nullify any special association or meaning a character may have outside of the given representation. For example, the . character servers a different purpose outside of the nullification of the backslash. Also a caret ^ can be used to match the beginning of a string. However, when used with a backslash it nullifies any specific range or character.

## Author

Bradley Hankus is a certified Fullstack Web Developer and recent bootcamp graduate from UCI.

Below are links to GitHub profile as well as the repo for this regexSummary:

[Github Profile](https://github.com/bradleyjosephh)
[Github Regex Link](https://github.com/bradleyjosephh/regexSummary)