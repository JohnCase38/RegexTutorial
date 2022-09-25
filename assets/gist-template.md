# R-R-R-Regex! How To:

In this tutorial we are going to break down a Regular Expression. Regex are used to validate text and to search through text.

## Summary

The Regex we are going to use in today's example is an expression used to validate passwords for a sign up form. We want passwords to include an uppercase letter, a lowercase letter, a number, and have a minimum of 8 characters. Here's how we do that:

const re = /^(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.*[a-zA-Z]).{8,}$/g

"1sMyPasswordOK?".search(re);


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
Let's see that again:

const re = /^(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.*[a-zA-Z]).{8,}$/g

"1sMyPasswordOK?".search(re);

The "const re = //" followed by some special characters between the two forward slashes creates the Regex.

### Anchors

### Quantifiers
You can use quantifiers to control how often the proceeding pattern is allowed to occur. 
? = 0 or 1 time
* = 0 or many times
+ = 1 or many times 
Braces are used to explicitly state how many times the pattern is allowed to occur. Use curly braces followed by a {minimum,maximum} number of occurrences.

### OR Operator
Use a vertical bar as a logical OR, to match one string or the other.

### Character Classes
Use a backslash to escape special characters.

### Flags
The lowercase "g" after the second forward slash is called a Flag, which changes the behavior of how the code retrieves matches based on your search pattern. The g flag refers to "global" and will return multiple matches for the same text.


### Grouping and Capturing
Group logic with parentheses. This isolates your code from the rest of the pattern, so you can capture sub strings.

### Bracket Expressions
You can use brackets to define your own custom character sets. [A-Z]

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author
JohnCase38 on github.
