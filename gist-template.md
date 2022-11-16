# Hex Regex Tutorial!

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

In this tutorial, I will explain how to match a hex value using regular expressions. 

code snippet: 

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`



## Table of Contents

- [Anchors](#anchors)
- [Optional Items](#optional-items)
- [Grouping Constructs](#grouping-constructs)
- [Quantifiers](#quantifiers)
- [Bracket Expressions / Character Classes](#bracket-expressions)
- [The OR Operator](#the-or-operator)

## Regex Components

### Anchors

This regular expression has two anchors. The first anchor is the `^` symbol. This will match the begining of a string. In this case, it will match if there is a # at the begining of the string. 

The next anchor is the `$` symbol. This will match the end of a string. In this case it will match if the pattern is included from the begining to the end of the string. 

### Optional Items

In regular expressions, we use the `?` symbol to make the previous character or capture group optional. The `?` is also a quantifier. 

In this regex, we have `?` to optionally include "#" at the begining of the string. This will only match if there is either a "#" at the begining or no character before the capture group. 

### Grouping Constructs

The `()` symbols define a character grouping/capture group. They allow us to match a part of a string. 

In this case we are going to match either 6 characters that are in the range of a-f and 0-9 or 3 characters that are in the range a-f and 0-9. 


### Quantifiers

Quantifiers look for a specific number of characters matched inside of a capture group. We use the `{}` symbols with a number inside to specify how many characters to match. 


In this case we are looking to match either 6 or 3 characters that are inside the capture group. 

*note: the `?` symbol is also a quantifier. See above in the section on optional items. 

### Bracket Expressions

Bracket expressions (character classes) are a way to match a single charachter out of a possibility of other characters within the same brackets. We use the `[]` symbol to designate a character class and pass in the characters we are hoping to match. 


In our expression we have two character classes, each which match any character between a-f and 0-9. 


### The OR Operator

The `|` symbol designates the OR operator. This operator will match a single regular expression out of many 
possible regular expressions. It is also called "alternation." 

In the Hex Regex above, we use the OR operator to match either a 6 character group or a 3 character group with the constraints described above. 

## Author


Hi I am Tiffany, I am a bootcamp student at University of Washington in Seattle. 

Here is my github profile: [https://github.com/Tiffany-Marko](https://github.com/Tiffany-Marko)