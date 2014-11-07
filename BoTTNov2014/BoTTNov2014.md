#Introduction to Unix

Biologists of Tyler, Texas

10 November 2014

Dr. Kate Hertweck

Outline and talking points, slides available [here](https://github.com/k8hertweck/UTTylerWorkshops/BoTTNov2014/BoTTNov2014.pdf)

##Introduction in powerpoint: first 5 slides, 10 minutes

##Navigation and file management (20 minutes)

Where are we in the computer? 

`pwd` and press `enter`

What is happening when you enter a command?

What is a directory?

Home directory: begins with `/`

What is in this directory?

`ls`

How do we know if these are files or directories?

`ls -F`

Can we move to one of those directories?

`cd`

Can we move upwards in the hierarchy, like to move back to the first directory?

`cd ..`

Can we make a directory?

`mkdir`

Can we remove a directory?

`rmdir` 

Can we move files around?

`mv`

Can we copy files?

`cp`

##Navigation and file management summary, shortcut slide (5 minutes)

##Practicing skills (5 minutes)

Move into the directory you just downloaded (biology Haiku)

What files and directories are in `biologyHaiku/`? How many of each?

##Finding things (10 minutes)

How many haikus (files) are there total?

`find . -type f`

Is there another way to do it?

`find . -name "*.txt"`

Who wrote this haiku?

`grep "Author" haiku1.txt`

Is grep case sensitive?

`grep "author" haiku1.txt`

Who wrote all of these poems?

`grep -r "Author" .`

##Other commands, software, and resources slides from powerpoint (10 minutes)