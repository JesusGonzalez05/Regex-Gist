# Regular Expressions (Regex)

Coding languges give developers the opportunity to check for a certain string of characters or numbers, many times you'll utilize the methods inside these languges to do so. Javascript allows it users to take advantage of methods such as `.startsWith()` `.endsWith()` to locate a particular string(s) in a series and return a value that matches that passed into one or more of these methods. Althought useful, regular expresions (or regex for short) can help us widen or narrow the scope we're searching for.  

## Summary

In this Github Gist we will be reviewing the functionality of a regex, focusing primarily on matching hex values. <br>

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` <br>

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
The characters `^` and `$` are considered anchors (anchors dont match but rather assert - meaning they enforce how a string starts or ends). The `^` anchor signifies a string that begins with the characters that follow it (`^abc` would indcate a string starting with the letters abc), The `$` anchor signifies a string that ends with the characters that precedes it (`xyz$` would indcate a string ending with the letters xyz). <br>

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` <br>

In our regex above we see that the `^` anchor is followed by a `#` value signifying the character follwing (or the first character of the string) must be a number.

Similarly before the `$` we notice a `{3}` and a `{6}` (we will review these in futher detail later) indicating the length of the string must either be a 3 or 6 digits long.

### Quantifiers
Similarly to their name quantifiers will determine a character, group, or a character class that must be present in the string for a match to be found. In our hex regex the `?` and `{n}` are going to be our quantifiers. 

The `?` character allows us to match something zero or one time (similar to a conditional), in our regex the `?` character is perceding the `#` character meaning it will look for a value containing a number or not.

The `{n}` character (shown in our regex expression as `{3}` and `{6}` indicates the exact character caount `{n}` times. In our regex, `[a-f0-9]{6}` would indicate any 6 character length string or numerical value and `[a-f0-9]{3}` would indicate any 3 character length string or numerical value.
### OR Operator
As discussed previously our regex is searching for a string or value either `{3}` or `{6}` characters long, but how are we able to search for both lengths? 

The OR operator or as depicted in our regex `|` allows us to join the two expressions `[a-f0-9]{6}` and`[a-f0-9]{3}` and search for both types of string or values by placing them in a set or parenthesis and seperating then with a `|`.
### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author
My name is Jesus Gonzalez I'm a Junior Software Engineer with a background in Retail Management. Trained at the University of Central Florida Coding Bootcamp, acquired skills in JavaScript, CSS, React.js, and responsive web design. Ambitious and innovative problem-solver passionate about continuous learning, collaboration, and developing applications, with a focus on a mobile-first design and development.

Check out my progress and watch me grow!

[Jesus Gonzalez](https://github.com/JesusGonzalez05)

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
