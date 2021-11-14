# Email Matching: Regex Tutorial

Regular expressions, Regex, are tools that developers use on the back-end of their code to validate data users input on the client side. There are many ways to write a Regex to validate, or match code but each expression follows a set of expectations.  

## Summary

The following Regex I will be describing in this tutorital is for matching email adress:

  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Character Escapes](#character-escapes)

## Regex Components


### Anchors
The anchors in this code are the ^ which is the beginning of the code and the $ that marks the end of the code.

### Quantifiers
The + sign in the first two groups of code represents that 1 or more of the items in the group must be included: for example ([a-z0-9_\.-]+), there needs to be at least one letter, number or match one of the special characters inside [].

The {} quantifier on the third group, states that the user needs to have between 2 and 6 of the allowable characters for the end of their email. 

### Grouping Constructs
The parantheses represent groups of code necessary for this regex to match an email. There are 3 groups, the first group is for what comes before the '@' symbol, the second set are the allowable characters for immediately after the @ symbol and the 3rd set represents the end after the '.' 
(first-set)@(second-set).(third-set)
### Bracket Expressions
The bracket expressions in this Regex, lets the application know which characters are allowed for each segment of the code.

### Character Classes
The character class [a-z0-9_\.-] tells the application that a user can use any letter, number or the "_", "," or "-"  for the first segement of the email address. 

[\da-z\.-] tells the application any digit 0-9, any letter or ".", "-" can be used in the second segment of the email address.

[a-z\.] the last set allows any letter a-z or the "." in the final segment of the email. 

### Character Escapes
This code uses "/." in a few places to let the application know that a period is an allowable character.

## Author

I am a student in the University of Minnesota Coding Bootcamp. I am a former teacher who is looking forward to a career in web development. You can view more examples of code in my repoository by visiting https://github.com/kesjoberg.
