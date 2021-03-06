# Title (replace with your title)
this is a tutorial explaining how the regex expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ is used to validate emails in node.js


## Summary
regular expressions commonly shortened to regex are a type of string that are commonly used to find things that match a certain pattern acting as a search and validation this
one in particular is used for validating emails and this tutorial will explain how it works.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)


### Anchors
^ indicated the beggining of the string whereas $ indicated the ending of the string for validation a visual example of this would be ^validemail@gmail.com$
### Quantifiers
The quantifiers used in this regex include + and {2,6} the + in this quantifier is used to connect the first, middle, and last parts of the expression the visual example would be validemail+ @gmail + .com the {2,6} in this regex is allows for 2-6 characters in the character set of a-z to ensure they match.

### Character Classes
the character classes being used in this regex include a-z, 0-9, /., the a-z is including any letter in its undercase form the 0-9 is there include any number between 0 and 9 and the /. is there to include the @ symbol in the email a-z(validemail) /.(@) a-z(gmail) /. (.) .com numbers are used for uniqueness in a real number 
### Flags
flags used in this regex incluce g which is a global search to ensure you do not create an email that is the same as someone elses email already signed up
### Grouping and Capturing
the capturing groups in this expression are ([a-z0-9_\.-]+) this matches the user email name in this case this is validemail, The second capturing group is ([\da-z\.-]+) which in this case would be the gmail, and ([a-z\.]{2,6}) is used to capture the domain at the end in this case .com
### Bracket Expressions
the bracket expressions used within this regex include [a-z0-9_\.-], [\da-z\.-], and [a-z\.]. the first of these is ensuring any letter a-z is lowercase and matches, any number between 0-9 will be accepted and it is allowing the special characters of _, -, and ., the second of these bracket expression is searching for any lowercase letter or hyphen/period and the last bracket is searching for any lowercase letter and and period
### Greedy and Lazy Match
This regex does not use lazy matching however it does use two instances of greedy matching the first being the + symbol which will match as many times as needed to validate the email and the other being the {2-6} which will do the same for the ending part of the email.
## Author
View my other projects at https://github.com/Chris-McLeod2

