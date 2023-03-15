# Regex Tutorial: Matching a URL

The following tutorial is using Regular Expression(Regex) to verify if the URL link is valid.

## Summary

As you can see below is the code below which is the Regex pattern to check whether the URL provided is valid.

```
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]_)_\/?$/
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

- `^` - The beginning of a multi-line pattern or a string.
- `$` - The ending of a multi-line pattern or a string.

### Quantifiers

The above Regex pattern shown included 2 Quantifiers; `?` and `+`. The `(https?:\/\/)?` quantifier should equal to 0 or 1 occurence only while `([\da-z\.-]+)` quantifier equals to any string that has one or more occurrences.

### Character Classes

- `\d` - that equates to a single literal character that is a digit
- `\w` - that equates to a word character (alphanumeric character plus underscore)

 Letters and digits are characters that are distinguished as Character classes. This `([a-z\.]{1,4})` character class checks for for small letters from `a to z` at least one to four characters of the preceding string.

### Grouping and Capturing

When it comes to extracting information from strings this operator can be very useful

- `(https?:\/\/)` - this grouping sample makes a value of  `https://`

Also another example could be:
- URL - `http://bootcamp.com/example` - the capture groups would be `(https?:)//([A-z|\.]*)/(.*)`

### Bracket Expressions

- `[\/\w \.-]` - matches a word character (alphanumeric character plus underscore)

### Greedy and Lazy Match

These quantifiers `*, +, ?, {}` are greedy operators, so they increase the match as long as they can through the provided text.
These quantifiers `*?, +?, ??, {}?` are lazy operators, so they decrease the match as short as they can through the provided text.

## Author

Future Junior Developer on his way to success. Have a look at my GitHub [Github Profile](https://github.com/Sakariya95)
