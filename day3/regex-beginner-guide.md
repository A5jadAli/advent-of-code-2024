# Regular Expressions (Regex) - A Beginner's Guide

## What is Regex?

Regular Expressions, or Regex, are powerful patterns used to search, match, and manipulate text. Think of them as a super-powered search and replace tool that can recognize complex text patterns.

## Basic Regex Syntax

### 1. Matching Literal Characters
- Simply type the characters you want to match
- Example: `hello` will match the exact word "hello"

### 2. Special Characters
- `.` (dot): Matches ANY single character
  - `h.t` matches "hat", "hot", "hit"
- `*` (asterisk): Matches 0 or more of the previous character
  - `he*llo` matches "hllo", "hello", "helllo"
- `+` (plus): Matches 1 or more of the previous character
  - `he+llo` matches "hello", "helllo", but NOT "hllo"

### 3. Character Classes
- `[]`: Match any single character in the brackets
  - `[aeiou]` matches any vowel
  - `[0-9]` matches any single digit
- `[^]`: Match any character NOT in the brackets
  - `[^0-9]` matches any non-digit character

### 4. Anchors
- `^`: Start of a line
  - `^hello` matches "hello" only at the beginning of a line
- `$`: End of a line
  - `world$` matches "world" only at the end of a line

### 5. Predefined Character Classes
- `\d`: Any digit (equivalent to `[0-9]`)
- `\w`: Any word character (letters, digits, underscore)
- `\s`: Any whitespace character

## Simple Examples

1. Email Validation (Basic):
   - `^[\w\.-]+@[\w\.-]+\.\w+$`

2. Phone Number:
   - `\d{3}-\d{3}-\d{4}` matches "123-456-7890"

## Practical Tools
- Online Regex Testers:
  - regex101.com
  - regexr.com

## Pro Tips
- Start simple and build complexity
- Use online testers to verify your patterns
- Practice, practice, practice!

## Common Pitfalls
- Overly complex patterns can be hard to read
- Some special characters need escaping with `\`
- Performance can degrade with very complex patterns

## Learning Resources
- MDN Web Docs
- RegexOne.com (Interactive tutorials)
- "Eloquent JavaScript" chapter on Regex
