# Regex Tutorial: Introduction

This tutorial aims to provide a comprehensive understanding of regular expressions, a powerful tool for searching and manipulating text.

## Summary

I will be explaining regex and the different components.

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

## Regex Components

### Anchors

Anchors are special characters that match a specific position within a string. They do not match any actual characters, but rather they match positions such as the start or end of a line, word, or string. Anchors are used to define boundaries for matching. Some common anchors include:

- `^`: Matches the start of a line.
- `$`: Matches the end of a line.
- `\b`: Matches a word boundary.
- `\B`: Matches a non-word boundary.

### Quantifiers

Quantifiers specify the number of times a character or group should be matched. They allow you to match patterns of varying lengths. Some common quantifiers include:

- `*`: Matches zero or more occurrences of the preceding character or group.
- `+`: Matches one or more occurrences of the preceding character or group.
- `?`: Matches zero or one occurrence of the preceding character or group.
- `{n}`: Matches exactly n occurrences of the preceding character or group.
- `{n,}`: Matches n or more occurrences of the preceding character or group.
- `{n,m}`: Matches between n and m occurrences of the preceding character or group.

### OR Operator

The OR operator, denoted by the pipe character `|`, allows you to specify multiple alternatives in a regex pattern. It matches either the pattern on its left or the pattern on its right. For example, the regex `cat|dog` will match either "cat" or "dog".

### Character Classes

Character classes allow you to match a single character from a set of characters. They are denoted by enclosing the set of characters within square brackets `[]`. Character classes provide a convenient way to specify a range of characters or a set of characters that can match at a particular position. For example:

- `[aeiou]`: Matches any lowercase vowel character.
- `[0-9]`: Matches any digit from 0 to 9.
- `[a-zA-Z]`: Matches any uppercase or lowercase letter.
- `[^0-9]`: Matches any character that is not a digit.

### Flags

Flags are optional modifiers that can be added to a regex pattern to change its behavior. They are usually added after the closing delimiter of the regex pattern. Some common flags include:

- `i`: Case-insensitive matching.
- `g`: Global matching (matches all occurrences, not just the first).
- `m`: Multiline matching (changes the behavior of `^` and `$` to match the start and end of each line, not just the whole string).
- `s`: Dot-all mode (changes the behavior of the `.` metacharacter to match any character, including newline characters).
- `u`: Unicode matching.

### Grouping and Capturing

Grouping allows you to treat multiple characters as a single unit and apply quantifiers or other operators to that unit. It is denoted by enclosing

 the group within parentheses `()`. Additionally, capturing groups allow you to extract and reuse the matched substrings. For example:

- `(ab)+`: Matches one or more occurrences of the sequence "ab".
- `(a|b|c)`: Matches either "a", "b", or "c".


### Bracket Expressions

Bracket expressions, also known as character classes, match a single character from a specified set of characters. They are similar to character classes but provide more flexibility in defining the set of characters to match. Bracket expressions are denoted by enclosing the set of characters within square brackets `[]`. For example:

- `[aeiou]`: Matches any lowercase vowel character.
- `[^0-9]`: Matches any character that is not a digit.

### Greedy and Lazy Match

By default, regex quantifiers are greedy, meaning they match as much as possible. However, sometimes it is desirable to have a lazy match, which matches as little as possible. Greedy quantifiers are denoted by `*`, `+`, `?`, and `{}`. To make a quantifier lazy, you can add a `?` after it. For example:

- `.*`: Matches zero or more characters, as many as possible (greedy).
- `.*?`: Matches zero or more characters, as few as possible (lazy).

### Boundaries

Boundaries allow you to specify positions in a string where matches should occur. They are not actual characters but rather assertions about the position in relation to certain characters. Some common boundary metacharacters include:

- `\b`: Matches a word boundary (the position between a word character and a non-word character).
- `\B`: Matches a non-word boundary (the position between two word characters or two non-word characters).
- `^`: Matches the start of a line or string.
- `$`: Matches the end of a line or string.

### Back-references

Back-references allow you to refer back to previously captured groups within the regex pattern. They are denoted by `\` followed by the group number. Back-references are useful when you want to match repetitive patterns. For example:

- `([a-z])\1`: Matches any repeated lowercase letter.

### Look-ahead and Look-behind

Look-ahead and look-behind assertions allow you to make assertions about the characters that come after or before a match, without including them in the actual match. Look-ahead assertions are denoted by `(?=...)`, and look-behind assertions are denoted by `(?<=...)` or `(?<!...)`. For example:

- `(?=\d+)\w+`: Matches one or more word characters that are followed by one or more digits.

## Author

This tutorial was written by [Madilyn Bariekman](https://github.com/your-github-username).