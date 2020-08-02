# Notes

* [Bash - Check if script has arguments](bash_-_check_if_script_has_arguments.md)
* [Bash - Convert Uppercase to Lowercase using awk](bash_-_convert_uppercase_to_lowercase_using_awk.md)
* [Bash - Echo Newline](bash_-_echo_newline.md)
* [Bash - Extract filename from path](bash_-_extract_filename_from_path.md)
* [Bash - Get First Line of File](bash_-_get_first_line_of_file.md)
* [Bash - Iterate over files in a directory](bash_-_iterate_over_files_in_a_directory.md)
* [Bash - Remove first Character From String](bash_-_remove_first_character_from_string.md)
* [Bash - Replace Whitespaces with Underscores](bash-replace_whitespaces_with_underscores.md)
* [C++ - Creating Pointers](c++_-_creating_pointers.md)
* [Markdown - Link to In-Page Anchor](markdown_-_link_to_in-page_anchor.md)



# Bash - Check if script has arguments<a name='bash_-_check_if_script_has_arguments.md'></a>

## Description

> Used for checking if a bash script or function was passed arguments.

## What is the syntax?

`NA`

## Why would you use it?

To change application logic flow depending on the data passed in.

## Demo

```
if [ $# -eq 0 ]
  then
    echo "No arguments supplied"
fi
```

## Notes


---


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


---


# Bash - Echo Newline<a name='bash_-_echo_newline'></a>

## Description

> echo newlines into text 

## What is the syntax?

`echo $`my text\n``

## Why would you use it?

If you want to pump a newline into a file or output while echoing

## Demo

```
echo $'some text with a newline at the end\n' >> myfile.txt
```

## Notes


---


# Bash - Extract filename from path<a name='bash_-_extract_filename_from_path'></a>

## Description

> Get only the file name for a given path. 

## What is the syntax?

`basename /path/to/file.extension`

## Why would you use it?

If you only want to know the file name and not the full path.

## Demo

```
$ basename /home/myuser/some-file.txt
$ some-file.txt
```

## Notes

Source: https://stackoverflow.com/a/965072/1491929
---


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
---


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
---


# Bash - Remove first Character From String<a name='bash_-_remove_first_character_from_string'></a>

## Description

> Removes the first character in string. 

## What is the syntax?

See demo

## Why would you use it?

If you needed to remove the first character of a string in a BASH file...

## Demo

```
echo "some string" | cut -c2-

```

## Notes

Source: https://stackoverflow.com/a/6594179/1491929

---


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

---


# C++ - Creating Pointers<a name='c++_-_creating_pointers.md'></a>

## Description

> Stores the memory location of data

## What is the syntax?

`int * myPointer = new int;`

## Why would you use it?



## Demo

```

```

## Notes


---


# Markdown - Link to In-Page Anchor<a name='markdown_-_link_to_in-page_anchor.md'></a>

## Description

> Create a markdown link that navigates to an element on the page. 

## What is the syntax?

See demo

## Why would you use it?

To create Markdown links that link to elements withing the document.

## Demo

```
[This is the link text](#heading)

## Heading<a name='heading'></a>
```

## Notes

* Source https://stackoverflow.com/a/7335839/1491929
* Markdown treats HTML as HTML

---


