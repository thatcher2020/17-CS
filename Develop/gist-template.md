# Regex Tutorial

## Summary

This tutorial will walk you through a regular expression that matches a URL. The regex that you will learn about in this tutorial is:

* Matching a URL: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)


### Anchors

Anchors are used to match a position before, after, or between characters. There are two types of anchors: line anchors and string anchors.

line anchors

- ^ matches the beginning of a line

- $ matches the end of a line

string anchors

- \A matches the beginning of a string

- \Z matches the end of a string


### Quantifiers

Quantifiers are used to match a character or group of characters a specific number of times. There are five types of quantifiers: greedy, reluctant, possessive, lazy, and possessive lazy. The code we are looking at is a greedy quantifier.

the URL: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

is a greedy quantifier because its using ? to say that s in https is optional. The ? is a greedy quantifier because it will match as many s as `https://` has. The greedy quantifier will match the entire string.


### Grouping Constructs

Grouping constructs are used to match a group of characters. There are two types of grouping constructs: capturing and non-capturing. The url is using a grouping construct because it is grouping the characters together to match the url. 

Here is some examples

- (abc) is a capturing group

- (?:abc) is a non-capturing group

the url is using multiple grouping constructs here are some examples

- (https?:\/\/) is a capturing group and is capturing the https://

- ([\da-z\.-]+) is a capturing group and is capturing the domain


### Bracket Expressions

Bracket expressions are used to match a single character out of a list of characters. There are two types of bracket expressions: character classes and character ranges.

- [abc] matches a, b, or c

- [a-z] matches any lowercase letter

some examples in our code would be
[da-Z.-] its matching any lowercase letter, any uppercase letter, any number, and a period or dash

[\/\w \.-] its matching a forward slash, any word character, a space, or a period or dash


### Character Classes

Character classes are used to match a single character out of a list of characters. There are two types of character classes: predefined and user-defined.

- \d matches any digit

- \w matches any word character

some examples in our code would be
[\da-z\.-] its matching any digit, any lowercase letter, a period or dash



### The OR Operator

The OR operator is used to match a character or group of characters. There are two types of the OR operator: alternation and grouping.

- | is the alternation operator

- () is the grouping operator

some examples in our code would be
([\/\w \.-]*)* its matching a forward slash, any word character, a space, or a period or dash and then it is using the * to say that it can match as many times as it wants to

### Flags

Flags are used to modify the behavior of a regex. There are two types of flags: inline and external.

- i is the inline flag and it is saying that it is case insensitive

- g is the inline flag and it is saying that it can match as many times as it wants to


### Character Escapes

Character escapes are used to match a character that has a special meaning in regex. There are two types of character escapes: special and unicode.

- \ is the special character escape and it is saying that the next character is special

- \u is the unicode character escape and it is saying that the next four characters are unicode

some examples in our code would be
\w its saying that the next character is a word character

\Z its saying that the next character is the end of a string



## Author
If you have any questions please reach out to me 

- Email: [email](mailto:thatcherjoe20@gmail.com)

github: [github](thatcher2020)