# Regex Tutorial

A regex, which is short for regular expression, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input.

## Summary

For this tutorial we will see how regex work and the different parts of that make it function properly.
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors
Anchors are used to indicate the beginning and ending of a string. ^ would be for the start and $ is for the end.

### Quantifiers
Quantifiers are used to specify how many instances of a character, group, or character class must be present in the input for a match to be found. The quantifiers in the regex are {2,6}, which will allow a match range of 2-6 characters for the character set of [a-z\.]. + will connect the users email name + email service + .com

### Character Classes
Character classes are components within our regular expression, They match a character from a specific set. The character class in this expression is \d, which matches a single characters that is a digit from 0-9. 

### Grouping and Capturing
The expression ([a-z0-9_\.-]+) is for the email name which would be group 1. The next expression ([\da-z\.-]+) is for matching the email service which would be group 2. The final expression ([a-z\.]{2,6}) is to match the .com which is group 3.

### Bracket Expressions
Bracket expressions are a list of characters and/or character classes enclosed in brackets []. [a-z0-9_\.-], which is matching any letter a-z and is case senstive. It also matches a character 0-9 and matches the characters _ , - , and .; [\da-z\.-], which is matching a single digit from 0-9, any character a-z (case senstive), and the characters . and -; [a-z\.] matches any character a-z(case senstive) and the character "."

### Greedy and Lazy Match
Greedy means matching the longest possible string.
Lazy means matching the shortest possible string.
For this regrex it only has greedy such as {} when matching `{2,6}, and the + Quantifier, it will match as many times as possible.

## Author
Tavaris Thompson UCF Coding Bootcamp

My github account https://github.com/varis1993

