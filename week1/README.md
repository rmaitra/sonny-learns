## Bash Basics
Unix is an operating system that many computer programmers use. Mac OS is built on Unix. Understanding how to use a Unix terminal is important for developers. On a mac, open up the terminal like so:

![Image of Mac Terminal](http://blog.teamtreehouse.com/wp-content/uploads/2012/09/Screen-Shot-2012-09-25-at-12.57.00-PM.png)

In the terminal you will have a prompt and a cursor blinking. There are several commands that you need to know (the prompt is denoted with the dollar sign $):
```
$ ls                        <--- list the contents of the current directory

$ cd SOME_DIRECTORY_NAME    <--- change current directory to directory called "SOME_DIRECTORY_NAME"

$ mkdir NAME                <--- create a directory with name="NAME"

$ cp FILENAME NEW_FILENAME  <--- copy a file and create a new file with same contents

$ less FILENAME             <--- open a file called FILENAME and read the contents to the screen

$ pwd                       <--- print which directory you are in (sometimes you can get lost)

$ rm FILENAME               <--- remove a file named FILENAME

$ ifconfig                  <--- print your systems network configurations (check your ip address, etc)

$ vi FILENAME               <--- vi is a text-editor for the terminal. you can open up a file and edit it, or you can create a new file.
```
Remember that when you enter a command in the terminal you need to hit enter for the terminal to read the command. 

![gif of bash](https://github.com/rmaitra/sonny-learns/blob/master/week1/bash_basics.gif)

**DON'T BE AFRAID OF THE TERMINAL!** People get scared of the terminal, but it's such a wonderful tool and with the right guidance it can be learned easily! 

## Python Basics
What is python? It's a language. A scripting language to be more specific. It is used by scientists, software developers, accountants, all sorts of people to do anything from manipulating CSV files (your basic Excel files), mining swaths of data across multiple SQL databases, generating jaw-dropping data visualizations, to artificially intelligent bot networks. It's also fairly easy to understand. Coders talk about pointers, or memory allocation, etc; terminology that tends to scare first-time coders. Python removes a lot of that scary behind-the-scenes logic and creates an easy place for coders to learn. 

Let's start by creating a simple python program, open up the terminal, open up your favorite text-editor and create a file:

```python
# this is a comment in python, denoted by the hashtag in front of this text
# none of this will be read by the computer when python compiles this file 
# to binary

print "Hello World"    # <--- this is the print command. we are printing a string to STDOUT (standard output, or in this case, the terminal when we run it)
```
