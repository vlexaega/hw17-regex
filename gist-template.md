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

Example:
/\d+/ matches one or more digits
/[a-z]{2,4}/ matches lowercase letters with a length between 2 and 4

### OR Operator
The OR Operator which is normally identified by '|' allows one to specify alternative patterns.  It matches either the pattern on the left or the pattern on the right. 

Example:
/apple|orange/ matches either "apple" or "orange"

### Character Classes
Character classes let you define a set of characters that can match a specific position in the text. 

    '\d': Matches any digit (0-9).
    '\w': Matches any word character (alphanumeric and underscore).
    '\s': Matches any whitespace character.
    '.': Matches any character except a newline.

Example:
/\d{3}-\d{2}-\d{4} matches a number such as "123-45-6789"
/\w+/ matches one or more word characters 
### Flags
Flags are optional modifiers.  They can be added at the end of a regex pattern to change the matching behavior. 

    'i': Case-insensitive matching.
    'g': Global matching (find all matches, not just the first).
    'm': Multi-line matching.

Example:
/cat/i matches "cat", "Cat", "CAT", etc., in a case-sensitive manner.
### Grouping and Capturing
Parenthese '()' are used for grouping parts of a pattern together. They also capture the matched substring for later use. 

Example:
/(ab)+/ matches one or more occurrences of "ab" together

### Bracket Expressions
These define a character class inside square brackets '[]' and will match any single character that appears within the brackets. 

Example:
/[aeiou]/ matches any vowel 
/[0-9]/ matches any digit 

### Greedy and Lazy Match
Regex by default is greedy. This means it matches as much text as possible. You can use quantifiers such as '?' to make it lazy, which means it is matching as little as possible. 

Example:
/<.+>/ this is a Greedy Match. Matches "<html>content</html>" as a single match.
/<.+?>/ this is a Lazy Match.  Matches "<html>" and "</html>" as separate matches.
### Boundaries
Boundaries are used to specify positions in the text where matches should occur. Common boundaries are:
    '\b': Matches a word boundary.
    '\B': Matches a non-word boundary.

Example:
/\bapple\b/ matches "apple" as a whole word but not "pineapple"
### Back-references
Back-references allow you to match the same text that was previously matched by a capturing group. 

Example:
/(\d{2})-\1/ matches "11-11", "22-22", etc. but will not match "11-22"

### Look-ahead and Look-behind
Look-ahead and look-behind assertions allow you to check if a pattern is followed or preceded by another pattern without including it in the match. 

Example:
/\d+(?= dollars)/ Matches numbers followed by " dollars" without including " dollars".
/(?<=\$)\d+/ Matches numbers preceded by "$" without including "$".


## Author

This tutorial was written by Alexander Vega, a current student of Columbia University Full Stack Engineering Bootcamp cohort May 2023 - August 2023. 
Check out my work and my GitHub below:
https://github.com/vlexaega 
