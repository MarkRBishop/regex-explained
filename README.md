# Email Checker - Regex Explained

Hey there! Welcome to this quick and easy tutorial on a regex that checks if an email address is legit. We're gonna break down the following code and see how it ensures a valid email address.
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
``` 

## Summary

This regex code ensures it has all of the elements of an e-mail address and in the correct format.

Username: ([a-z0-9_\.-]+) - Matches the username part, allowing lowercase letters, numbers, underscores, dots, and hyphens.

@ Symbol: @ - Matches the must-have "@" symbol.

Domain: ([\da-z\.-]+) - Matches the domain, allowing numbers, lowercase letters, dots, and hyphens.

Dot: . - Matches the dot between the domain and the top-level domain (TLD).

Top-Level Domain (TLD): ([a-z\.]{2,6}) - Matches the TLD, ensuring it's 2 to 6 lowercase letters or dots.

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

In regex Anchors are the symbols that signify the beginning character '^' and the end character '$' in a string.

### Quantifiers

The + and {2,6} are the quantifiers of the character groups that come before it.
The + means there is one or more (no definit limit) of the character group.
The {2,6} is a difinitive range, in this case its 2 to 6 lowercase letters or dots

### Grouping Constructs

'()' - Parentheses are used for grouping, you'll notice above that each group, such as the check for the username is grouped with its character classes and potentially a quantifier

### Bracket Expressions

Square brackets '[]' are used for character class grouping, for instance in the username part of the code, [a-z0-9_\.-] this checks for matches that are lowercase letters, numbers, dots or hyphens '.-'.

### Character Classes

'\d' in this a case represents any digit, you can also use something like \w for any word.

### The OR Operator

In this example we don't actually use the OR operator which is represented as '|' because we want a specific match, but you can have two different criteria and use the OR operator to verify one set of criteria or the other.

### Flags

In JavaScript you can use flags to change how the regex is interpreted. For example 'g' is for global and 'i' means that its not case-sensitive.

### Character Escapes

Characters like dots, hyphens, and slashes have meaning in regex. To match them literally, we use backslashes '\' as Escapes.

## Author

This was created by Mark Bishop, a buding web developer excited about the possibilities of the future of Web development and Computer Science.

https://github.com/MarkRBishop
