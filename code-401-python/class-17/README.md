
# Regular Expression



* **regex** are a sequence of characters used to check whether a pattern exists in a given text (string) or not

## import

      import re

## Characters

* **.** 
  *  A period. Matches any single character except the newline character.

* **^** 
  *  A caret. Matches the start of the string.

* **$** 
  * - Matches the end of string.

* **[abc]** 
  * - Matches a or b or c.
* **[a-zA-Z0-9]** 
  * - Matches any letter from (a to z) or (A to Z) or (0 to 9).

* **\\** 
  * - Backslash. Perhaps, the most diverse metacharacter!!

* **\w** 
  * - Lowercase 'w'. Matches any single letter, digit, or underscore.
* **\W** 
  * - Uppercase 'W'. Matches any character not part of \w (lowercase w).

* **\s** 
  * - Lowercase 's'. Matches a single whitespace character like: space, newline, tab, return.
* **\S** 
  * - Uppercase 'S'. Matches any character not part of \s (lowercase s). 

* **\d** 
  * - Lowercase d. Matches decimal digit 0-9.
* **\D** 
  * - Uppercase d. Matches any character that is not a decimal digit.

* **\t** 
  * - Lowercase t. Matches tab.
* **\n** 
  * - Lowercase n. Matches newline.
* **\A** 
  * - Uppercase a. Matches only at the start of the string. Works across multiple lines as well.
* **\r** 
  * - Lowercase r. Matches return.
* **\b** 
  * - Lowercase b. Matches only the beginning or end of the word.
* **\Z** 
  * - Uppercase z. Matches only at the end of the string.


## shutil

- copyfile() copies contents of the source to destination and raises IOError if it doesn't have the permission to write to the file
- copy() interprets the name of the command line file
- copy2() is like copy() but includes the access and modificiation times in the metadata copied to the new file
- to compy permissions from one file to another use copymode()
- copytree() will copy the directory tree
- copystat() is used to copy other metadata about the file
- move() moves a file or directory from one place to another
- rmtree() will remove a directory and its contents
- make_archive() will make a new archive file
- which() scans a search ptath looking for a named file
- disk_usage() retuns a tuple with the total space, the amount being used, adn the amount remaining