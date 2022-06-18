# Matching an Email with Regex

This is a tutorial on how to create a regular expressions from its core components.

## Summary
I will be describing the different regex components of this particular regular expression. This expression will search for something that is in email format.

```
  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors
```
/^ and $/
```
Our anchors are what determine the beginning and end of what we are looking for. In the beginning of our example, we have "/^" before another component. This means that we are looking for that following component. It also end with "$/" following a component. This means we are looking for it to end with the previous component.
### Quantifiers
```
([a-z0-9_\.-]+)
```
```

([a-z\.]{2,6})
```
Quantifiers determine how many we want of a certain component. The + means that we want to match the preceding character one or more times. In our case (Code Block 1), we have a + following a bracket containing components. This means we want to have one or more of whats in the bracket.

The {} means we want a certain amount of something. It can be formatted like {1} or {1,2} meaning match one time and match 1 to 2 times respectively. In our case, we want two to six of the component that is preceding it.
### Grouping and Capturing
```
([a-z0-9_\.-]+)
```
Grouping and capturing is using parenthesis to trap a certain amount of components and group them together. This final value is what will be used. In this example, we have multiples components contained inside the parentheses. We are taking everything in the brackets one or more times and containing the whole value in the parentheses.
### Bracket Expressions
```
[a-z0-9_\.-]
```
Using brackets [], we can contain a set amount of components and use any of them. In our example, we can have either a lowercase letter, or a digit, or an underscore, or a period, or a hyphen.

## Author

The author of this really enjoys regex because it seems so intimidating, but is actually quite easy to get the hang of. Contact the author at [this link](https://github.com/cole22simpson)
