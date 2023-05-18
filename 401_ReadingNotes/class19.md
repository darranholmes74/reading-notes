# Class 19 Reading Assignment

1. The primary library for working with regular expressions in Python is the re module. It provides various functions and methods, such as re.search(), re.match(), re.findall(), re.sub() to perform pattern matching, substitution, and manipulation operations on strings using regular expressions.

2. The shutil library in Python provides a high-level interface for file and directory operations. It offers functions to efficiently perform common file management tasks such as copying, moving, renaming, and deleting files and directories.

Example:

```import shutil


source = 'path/to/source/file.txt'
destination = 'path/to/destination/file.txt'


shutil.copy(source, destination)```

3. One automation idea from the assigned material is to create a script that automatically organizes files in a directory based on their file extensions.

To implement this automation:

- Use the os module to retrieve a list of files in the directory.

- Iterate over each file in the list.

- Use regular expressions to extract the file extension from the file name.

- Create a destination directory based on the file extension if it doesn't already exist.

- Use the shutil.move() function to move the file to the appropriate destination directory.


### Things I want to know more about


