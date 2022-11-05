# Regex

A regex, short for regular expression, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input.

## Summary

A tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does.

Brief summary of the regex with a description and explanation:


Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


This regex group 1 will check an email for charachters (a-z) or numbers (0-9) followed by an @ symbol then;

Group 2 matches any digit character (0-9) and character (a-z) to include "." and "-" then;

Group 3 matches a charcter (a-z) and escapes with "." then;

The quantifier match between 2 and 6.

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

### Anchors, Boundaries:

Some regex tokens do not consume characters. They just assert the matching engine is at a particular place.

^: Beginning of string

$: End of string

### Quantifiers:

Quantifiers set the limits of the string that the regex matches. This exapmple uses:

"+" Quantifier to 1 or more of the preceding Bracket expressions within group 1 and does it again in group 2.

{2,6} Quantifier within the {} provides pattern match between min of 2 and a max of 6 for the preceding bracket expression.

### OR Operator:

The OR operator is expressed by ( | ), but is not contianed in this regex example.

### Character Classes:

The Character class wihtin this example defines the set of characters.

"." and "-" represent the exact matches for those charcters.

a-z matches characters within the english alphabet

0-9_\. matches for numerical values within the range from 0 through 9

\d will match for any Arabic numeral digit.

### Flags:

Flags are placed at the end of the regex at the end of the second / and provide addiitonal functionality or limits. 

There are no flags within this example.

### Grouping and Capturing:

The primary way you group a section of a regex is by using parentheses ( () ). There are three Groups within the boundries to help break up the email matching into separate segments.

### Bracket Expressions:

Inside a set of square brackets ( [] ) represents a range of characters that we want to match. This represent the three separate group matches within the email match.

### Greedy Match:

Quantifiers like * and + are "greedy", meaning that they try to match as much of the string as possible.

"+" Quantifier to 1 or more of the preceding Bracket expressions within group 1 and does it again in group 2.

### Back-references:

[\b] Matches a backspace. If you're looking for the word-boundary character (\b), this example did not contian a back-reference.

### Look-ahead and Look-behind:

Lookarounds do not consume anything. There are typically Look-aheads and Look-behinds and they can be positive or negative. They attempt to match if followed by a varibale or proceeded by it. This example did not contain those tokens. 

## Author

For any other issues or comments please contact me at:

GitHub username: RamRod79

GitHub: https://github.com/RamRod79/regex.git

Email: armando.rod79@gmail.com