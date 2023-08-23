# String Library

A collection of essential string utilities to aid in the manipulation and transformation of strings in JavaScript.

![npm package minimized gzipped size (select exports)](https://img.shields.io/bundlejs/size/%40andrew_dominican%2Fstring-lib)

## Installation

```bash
npm install [string-library]
```

## Usage

```javascript
const {
    capitalize,
    allCaps,
    capitalizeWords,
    capitalizeHeadline,
    removeExtraSpaces,
    kebobCase,
    snakeCase,
    camelCase,
    shift,
    makeHashTag,
    isEmpty
} = require('[string-library]');


capitalize(str)
Description: Converts the first character of a given string to uppercase.
Example: "hello world" returns "Hello world"

allCaps(str)
Description: Converts all characters of a given string to uppercase.
Example: "foo bar" returns "FOO BAR"

capitalizeWords(str)
Description: Capitalizes the first character of each word in a string.
Example: "do all the things" returns "Do All The Things"

capitalizeHeadline(str)
Description: Capitalizes each word except specific small words unless they start the string.
Example: "the most foo in bar" returns "The Most Foo in Bar"

removeExtraSpaces(str)
Description: Removes spaces from the beginning and end of a string and replaces multiple spaces with a single space.
Example: " Hello world! " returns "Hello world!"

kebobCase(str)
Description: Converts a string to kebob-case, removing extra spaces and replacing spaces with hyphens.
Example: " Hello world! " returns "hello-world"

snakeCase(str)
Description: Converts a string to snake_case.
Example: " what the heck " returns "what_the_heck"

camelCase(str)
Description: Converts a string to camelCase.
Example: "Camel Case" returns "camelCase"

shift(str, n)
Description: Takes the first n characters of a string and moves them to the end.
Example: shift('foo bar', 3) returns ' barfoo'

makeHashTag(str)
Description: Converts the given string to a hash tag. Picks the three longest words if more than three words are provided.
Example: "Amazing bongo drums for sale" returns ['#amazing', '#bongo', '#drums']

isEmpty(str)
Description: Returns true if the string is empty or contains only whitespace.
Example: isEmpty(" \n\t\r ") returns true
```
