# Regex Tutorial: Introduction

This tutorial aims to provide a comprehensive understanding of regular expressions, a powerful tool for searching and manipulating text.

## Summary
The regex covered in this tutorial is `[a-z]+`, which matches any lowercase letter sequence.

## Table of Contents
- [Component 1: Character Class](#component-1)
- [Component 2: Quantifier](#component-2)
- [Component 3: Grouping](#component-3)

## Component 1: Character Class
A character class matches a single character from a set of characters. It is denoted by enclosing the set of characters within square brackets `[]`. For example, the regex `[aeiou]` will match any lowercase vowel character.

```regex
Regex: [aeiou]
String: "apple"
Match: "a"
```

## Component 2: Quantifier
A quantifier specifies how many times a particular character or group should be matched. The most common quantifiers are `+` (matches one or more occurrences) and `*` (matches zero or more occurrences). For example, the regex `[a-z]+` will match any sequence of lowercase letters.

```regex
Regex: [a-z]+
String: "apple"
Match: "apple"
```

## Component 3: Grouping
Grouping allows you to apply quantifiers and other operators to a specific section of the regex. It is denoted by enclosing the group within parentheses `()`. For example, the regex `([a-z]+)-\1` will match any repeated sequence of lowercase letters separated by a hyphen.

```regex
Regex: ([a-z]+)-\1
String: "hello-hello"
Match: "hello-hello"
```

## Component 4: [Insert Component 4 Title Here]
[Insert explanation of what Component 4 does, using your own words and being thorough.]

```regex
[Insert code snippet of Component 4]
```

[Insert example that meets the requirements of Component 4.]

## About
This tutorial was written by Madilyn Bariekman. 

**Note: To view the properly rendered Markdown, please visit the [public gist](https://gist.github.com/) and ensure that the file has the `.md` extension.