# Regex Email Match Tutorial

Regular Expressions or also known as Regex are expressions that define a search pattern used for validation purposes, like email validation, url validation, phone number validation and so on. I will take the time today to talk more about regex to match emails using the expression `/^([a-z0-9_\.\+-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`


## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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

This expression starts and ends with `/`. The anchors used in this regular expression for matching an email are `^` , which indicates the beginning of the string and `$` to indicate the ending of the string. 


### Quantifiers

Quantifiers in this expression is `{2,6}`, which will allow a match range of 2-6 characters for the character set of `[a-z\.]`.


### Grouping Constructs

Capturing group are multiable tokens grouped together and create a capture group for extracting a substring of using a backrefrance.This expression captured substringes as following:
`([a-z0-9_\.-]+)` is capture group #1, which matches the user email name. 
`([\da-z\.-]+)` is capturing group #2, which will match the email service. 
`([a-z\.]{2,6})` is capture group #3, is to capture the .com.


### Bracket Expressions

Bracked expressios match any character in the set. for this expression it matches as follwed 
 `[a-z0-9_\.-]` is matching any letter (case senstive), character 0-9 and matches the characters "_" , "-" , and ".".
 `[\da-z\.-]` is matching a single digit from 0-9, any character a-z (case senstive), and the characters "." and "-".
 `[a-z\.]` matches any character a-z(case senstive) and the character ".".


### Character Classes

The character class in this expression is `\d`, which matches a single digit.


### Character Escapes

`\` is used to escape special characters. 

## Author

This Tutorial was created by Mariam Mohamed, you can view more projects at my [GitHub](https://github.com/Mimimoha) 
