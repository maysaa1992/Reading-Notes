**1. The Command Line:**

is a text based interface to the system. You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text.

**2. Navigation**

basics of moving around the system

**pwd**
Print Working Directory - ie. Where are we currently.


**ls**
List the contents of a directory.


**cd**
Change Directories - ie. move to another directory.

**Relative path**
A file or directory location relative to where we currently are in the file system.


**Absolute path**
A file or directory location in relation to the root of the file system.

 **3. More About Files**

 **file**

obtain information about what type of file a file or directory is.

**ls -a**


List the contents of a directory, including hidden files.


**Everything is a file under Linux**


Even directories.


**Linux is an extensionless system**


Files can have any extension they like or none at all.


**Linux is case sensitive**


Beware of silly typos.

**4. Manual Pages**


The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept. 

`man <command>`


Look up the manual page for a particular command.


`man -k <search term>`


Do a keyword search for all manual pages containing the given search term.


`/<term>`


Within a manual page, perform a search for 'term'


`n`


After performing a search within a manual page, select the next found item.

**5. File Manipulation**

Creating a directory is pretty easy.

to creat directory `mkdir [options] <Directory>`


to delet directory `rmdir [options] <Directory>`

Creating a Blank File`touch [options]<filename>`


`cp` ->
Copy - ie. Copy a file or directory.


`mv` ->
Move - ie. Move a file or directory (can also be used to rename).


`rm`->
Remove - ie. Delete a file.