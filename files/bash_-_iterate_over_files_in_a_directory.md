# Bash - Iterate over files in a directory<a name='bash_-_iterate_over_files_in_a_directory.md'></a>

## Description

> A bash for loop that iterates over files in the specified directory.

## What is the syntax?

See demo below

## Why would you use it?

To loop and take action on a list of files in a directory.

## Demo

```
for f in /some/path/; do
  echo $f
done

# Matching by file extension or name

for f in /some/path/*.md; do
  echo $f
done
```

## Notes

* Source https://stackoverflow.com/a/20796617/1491929
