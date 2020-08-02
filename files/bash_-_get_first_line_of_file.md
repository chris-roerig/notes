# Bash - Get First Line of File<a name='bash_-_get_first_line_of_file.md'></a>

## Description

> Get only the first line from a file.

## What is the syntax?

`head -n 1 /path/to/file`

## Why would you use it?

To get the first line in a file.

## Demo

```
file=/path/to/file.txt
echo "This\nis\na\ntest"
line=$(head -n 1 $file)
echo $line
$ This
```

## Notes

* Source https://stackoverflow.com/a/2439587/1491929
* Note, `head` can return any number of lines from the top. Use `man head` for more info
* To get the last line use `tail -n 1 /path/to/file` 
