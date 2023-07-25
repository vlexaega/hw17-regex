# Regex Decoded

Regular expressions (regex) are powerful tools for text manipulation and patter matching. Normally, they provide a concise and flexible way to search, match and manipulate strings based on specific patterns.  In this tutorial, we will be exploring the essential components of regex along with examples demonstrating their general usage and expected behaviour. 

## Summary

This tutorial will be aiming to provide an understanding of regex by exploring various essential components.  It will cover the general basics of regex such as syntax and detail various features of regex such as Anchos, Quantifiers, OR Operator, Character Classes, Flags, Grouping and Capturing, Bracket Expressions, Greedy and Lazy Match, Boundaries, Back-References, Look-Ahead and Look-Behind.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
Anchors are regex elements used to assert positions in the text, rather than matching specific characters. Two common anchors are:
    '^': The caret anchor asserts the start of a line.
    '$': The dollar sign anchor asserts the end of a line.

Example:
/^Hello/ would match "Hello" only if appearing at the start of a line.
/World$/ would match "World" only if appearing at the end of a line. 
### Quantifiers
Quantifiers specific how many times a character or group of characters should occur. Normally, they allow you to control the number of maths.
    '*': Matches zero or more occurrences.
    '+': Matches one or more occurrences.
    '?': Matches zero or one occurrence.
    '{n}': Matches exactly n occurrences.
    '{n,}': Matches at least n occurrences.
    '{n,m}': Matches between n and m occurrences.

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)