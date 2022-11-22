# Regex Tutorial

Within this Regex Tutorial I will be discussing what regex is, what it does, how it's used, and why you should use it.

## Summary

- What is Regex? Regex or regular expression is a sequence of characters that define a specific search pattern in text.
- What does it do? Regex is particularly used for defining specialized or general filters.
- How can you use it? Regex is a unique library that consists of different technologies best learned if referenced by documentation.
- Why should you use it? Regex is helpful in search and replace operations. A scenario where regex is useful is searching for a sub-string that matches a pattern and replaces it with something else.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)
- [Sources](#sources)

## Regex Components

### Anchors

Anchors allow users to match a position before or after characters.
- The ^ anchor is used to match the beginning of the text.
- The $ anchor is used to match the end of the text.

### Quantifiers

Quantifiers indicate numbers of characters or expressions to match.
Quantifier types:
- *
- +
- ?
- x{n}
- x{n,}
- x{n,m}

### OR Operator

The OR Operator matches characters or expressions of either the left or the right of the | operator. For example four|4

### Character Classes

Character Classes distinguish kinds of characters between letters and digits.
Character Class types:
- [xyz] [a-c]
- [^xyz] [^a-c]
- .
- \d
- \D
- \w
- \W
- \s
- \S
- \t
- \r
- \n
- \v
- \f
- [\b]
- \0
- \cX
- \xhh
- \/uhhhh
- \u{hhhh} or \u{hhhhh}
- \p{UnicodeProperty}, \P{UnicodeProperty}
- \
- x|y

### Flags

Flags are an optional parameter that modify the searching behavior.
- The i (Ignore Casing) flag is used to make the expression search case-insensitively.
- The g (Global) flag makes the expression search for all occurrences.
- The s (Dot All) flag makes the wild character [.] match newlines as well.
- The m (Multiline) flag is used to enable the multiline mode that instructs the ^ and $ anchors to match the beginning and end of the text as well as the beginning and the end of the line.
- The y (Sticky) flag makes the expression search from the index indicated with the lastIndex property.
- The u (Unicode) flag makes the expression assume individual characters as code points.

### Grouping and Capturing

Groups and Capturing combines multiple patterns as a whole, the captured groups provide extra submatch information when using a regular expression pattern to match against a string.
Grouping and Capturing types:
- (x)
- (?<Name>x)
- (?:x)
- \n
- \k<Name>

### Bracket Expressions

Bracket Expressions match a specific set of single characters, as well as mulit-character collating elements based within the non-empty set of list expressions.
Bracket Expression types:
- Square bracket [] denotes a character class.
- Parentheses () denotes a capturing group.
- Curly bracket {} indicates the number of times to apply the preceding regular expression.

### Greedy and Lazy Match

Greedy match is the longest possible string, while lazy match is the shortest possible string.
* Greedy Match: It allows the engine to match one or more of the token it quantifies.
* Lazy Match: Repeats the token as few times as required, and gradually expands as the engine backtracks through the regex to find an overall match.

### Boundaries

Boundaries match a position that is called a "word boundary".
- Before the first character in a string if the first character is a word character.
- After the last character in a string if the last character is a word character.
- Between two characters in a string if one is a word character and the other is not.

### Back-references

Back-references are regular expression commands which refer to a previous part of the matched regular expression. Back-references are signified with a backslash and a single digit (e.g. '\1').

### Look-ahead and Look-behind

Look-ahead and Look-behind, referred to as look-around when together.
* Look-ahead: Are the patterns that ask JavaScript to look ahead in the string to check for inteded patterns in the string.
* Look-behind: Tells the regex engine to temporarily step backwards in the string, to check if the text inside the look-behind can be matched there.

### Sources

- https://www.javascripttutorial.net/regular-expression-anchors/

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions/Quantifiers

- https://kodejava.org/how-do-i-use-logical-or-operator-in-regex/

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions/Character_Classes

- https://www.codeguage.com/courses/regexp/flags

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions/Groups_and_Backreferences

- https://plainenglish.io/blog/regular-expressions-brackets-f2d6f69ffe13

- https://www.javascripttutorial.net/regular-expression-word-boundaries/

- https://javascript.info/regexp-lookahead-lookbehind

## Author

The author of this Regex Tutorial is Preston Ramsey. Find me on GitHub: [PRamsey02](https://github.com/PRamsey02) | Follow me on LinkedIn: [Preston Ramsey](https://www.linkedin.com/in/preston-ramsey-354ab5244/)