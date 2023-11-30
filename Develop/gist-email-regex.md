# Understanding Email Regex Tutorial

## Introduction
This tutorial explains the regular expression (regex) used to validate email addresses. Regular expressions are powerful patterns used for matching character combinations in strings, and they are widely used in input validation, search, and text manipulation.

## Summary
The regex we are focusing on is `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. This pattern is commonly used to validate email addresses.

## Table of Contents
1. [Start and End Anchors (`^` and `$`)](#start-and-end-anchors)
2. [Username Match (`[a-z0-9_\.-]+`)](#username-match)
3. [Literal `@` Character](#literal-at-character)
4. [Domain Name Match (`[\da-z\.-]+`)](#domain-name-match)
5. [Period Literal (`\.`)](#period-literal)
6. [Domain Suffix (`[a-z\.]{2,6}`)](#domain-suffix)

## Start and End Anchors
### `^` and `$`
- `^` asserts the start of a line.
- `$` asserts the end of a line.
- These ensure that the pattern matches the entire line, not just a part of it.

## Username Match
### `[a-z0-9_\.-]+`
- This part matches the username of the email.
- It includes lowercase letters (`a-z`), numbers (`0-9`), underscores (`_`), periods (`.`), and hyphens (`-`).
- The `+` allows for one or more characters in this set.

## Literal `@` Character
- The `@` character is a literal in this regex, matching itself.
- It separates the username and domain parts of an email.

## Domain Name Match
### `[\da-z\.-]+`
- Matches the domain name of the email.
- `\d` matches any digit, equivalent to `0-9`.
- The domain name can include letters, numbers, periods, and hyphens.

## Period Literal
### `\.` 
- This matches a literal period (`.`).
- It separates the domain name and the domain suffix.

## Domain Suffix
### `[a-z\.]{2,6}`
- Matches the domain suffix, such as `.com` or `.org`.
- Must be between 2 to 6 characters long.

## Conclusion
This regex is a basic pattern for validating email addresses. Understanding each component helps you modify the regex for different requirements or write your own patterns for other validation purposes.

## About the Author
[ricosantangelo](https://github.com/ricosantangelo)

