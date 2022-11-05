# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Regex, short for regular expression, is a string that lets you create patterns to help locate, manage, and match text. 

An example is this email matching regex.
```
(/[w._%+-]+@[\w.-]+\.[a-zA-Z]{2,4}/)
```

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

Anchors are characters within the regular expression that allow the user to match strings that begin with or ends with (or both) certain characters. 

Examples of Anchors are as follows:

* `^` - matches any string that start with the anterior word
* `$` - matches a string that end with preceeding word before the character
* Examples:

```
^Hello          matches any string starting with `Hello`
World$          matches any string ending with `World`
^Hello World$   matches exact string
goodbye         matches any string that has the exact text `goodbye` in it
```

### Quantifiers

### OR Operator

### Character Classes

Character Classes (Character Set) tells the regex engine to match only one out serveral specific characters, such as digits, words, or whitespace.

Examples of Character Classes are as follows:

```
\d    matches a single any digit 0-9
\w    matches a single any character that is a-z
\s    matches ` `
.     matches any character
\D    matches a single non-digit character
\W    matches a single any non-character that is a-z
\S    matches a single non-` `
```

### Flags

Flags are optional parameters that we can add to a plain expression to make it search in a different way. Each flag is denoted by a single alphabetic character, and serves different purposes in modifying the expression's searching behavior.

Examples of Flags are as follows:
```
/Hello/g   matches all `Hello` in the test
/Hello/m   matches the beginning and ending of each line with `Hello`, rather than the whole string `Hello` itself
/Hello/i   matches all `hello` despite case (Hello, hEllo, heLlo, hellO, hello, HELLO all match)
```

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

Not to be confused with actual characters, simply put, Boundaries are the places between characters. A Boundary should be thought of as a wall between any adjacent characters.
There are two types of Boundaries, **Word** and ***Non-Word**, each denoted by a specific character. 

Examples of Boundaries are as follows:
```
`Hello World` has 12 total Boundaries with 8 Word Boundaries as seen below:
|H|e|l|l|o| |W|o|r|l|d|
^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^
N W W W W N N W W W W N  -  N = Nonword Boundary \ W = Word Boundary
\bxyz\b     matches a "whole words only search" for the string `xyz`
\Bxyz\B     matches only if the pattern is fully surrounded by word characters `txyzt` would match the string `xyz` because it only has word boundaries
```

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
