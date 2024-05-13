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

The anchors in the above regex expression can be found at the beginning and at the very end of the string. Anchors are represented by the `^` and the `$` special characters. The `^` character asserts the beginning of the string and means that the match will start there, while the `$` character asserts the match ends at the end of the string. These anchors used this way mean that the match will include the entire string and won't include any additional characters before or after where the pattern is found. 


### Grouping and Capturing

#### Capturing
Capturing is the process of remembering a part of the input string that matches a specific part of the pattern and is represented by a parentheses`()`. Capturing parts of an expression allows us to use the parts of the inputed string that matter to us. Within our email validation pattern the entire expression is enclosed in the parenthesis and is therefore captured. This allows us to perform operations and methods on the captured input. Since our regex expression captures the entire input it will allow us to use the input beyond simply verifying that the pattern is matched. 

#### Grouping
Grouping in this context allows one to treat multiple characters within an expression as a single unit. Within the above expression we see a lot of groupings including nested groups. Groups are represented by a parentheses `()` as it is in the above pattern. The parenthesese wrapping around nearly the entire expression means that the pattern has to match the entirety of the expression. If there is only a part of the pattern that matches then nothing matches. You can group a pattern together without capturing with a noncapturing group which is represented by a questionmark followed by a colon within the parenthesis `(?:)`. 


### Bracket Expressions


### Quantifiers
Quantifiers do exactly what they sound like they do. They determine the quantity or amount of characters that must match a pattern. In our email validation pattern there are two types of quantifiers. First are the two `+` characters that appear after the `[a-zA-Z0-9._%-]` and `[a-zA-Z0-9.-]` parts of our pattern. the `+` quantifier means that the string being matched must include one or more of the characters from the bracketed set. The second quantifier in our expression is the `{2,}` near the end of the pattern. This quantifier appears after the `[a-zA-Z]` set and means that the string must include 2 or more characters from the bracketed set. 


## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
