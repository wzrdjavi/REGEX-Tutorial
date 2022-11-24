# REGEX-Tutorial

A regex, which is short for regular expression, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input.

For example, the following regular expression can be used to verify that user input is a valid email address:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ . 

## Summary

The regex expression that I will explaining today is the one that makes up an email address. (/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/) , Each one of these verifys that the user enters a correct email address and in a correct format. I will be going over the characters of the expression and how they work together to allow emails to work.

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
For this tutorial, the email regex componets is - (/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/)

### Anchors
the anchors are the ^ and the $ at the beginning and end of the expression. 
This is what tells the computer to look at everything in between. 

### Quantifiers
A quantifier is used to determine how many times a specific character or sequence of characters needs to be present in order to match. 
"+" adds the values within the parentheses {2,6} check the length of the string between 2 and 6 characters.

### OR Operator
The "OR" operator within a regular expression is defined by using "|", which is an element. or the 'Alternate' operator which performs either match ro whatever is side by side of the "|".

### Character Classes
A character class matches only a single character.
Since it only matches one character class, gr[ae]y does not match graay, or graey. 
You can find a word, even if it is misspelled, such as sep[ae]r[ae]te or li[cs]en[cs]e. You can find an identifier in a programming language with [A-Za-z_][A-Za-z_0-9]*. You can find a C-style hexadecimal number with 0[xX][A-Fa-f0-9]+.

### Flags
Flags are placed at the end of a regex, after the second slash, and they define additional functionality or limits for the regex.
-  g—Global search: the regex should be tested against all possible matches in a string.

### Grouping and Capturing
Grouping occurs when the () is used. This indicates a group of the string being comapared to a regular expression. 
Our email regular expression would be /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Bracket Expressions
A bracket expression is anything inside of square brackets ([]) represents the range of characters we want to match. 
- username: ([a-zA-Z0-9._-]+)
- email host name: ([a-zA-Z0-9._-]+)
- domain: ([a-zA-Z]{2,4})

### Greedy and Lazy Match
THIS EXPRESSION DOESN'T HAVE GREEDY OR LAZY MATCHES.

### Boundaries
THIS EXPRESSION DOESN'T STATE ANY BOUNDARIES. 

### Back-references
THIS EXPRESSION DOES NOT HAVE ANY BACK REFRENECES.

### Look-ahead and Look-behind
THIS EXPRESSION DOES NOT INCLUDE LOOK A-HEAD OR LOOK-BEHIND COMPONETS.