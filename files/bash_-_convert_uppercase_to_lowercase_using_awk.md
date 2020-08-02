# Bash - Convert Uppercase to Lowercase using awk<a name='bash_-_convert_uppercase_to_lowercase_using_awk.md'></a>

## Description

> Converts UPPERCASE string to lowercase using awk.

## What is the syntax?

`awk '{print tolower($0)}'`

## Why would you use it?

File names and paths are easier to work with when the case is the same.

## Demo

```
str="This Is My String"
echo "$str" | awk '{print tolower($0)}' 

$ this is my string
```

## Notes

* There are various ways to do this and not all are OS portable. Large list can be found here https://stackoverflow.com/a/2264537/1491929


