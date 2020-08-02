# Bash - Replace Whitespaces with Underscores<a name='bash-replace_whitespaces_with_underscores.md'></a>

## Description

> Replaces string spaces with underscores 

## What is the syntax?

`${str// /_}`

## Why would you use it?

Usefule when saving files with names that contain spaces.

## Demo

```
str="This is just a test"
echo ${str// /_}
```

## Notes

* source: https://stackoverflow.com/a/1706459/1491929

