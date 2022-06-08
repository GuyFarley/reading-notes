# Practice in the Terminal

## The Command Line (or Terminal)

- The **Command Line** is a text-based interface system
- The **shell** is the part of the OS that dictates how the terminal will behave, and is responsible for running commands
- **Bash** (Bourne again shell) is the most commonly-used shell

## Basic Navigation

- `pwd` = print working directory (where are we?)
- `ls` = list (what's in our current location?)
- **absolute paths** = location of a file or directory in relation to the root directory (always begin with a '/')
- **relative paths** = location of a file or directory in relation to where we currently are
  - `~` (tilde) = shortcut to home directory
  - `.` (dot) = reference to current directory
  - `..` (dotdot) = reference to parent directory

## More About Files

- Everything is a file (text files, directories, your keyboard, your monitor)
- Linux is extensionless and case sensitive

## Manual Pages

- Pages that explain every command available on your system (what they do, how to execute them, which command line arguments they accept)
- Manual pages can be searched with the following command: `man -k <search term>`

## File Manipulation

- `mkdir` (makes a new directory)
- `rmdir` (deletes a directory)
- `touch` (creates a blank new file)
- `cp` (copy)
- `mv` (move or rename a file)
- `rm` (deletes a file)
- There is no "undo" feature in the Linux terminal! Be careful.

[Back to Home](../README.md)
