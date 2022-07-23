# Email_Regex_Tutorial_17.1

Regular Expressions - Regex - are a series of special characters that define a search pattern.

## Summary

This tutorial will help explain how Regex is used to validate an email address using specific search patterns. For example, to match an Email: 
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

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
The characters ^ and \$ are anchors. Start your expressions with: "^", and end them with: "$". (exclude the quotes) 

Notice how there is a ^ and $ at the beginning and end of this regex:
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

### Quantifiers
Quantifiers set the limits of the string that your regex matches. They will usually include the min/max number of characters that your regex is looking for, along with setting other desirable limits.

Quantifiers match as many occurrences of particular patterns as possible. They include the following:
```
* —Matches the pattern zero or more times
```
```
+ —Matches the pattern one or more times
```
```
? —Matches the pattern zero or one time
```
```
{} —Curly brackets can provide three different ways to set limits for a match:
```
```
{ n } —Matches the pattern exactly n number of times
```
```
{ n, } —Matches the pattern at least n number of times
```
```
{ n, x } —Matches the pattern from a minimum of n number of times to a maximum of x number of times
```
in this code:
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
We see + and {} quantifiers in this Regex.
<br>
...{2,6} in this example matches a minimum of 2 times, up to a maximum of 6 times.


### Grouping Constructs

You'll need to use grouping constructs to break regex sections up.

The primary way you group a section of a regex is by using parentheses. Each section within parentheses is known as a subexpression.

For Example:
```
([a-z0-9_\.-]+)
([\da-z\.-]+)
([a-z\.]{2,6})
```
are all present in the example regex:
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)