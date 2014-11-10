#Introduction to Unix
##Outline and talking points

Biologists of Tyler, Texas

10 November 2014

Dr. Kate Hertweck

Slides available [here](https://github.com/k8hertweck/UTTylerWorkshops/BoTTNov2014/BoTTNov2014.pdf)

*Notes in italics are quick tests of material from earlier in the lesson*

##Introduction in powerpoint: first 5 slides, 10 minutes

##Navigation and file management (20 minutes)

For demo, start from Desktop of computer attached to projector.

Where are we in the computer? 

`pwd` and press `enter`

What is happening when you enter a command?

What is a directory?

Home directory: begins with `/`

What is in this directory?

`ls`

How do we know if these are files or directories?

`ls -F`

Can we make a directory?

`mkdir testFolder`

*How do we test to see if the folder was created?*

Can we move into this directory?

`cd testFolder`

Tab completion is a shortcut for long filenames.

Can we move upwards in the hierarchy, like to move back to the first directory?

`cd ..`

Can we make a file? This command isn't particularly useful because the file is empty.

`touch test.txt`

*Now make another file in `testFolder`*

```
cd testFolder
touch test2.txt
```

OR `cd ..` back up, and from original directory:

`touch testFolder/test2.txt`

*Are there two files called test2.txt? Were you warned that you were overwriting? Be careful or use `-i`*

Can we copy files? 

`cp test.txt test3.txt`

Can we move files around? This can be used to rename files AND move from one folder to another.

```
mv test.txt test4.txt
mv test4.txt testFolder/test5.txt
```

Can we remove files?

`rm test3.txt`

Can we remove a directory?

`rmdir testfolder`

How do we remove a folder with files in it? We can't remove a folder unless it's empty. There are a few ways.

```
rm testFolder/*
rmdir testFolder
```

##Navigation and file management summary, shortcut slide (5 minutes)

##Practicing skills (5 minutes)

*Move into the directory you just downloaded (`biologyHaiku`)*

How do we find the path?

*What files and directories are in `biologyHaiku/`? How many of each?*

What if we forgot the flags (options) for `ls`?

`ls --help`

##Finding things (10 minutes)

How many haikus (files) are there total?

`find . -type f`

Is there another way to do it?

`find . -name "*.txt"`

Wildcards.

Who wrote this haiku?

`grep "Author" haiku1.txt`

Is grep case sensitive?

`grep "author" haiku1.txt`

Who wrote all of these poems?

`grep -r "Author" .`

##Other commands, software, and resources slides from powerpoint (10 minutes)
