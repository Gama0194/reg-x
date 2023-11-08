# Regex Tutorial: Matching an HTML Tag


## Table of Contents
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
- [Matching an HTML Tag](#matching-an-html-tag)
- [Author](#author)

## Anchors
Anchors, such as ^ and $, are used to match the start and end of a line respectively. Anchors are used to match the position of a regex in a string. In our example, ^ denotes the start of the string, and $ denotes the end.

## Quantifiers
Quantifiers specify how many instances of a character or a group of characters should be matched. In our regex, we used + to match one or more occurrences of the preceding character set.

## Grouping Constructs
Grouping constructs, denoted by (), allow you to group multiple characters together and apply quantifiers to them as a single unit. We used grouping to capture the local-part and domain in the email address.

## Bracket Expressions
Bracket expressions, such as [a-z] or [0-9], are used to match any character from a specified set. In our regex, we used them to define the character set for the local-part and domain.

## Character Classes
Character classes, such as \d and \w, are shorthand for matching certain types of characters. We used them to match digits, letters, and certain special characters in the email address.

## The OR Operator
The OR operator, denoted by |, allows you to specify multiple alternative patterns to match. We did not use this operator in our email validation regex.

## Flags
Flags, such as g and i, are used to perform global and case-insensitive matching respectively.

## Character Escapes
Character escapes, such as \. and \\, allow you to match special characters like periods and backslashes literally.

## Matching an HTML Tag
Matching an HTML Tag – /^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)/

HTML tags can be matched using regular expressions. The provided regex pattern can be used to match HTML tags in a string. It captures both opening and closing tags and accounts for potential attributes within the tags. Make sure to use this pattern within the appropriate context and with proper caution, as regular expressions might not cover all complexities of HTML parsing.

## Author
This tutorial was written by Ricardo Esparza. You can find more of my work on GitHub: [https://github.com/Gama0194](https://github.com/Gama0194).
