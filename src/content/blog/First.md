---
title: 'Masterclass in Linux'
description: 'By Kartik Nandagaon(Student Chair IEEE SMVIT SB)'
pubDate: 'Jul 13 2023'
heroImage: '/kali-linux.jpg'
---


## **What happens when your start a computer?**

The first thing that happens on starting a computer is that it executes the software that are there in the BIOS (Basic Input Output System) also referred to as a firmware.

This firmware comes by default in a computer stored in ROM attached to the motherboard. Secondly, it loads the bootloader which is responsible to initialize the OS.
___

## **What is Bootloader?**

It is a program that is responsible for initializing the *Operating System.*

___

 ## **What is OS (Operating System)?**
 
 An operating system (OS) is system software that manages computer hardware, software resources, and provides common services for computer programs. 
 
 ___
## **An operating system should have :**
 - Kernel
 - File system
 - User interface (GUI & CLI)
 - Should be able to manipulate data based on command.
 ___
 
## **What is file system?**

Method or Data Structure that the OS use to store and retrieve the data in the memory.

___

## **What is kernel?**
The kernel is a core component of an operating system and serves as the main interface between the computer's physical hardware and the processes running on it. 
It is also known as bridge between *Software* and *Hardware.*
___

## **What are Most Popular OS ?**
- Microsoft Windows
- Mac OS (Only on apple)
- Linux (UNIX based)
- Android 
- iOS (iPhone Operating system)
___

## **Why use Linux?**
 - Open Source 
 - Support almost all *Programming Languages*
 - Developer Friendly
 - Terminal is superior to CMD
 - Bash Scripting 
 - SSH (Secure Shell)
 ___

  ## **History of Linux**
 
  In **1969** First unix OS created by <u>*Ken Thompson*</u> and <u>*Dennis M. Ritchie*</u>
  10 years later <u>*Richard Stallman*</u> started working on GNU project (BSD , MINIX, etc).

  In **1991** <u>*Linus Torvalds* </u>started working on the "Linux Kernel". This kernel was used in every linux distribution.

>**Linus Torvalds is the father of Linux** 


## **Linux Distributions** 
 - Ubuntu
 - Fedora
 - Arch
 - Kali Linux
 - Pop OS and many more

As a beginner you should start out with Ubuntu.

>**Fun fact : Linux is all about of Keyboard**
___

## **What is Terminal?**

A terminal(black window) is a tool where we are going to write our commands.Start terminal using this command : `ctrl+alt+t` or you can press windows button and type terminal.
___
 
 ## **What is SHELL?**
 A *shell* is a command line interpreter because it executes the commands line by line. 
 
 >**Just like how Python (a programming language) works.**
 ___
 
 ## **What is BASH Programming?**
 
 Every command we are writing on the terminal is a BASH language.
 ___
 
 ## **Shell Format**
 `kali@kali:~$`
  this is the format of shell, lets understand what all this means:
  
  - `kali` : username 
  - `@kali` : hostname
  - `~` : represents the home directory of the user('~' symbol is called tilde)
  - `$` : after this you can start writing command
  ___
  
## **Printing "Hello World" in terminal**
 `kali@kali:~$ echo "Hello World" `
 ___
  
## **pwd (Print Working Directory)**
 The pwd command writes the full pathname of the current working directory to the standard output.<br>
  `kali@kali:~$ pwd`
 ___

 ## **File Structure in Linux**
 The linux file hierarchy structure or the Filesystem Hierarchy Standard (FHS) defines the directory structure and directory contents in Unix like operating systems. It is maintained by the Linux Foundation.
 
 ![image](https://www.linuxtrainingacademy.com/wp-content/uploads/2014/03/linux-folders.jpg)
 ### If you want to know in depth then [Go follow this Link](https://www.geeksforgeeks.org/linux-file-hierarchy-structure/)

 ___
   
   
## **Path of a Directory**
Suppose you have to go `/home` directory in the above diagram. How will u go in terminal?

You can use this way `~$ cd ~/home`

## Basics Commands in Linux
|                Task                          |          Command                 |
|----------------------------------------------|----------------------------------|
|List files                                    |`ls`                              |
|Changed directory                             |`cd <Directory name> `            |
|Clean the terminal                            |`clear`                           |
|Make directory                                |`mkdir <Directory name>`          |
|Make file                                     |`touch <File name>`               |
|Reads data and opens in the terminal          |`cat <file name>`                 |
|Previously executed commands                  |`history`                         |
|Short discription of the command              |`whatis <command>`                |
|Remove directory                              |`rmdir <directory name>`          |
|Copy file or directory                        |`cp <directory/file name>`        |
|Move file or directory                        |`mv <directory/file name>    `    |
|Opens a text editor                           |`gedit <file name>`               |

___

# Debian Command Cheat Sheet

This cheat sheet provides a collection of basic Ubuntu commands along with some useful information and examples. It covers file system navigation, file and directory operations, package management with apt-get, network commands, system information, and basics of the Vim text editor.

## Navigating the File System

- `pwd`: Print the current working directory.
- `ls`: List files and directories in the current directory.
  - `ls -l`: List files and directories in long format.
  - `ls -a`: List all files and directories, including hidden ones.
- `cd`: Change directory.
  - `cd /path/to/directory`: Change to the specified directory.
  - `cd ..`: Change to the parent directory.
- `mkdir`: Create a new directory.
  - `mkdir directory_name`: Create a directory with the given name.
- `rmdir`: Remove a directory.
  - `rmdir directory_name`: Remove the directory with the given name (directory must be empty).

## File and Directory Operations

- `cp`: Copy files and directories.
  - `cp source_file destination_file`: Copy a file to a new location.
  - `cp -r source_directory destination_directory`: Copy a directory and its contents to a new location.
- `mv`: Move or rename files and directories.
  - `mv source destination`: Move a file or directory to a new location.
  - `mv old_filename new_filename`: Rename a file or directory.
- `rm`: Remove files and directories.
  - `rm file`: Remove a file.
  - `rm -r directory`: Remove a directory and its contents.
- `ln`: Create a link to a file or directory.
  - `ln -s source_file link_name`: Create a symbolic link to a file.
  - `ln -s source_directory link_name`: Create a symbolic link to a directory.

## Package Management with apt-get

- `apt-get update`: Update the local package index.
- `apt-get upgrade`: Upgrade installed packages.
- `apt-get install package_name`: Install a package.
- `apt-get remove package_name`: Remove a package.
- `apt-get autoremove`: Remove unused dependencies.
- `apt-get purge package_name`: Remove a package along with its configuration files.

## Network Commands

- `ping`: Send ICMP Echo Request packets to a destination host.
  - `ping host`: Send ICMP Echo Request packets to the specified host.
- `ifconfig`: Display network interface configuration.
  - `ifconfig`: Display configuration for all network interfaces.
  - `ifconfig interface_name`: Display configuration for a specific network interface.

## System Information

- `uname`: Print system information.
  - `uname`: Print the system’s kernel name.
  - `uname -a`: Print all available system information.
- `df`: Display disk space usage.
  - `df`: Display disk space usage for all mounted filesystems.
  - `df -h`: Display disk space usage in a human-readable format.

## Vim Basics

Vim is a powerful text editor with a steep learning curve. Here are some basic commands to get you started:

- Open a file with Vim: `vim filename`
- Switch to insert mode: Press `i`
- Save the file and exit: Press `Esc` to exit insert mode, then type `:wq` and press `Enter`
- Exit without saving: Press `Esc` to exit insert mode, then type `:q!` and press `Enter`
- Search for a pattern: While in normal mode, type `/pattern` and press `Enter`
- Replace text: While in normal mode, type `:%s/old_text/new_text/g` to replace all occurrences of `old_text` with `new_text`

## Copy, Paste, and Cut Operations

- Copy: While in visual mode, select the text to be copied, then type `y`
- Paste: Place the cursor at the desired location, then type `p`
- Cut: While in visual mode, select the text to be cut, then type `d`