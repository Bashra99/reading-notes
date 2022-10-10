# FileIO & Exceptions

## Reading and Writing Files


### What Is a File

* a contiguous set of bytes used to store data
* This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable
  * Header: metadata about the contents of the file (file name, size, type, and so on)

  * End of file (EOF): special character that indicates the end of the file

  * Data: contents of the file as written by the creator or editor


* File Paths
  * When you access a file on an operating system, a file path is required

    * Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / or backslash \
    * File Name: the actual name of the file
    * Extension: the end of the file path pre-pended with a period (.) used to indicate the file type

  


* Character Encodings

  * translation from byte data to human readable characters
  * This is typically done by assigning a numerical value to represent a character


### Opening and Closing a File

* invoking the open() built-in function
  * `file = open('dog_breeds.txt')`

*  close a file is to use the try-finally block
   *  `reader = open('dog_breeds.txt')`</br>
`try:`</br>
`    # Further file processing goes here`</br>
`finally:`</br>
`   reader.close()`



### Reading and Writing Opened Files
* There are multiple methods that can be called on a file object to help out reading
  * `.read(size=-1)`</br>
  * `.readline(size=-1)	`</br>
  * `.readlines()`

*  file objects have multiple methods that are useful for writing to a file
  * `.write(string)`</br>
  * `.writelines(seq)`</br>

###   Tips and Tricks

* `__file__`
  * a special attribute of modules, similar to` __name__`

* Appending to a File
  *  `with open('dog_breeds.txt', 'a') as a_writer:`</br>
    `a_writer.write('\nBeagle')`


## Exceptions

### Exceptions versus Syntax Errors

![](https://files.realpython.com/media/

* Syntax errors occur when the parser detects an incorrect statement
  * `  print( 0 / 0 ))`</br>
 `SyntaxError: invalid syntax`

* The arrow indicates where the parser ran into the syntax error
  *  `  File "<stdin>", line 1, in <module>`</br>
`ZeroDivisionError: integer division or modulo by zero`

### The AssertionError Exception

* Instead of waiting for a program to crash midway
*  you can also start by making an assertion in Python
* We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue
* If the condition turns out to be False, you can have the program throw an AssertionError exception.

  * `import sys`</br>
  `assert ('linux' in sys.platform), "This code runs on Linux only."`
* If you run this code  the result would be the following:
  * `Traceback (most recent call last):`</br>
`  File "<input>", line 2, in <module>`</br>
`AssertionError: This code runs on Linux only.`

### The try and except Block: Handling Exceptions

* Python executes code following the try statement as a “normal” part of the program.
* The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.

  * `try:`</br>
`    linux_interaction()`</br>
`except:`</br>
`    print('Linux function was not executed')`</br>

  * `    with open('file.log') as file:`</br>
`        read_data = file.read()`</br>
`except FileNotFoundError as fnf_error:`</br>
`    print(fnf_error)`</br>
  

### The else Clause

*  `try:`</br>
 `   linux_interaction()`</br>
`except AssertionError as error:`</br>
 `   print(error)`</br>
`else:`</br>
`    print('Executing the else clause.')`