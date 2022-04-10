# CSJC_RT
Regex Tutorial

## Using REGEX with JavaScript

```JavaScript’s regular expression flavor is part of the ECMA-262 standard for the language. This means your regular expressions should work exactly the same in all implementations of JavaScript. In the past there were many serious browser-specific issues. But modern browsers do a very good job of following the JavaScript standard for regular expressions. You only need to make sure your web pages have a doctype that requests the browser to use standards mode rather than quirks mode.```

## Summary

```A Regex (regular expression) is a group of symbols which is used to find a specific pattern (match) in a text.```
* Basically, a regular expression is a pattern describing a certain amount of text. Their name comes from the mathematical theory on which they are based. But we will not dig into that. 
* In this tutorial i will explaining a specifics of regex so that we can understand the search pattern the regex defines.
* As a task i will keep Match all letters `A through E` and `a through e` in text by using regular expressions &ndash; `/[A-Z]/g`

## Example javascript code by criteria

* ```const str = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz';```
* ```const regexp = /[A-E]/gi;```
* ```const matches_array = str.match(regexp);```
* ```console.log(matches_array);```

In console we will see ```['A', 'B', 'C', 'D', 'E', 'a', 'b', 'c', 'd', 'e']```
In this example `[A-E]` combination explayning capital latters from `A` (included) to `E` (included) And last `i` is general ignore case flag and letting us to ignore key sensitivity of operator.

## Table of Contents (JavaScript)

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

Anchors belong to the family of regex tokens that don't match any characters, but that assert something about the string or the matching process. Anchors assert that the engine's current position in the string matches a well-determined location: for instance, the beginning of the string, or the end of a line.

Examples
* `^` (caret) -  Matches at the start of the string the regex pattern is applied to.
* `$` (dollar) - Matches at the end of the string the regex pattern is applied to.

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found.

Examples
* `?` (question mark) - 	Makes the preceding item optional. Greedy, so the optional item is included in the match if possible.
* `??` - Makes the preceding item optional. Lazy, so the optional item is excluded in the match if possible.
* `*` (star) - Repeats the previous item zero or more times. Greedy, so as many items as possible will be matched before trying permutations with less matches of the preceding item, up to the point where the preceding item is not matched at all.

### OR Operator

Alternation is the term in regular expression that is actually a simple “OR”. In a regular expression it is denoted with a vertical line character `|`.

### Character Classes

In the context of regular expressions, a character class is a set of characters enclosed within square brackets. It specifies the characters that will successfully match a single character from a given input string.

Examples 
* `[abc]` matches `a`, `b` or `c`.
* `[a-zA-Z0-9]` matches any ASCII letter or digit.

### Flags

A flag is an optional parameter to a regex that modifies its behavior of searching. A flag changes the default searching behaviour of a regular expression. It makes a regex search in a different way. A flag is denoted using a single lowercase alphabetic character.

Example
* `y` (sticky) - Makes the expression start its searching from the index indicated in its lastIndex property.

### Grouping and Capturing

Capturing groups are a way to treat multiple characters as a single unit. They are created by placing the characters to be grouped inside a set of parentheses.

Example
* The regular expression `(dog)` creates a single group containing the letters `d` `o` and `g`.

### Bracket Expressions



### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

Regex tutorial was created by Alik Margaryan. [GitHub](https://github.com/AM0726Github)