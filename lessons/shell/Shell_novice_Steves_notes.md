 # Shell novice: Steve's notes and extras!

## Setup

Please download the data files and install the software is the pre-session because we won’t have time in the main session.

For both of these see the link: 
http://swcarpentry.github.io/shell-novice/setup.html

I recommend that you tidy up your desktop (perhaps put everything into a folder so that only the file you need for this workshop are on the desktop). OR MAYBE A SECOND FOLDER CALLED DC-DESKTOP. Put the data file onto your desktop (or your second desktop folder). The key thing is that you should know where it’s stored.)



## The Blurb (extra!)

We’re going to start an adventure in coding – it’s just like any language – practise is key– so just follow along. What I start put in the chat of you have, or haven’t done any coding before and what coding languages you’ve used. 

Try and follow me with your typing, but don’t fall to far behind. I will show you all a couple of shortcuts early on to which will reduce the amount of typing you need to do. If I move onto something else, while you’re still typing away, just sit-back and let me do the work, and join in whenever you’re ready. SWC has full notes online, so you can catch up at the breaks or during the exercises.

## Introduction 

All of you I’m sure will have used a Graphic User Interface. This is the very common point and click, drag and drop is easy and has revolutionised the ‘accessibility’ of computers (so of us are old enough to remember computers before mice and windows!)

This is what my first experience of computers was:

[Evan-Amos, CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0) 
[, via Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Sinclair-ZX81.png")

<img width="512" alt="Sinclair-ZX81" src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8a/Sinclair-ZX81.png/512px-Sinclair-ZX81.png"/>

 It plugged into the family TV and files were loaded and saved on a tape recorder (which was like an old fashioned, analogue MP3 player). The user would type commands onto the keyboard, anf the commands are written on the keyboard (if you look closely enough). If you wanted to use computers you had to *code*, using the command line interface (or CLS). 
 
 About 10 years later I bought one of these to write my final year dissertation and PhD on. *Actually Id didnt have enough money to buy the 1040ST, only the cheaper 520ST)

 [© Bill Bertram, 2006, CC BY-SA 2.5](https://creativecommons.org/licenses/by-sa/2.5), [via Wikimedia Commons](https://creativecommons.org/licenses/by-sa/3.0) 
[, via Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Atari_1040STf.jpg)

<img width="512" alt="Atari 1040STf" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/39/Atari_1040STf.jpg/512px-Atari_1040STf.jpg"/>
 
 Here you can see a proper keyboard, monitor and a mouse that allows the user to point-click, drag-drop and so on. 
These Graphic User Interface's (GUI's) have revolutioned computer accessibility. GUI's are easy to use, conceptually simple, and flexible, but not scalable (imagine having to transfer a line of data from a thousand individual files to an Excel spreadsheet using a GUI!). 

 To get scalablilty of a repeatative task we should start to look at writing some code. There are lots of different ways of writing code, but we’ll focus in this session on Unix. Unix is a command-line interface (the user writes lines of code that perform operations).

This morning we will look at Unix as a shell program. A shell is like a simple program that takes our typed instructions, interprets them for the computers kernel or operating system, and the kernel controls the hardware of the computer. 

We'll be using a version of Unix called Bash. Bash started in 1979 as Bsh (which stood for [Bourne Shell](https://en.wikipedia.org/wiki/Bourne_shell), after it's creator, Stephen Bourne). About 10 years later it was updated and re-written as Bash (which stood for the Bourne again Shell).

### Off script exercise
Type $

`echo “Hello World” `

Press return.

So getting the computer to output ‘Hello World’ is traditionally the first line of code you write when learning a new programming language. There is an unofficial metric called Time To Hello World and that is a measure of how easy a programing language is to install and use. 

Type $ 

`echo “Hello Steve” # This is my name`

Press return.

Note that the text after the comment hasn’t shown up: this is because the text after the code is interpreted as a ‘comment’, sometimes called REM (in versions of Basic), but apostrophes and slashes might be used in other programming languages too. Please remember the hash # is your friend (find it on your keyboard and remember it) comments in code are absolutely essential.

### Essential shorts (off script)

Two tricks: the arrow keys and the tab key. 

These are shortcuts that will mean you don’t have to rewrite lines of code several times.
Press the arrow key once and twice and you will see the previous code lines appear. The lines can be reused, or modified.

Type ec and then tab. You will see the shell fills in the code for you. I’ll be using tab a lot so just try it a few times and make sure use know where your tab button is.

### Back on script

Try the ls and ks examples
 
Just to say that we’re not going to do Nellie exercises. You can go through it yourself over lunch if you want, but we’re compressing a 4:30 hr session into about 2:30 hours, so somethings got to go.

## Navigating files and directories (folders)

If you get lost’ in your directory type 

`cd`

only and it will get you back to your home directory. I'll give an example of ‘getting lost’ by going to the root directory and then getting back ‘re-spawn’.

Do the pwd (print working directory) examples.

Go to the folders diagrams on the SWC pages. Read the text and use the marker to highlight the parts of the file structure with the tablet pen. We call this a ‘path’.


Look at the ls –F  file and highlight command-option-argument. The ls gives a list, the –F shows the different types of file (which are coloured anyway).


Look at the syntax (the arrangement of words in a language). We have:
1. command
2. option (also called switch or flag) 
3. argument. 

Do the ls –F / example. Where / is a ‘shorthand’ for the root directory.

You will see that my ls –F looks the same as my ls! Why is that? 

We’ll on Git Bash (which is what I’m using), ls is a command, by it is also an alias. If I type `alias ls`, then it tells me that unix had modified ls for me so that I can customise my output.

If you want to modify you ls (or any other function catch us in the breaks). The code in Unix is  `alias ls = ‘ls –F’`

**NOTE** that the man example doesn’t work in my version

For the exercise: -h, --human-readable       with -l and -s, print sizes like 1K 234M 2G etc and   -l                         use a long listing format

Do the exploring other directories material.

Cover the idea of relatives and absolute paths.

## Summary table/cheat sheet

| Commands|Action|
|-------|---------------|
|cd| Change directory (`cd` only will take you back to your home directory)|
|ls|Lists the files and folders|
|pwd|Print working directory - where you are now|

|Shortcuts|Meaning/effect|
|---------|---------------|
|. (one dot)| Current directory|
|.. (two dots)| Parent directory (go up up in the file path)|
|- (one dash)|The last working directory|
|/ |The root directory|
|~ (tilde)| The users home directory|
|Tab |Completes your command or file/folder|
|Up/down arrow|Recalls your previous code|

# Working with files and directories

This will be following the Softwate Carpentries lesson very closely.

## Summary table/cheat sheet

| Commands|Action|
|-------|---------------|
|mkdir| Make a directory (new folder!)|
|nano|Text editor (we use it to make a new files)|
|rm|Remove/delete a file|
|rmdir|Remove/delete a directory|
|mv|Move, or rename, a file or directory|
|cp|Copy a file (use –r, recursive, to copy a folder)|

# Pipes and Filters (or it should really be called ‘Filters and Pipes’!)

Note that we can use nano (and the filename) to look at a file. This is good practise.

For the ‘Which Pipe’ exercise the solution is poorly written: option 1 will sort the animal file but will include the dates in the line’s it sorts and so `uniq` won’t work properly because the dates won’t allow the animals to line-up, Option 2: I’m not sure that’s code that would work (I had to look it up) the –t tells sort the columns are separated by spaces, -k is another flag that sorts based upon charaters in a line (ie sort using the two characters beginning at the second character). Option 3 misses out the sort (and sort needs come before `uniq`), option 4 is correct, option 5 will take the correct option and extract from it the number of lines (ie the number of different animals found, and not the number of the each unique animal found).

## Summary table/cheat sheet

| Commands|Action|
|-------|---------------|
|wc|Word count (gives lines, words and characters) |
|cat|Shows the text in a file onscreen|
|less|Same as cat but a screen at a time|
|sort|Sorts a file (or output)|
|head/tail |Top/bottom of a file|
|echo|Shows something on screen|
|cut| Cuts data out of a table/file (complex flags - see help!|
|uniq|Removes duplicate lines (after sorting)|
|>| Redirects the output to a file (overwrites existing files)|
|>>| redirects and output and adds the output to a file|
|\|| Pipe the output from one filter to another|

Bonus question: in the markdown code in the table above | is actually written as \| - why?

# Loops

I rememeber it as For, Do, Something, Dollar, Done'

In the first example try to pipe the head result to the tail code (it considers the whole head output as one!)

Use the space bar to indent your code, and **not the tab key**. 

The $ sign is also used to say ‘get the value of a variable’.

# Shell scripts
Using nano to set up scripts (*.sh files) But you don’t need the .sh extension (but it’s probably a useful convension). 

# Finding things
If you buy a book it has an index at the back. We now accept that the index of a book is a given, but it was a revolutionary innovation that helped in searching for information). I was an undergrad before google and even before journals started putting abstracts and keywords in electronic format. We had to search by a topic called ‘Chemical Abstracts’ they were huge books where all the keywords for papers were listed together with abstracts from papers…)

Grep – stands for global search (ie search somewhere you specify) for a regular expression (ie search for something you specify) and print.

When Little Women comes into the lesson we can use wc to get an idea of the filesize.

IF I HAVE GONE HERE FIRST THEN I NEED TO GO BACK TO CUT IN PIPES AND FILTERS or “The cut command is used to remove or ‘cut out’ certain sections of each line in the file, and cut expects the lines to be separated into columns by a Tab character. A character used in this way is a called a delimiter. In the example above we use the -d option to specify the comma as our delimiter character. We have also used the -f option to specify that we want to extract the second field (column). This gives the following output:”

For the ‘Tracking a species” exercise the thing to remember is that the grep is recursive and so the output of the grep contains the filepath (which has to be remove using the first cut statement).


