# Regex - Match Between Two Characters<a name='regex_-_match_between_two_characters'></a>

## Description

> Match text between to characters in a string. 

## What is the syntax?

See demo

## Why would you use it?

To extract text between two characters.

## Demo

```
text = "[Markdown - Link to In-Page Anchor<a name='markdown_-_link_to_in-page_anchor.md'></a>]"
regex = /[^\[].+?(?=<)/

# Selected:
# Markdown = Link to In-Page Anchor
```

## Notes

* Demo: https://regex101.com/r/M3diiX/1
