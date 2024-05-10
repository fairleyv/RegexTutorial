# Email Validation (a study in Regular Expression)

Regular Expression (regex) is an incredibly useful tool that allows us to ensure the data we receive is the data that
we mean to receive. We encounter it all the time whether a site prompts us to enter a password that meets all 
of the criteria or we're told we need a valid email address to sign up for our free trial. Regular expression is a tool that helps developers ensure that user input is exactly what we expect. Today we're going to learn the basics of regular expression through email validation. 

## Summary
`^([a-zA-Z0-9._%-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,})$`

We're going to be doing a deep dive into the components that make up the regex expression above. Understanding all of the things that make up a regex expression makes understanding the admittedly scary looking piece of code above very simple and easy.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

There are a number of different regex components that can be found in a regex expression. The regex expression we have for validating an email includes the following components: Quantifiers, Anchors, Grouping & Capturing, and Bracket Expression. This is not an exhaustive list, but it does include the most common components found in regex expressions. 

### Anchors
`^([a-zA-Z0-9._%-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,})$`

The anchors in the above regex expression can be found at the beginning and at the very end of the string. Anchors are represented by the `^` and the `$` special characters. The `^` character asserts 

### Quantifiers

### Grouping and Capturing

### Bracket Expressions

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
