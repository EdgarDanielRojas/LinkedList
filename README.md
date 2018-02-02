# LinkedList
Linked List project for Advanced Programming Class.
First of all I want to say that most of the code here was provided by the instructor. The only code that is mine is the one included in UserDefined.c as you can see by the commit history. The comments with Doxygen formatting in said file are the instructors as well, with only the comments included in the functions being my own. 
Profesors original code can be found in https://github.com/alopez1327/AdvProgClass/tree/master/Assignments/1_LinkedLists
It is also understood that anyone that will use this knows how to manage the command line.

# Compiling Instructions
If you are using a distribution of Linux or Mac OSX you must first install the glib library

### Linux installation
sudo apt-get install libgtk2.0-dev

### MAC OSX with Homebrew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" 

^Homebrew installation

brew install glib

^ glib installation

## Linux compilation
### Debugging mode on
gcc -D DEBUG *.c \`pkg-config --cflags --libs glib-2.0\` -o LinkedList
### No debugging mode on
gcc *.c \`pkg-config --cflags --libs glib-2.0\` -o LinkedList
## MAC OSX compilation
### Debugging mode on
gcc -D DEBUG *.c -o LinkedList (pkg-config -- cflags -- libs glib-2.0)
### No debugging mode on
gcc *.c -o LinkedList (pkg-config -- cflags -- libs glib-2.0)

# Running the program
The program expects a text file (two are included in this repository) with the format of # Text
LinkedList nodes.txt
