# Regular Expression Tutorial - Matching an Email

Regular expressions are powerful tools used for pattern matching within strings. They are commonly employed in programming languages and text editors to perform various operations like search, replace, and validation. In this tutorial, we will delve into understanding a specific regular expression: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. We will break down each component of this regex and explore its functionality, so you can grasp its pattern and use it effectively in your projects.

## Summary
In this tutorial, we will analyze the regular expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/, which is designed to match valid email addresses. This regex employs a combination of anchors, character classes, quantifiers, and grouping to identify email addresses that follow a specific format. We will break down the regex into its individual components, explaining the purpose of each part, and provide examples to illustrate its usage.

## Table of Contents
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Dot](#dot)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Author](#author)

## Regex Components
The regular expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ consists of several components, each serving a specific purpose:

### Anchors
Anchors (^ and $) are used to specify the start and end positions of the string. In our regex, ^ asserts the start of the string, and $ asserts the end of the string, ensuring the entire string matches the pattern.

### Quantifiers
Quantifiers control the number of times a character or group appears. +: The + quantifier specifies that the preceding element should occur one or more times. {2,6}: The {2,6} quantifier specifies that the preceding element (in this case, the character class [a-z\.]) should occur between 2 and 6 times.

### OR Operator
The OR operator (|) is not explicitly used in this regex.

### Character Classes
Character classes define a set of characters to match. In our regex, [a-z0-9_\.-] matches lowercase letters, digits, underscores, hyphens, and periods. [\da-z\.-]: This character class matches digits, lowercase letters, hyphens, and periods

### Dot
The dot . is used to match any character except a newline

### Grouping and Capturing
Parentheses (...) are used for grouping and capturing subpatterns. Our regex contains three groups to capture different parts of the email address: the username, the domain name, and the top-level domain.

([a-z0-9_\.-]+): This is the first capturing group. It matches and captures the username part of the email address. The character class [a-z0-9_\.-] matches lowercase letters, digits, underscores, hyphens, and periods. The + quantifier allows one or more occurrences of characters in the character class.

([\da-z\.-]+): This is the second capturing group. It matches and captures the domain name part of the email address. The character class [\da-z\.-] matches digits, lowercase letters, hyphens, and periods. The + quantifier allows one or more occurrences of characters in the character class.

([a-z\.]{2,6}): This is the third capturing group. It matches and captures the top-level domain part of the email address. The character class [a-z\.] matches lowercase letters and periods. The {2,6} quantifier specifies that the top-level domain should consist of 2 to 6 characters.

### Bracket Expressions
Bracket expressions ([…]) define a set of characters, similar to character classes. Our regex uses bracket expressions to match specific characters like digits and periods.

### Greedy and Lazy Match
Greedy matching is used by default, meaning the regex tries to match as much as possible. Lazy matching (using +?, *?, ??, or {n,m}?) is not employed in this regex.

## Author
Dele Ayansola is graduate of the Columbia Engineering Full Stack Bootcamp and ardent follower of technology. More about Dele Ayansola - https://github.com/ayandele/professional-portfolio.git
