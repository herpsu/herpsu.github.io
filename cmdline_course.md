---
layout: default
---

## Report: Command line tools for linguists

<img src="assets/images/code.jpg" alt="Photo" hspace="20" width="30%" align="right"/> During 
the course the students get comfortable with both basic and advanced unix commands 
and programs used in NLP, and the unix environment in general.

### Week 1: Introduction

> All of you will have problems.  
> -Hande Celikkanat

The course started with a Zoom-meeting (2020...). 
People introduced themselves and the course instructor gave a lecture about computer hardware 
and the UNIX operating system. 
Each student installed and/or configured their own UNIX system and learned some 
basic commands to move around in the file system and manipulate files. 
Starting programs and stopping them in different ways were also explored.

**I** already knew some of the commands since I had taken a similar course earlier. 
I still had to read the manpages a lot though! 
I had completely forgotten the flags associated with each program.

#### Commands learned this week:

Command | Description
--- | ---
`ls` | lists directory contents
`pwd` | prints name of current directory
`whoami` | prints current user name
`cd` | changes directory
`wget` | downloads from a url
`mkdir` | creates a folder
`cat` | prints input
`less` | prints input, scrollable
`touch` | creates file
`cp` | copies file
`rm` | deletes file
`mv` | moves or renames file
`nano` | a simple text editor
`emacs` | a text editor with more features

### Week 2: Navigating a UNIX System

The second week was a deeper dive into some of the programs introduced in the beginning. Students learned to
* manipulate entire folders with the `-r` flag,
* find and change file and folder permissions with `ls -l` and `chmod` and
* run and shut down processes in the background using `&`, `ps` and `kill`.

[CSC](https://www.csc.fi/) servers were also used to test connecting to a remote host using `ssh` and `scp`.

**M**ost of the commands were again familiar. 
The biggest problem this week was to get the permissions to use CSC servers to work... 
I also had to switch from the Windows Linux subsystem to Virtualbox because of 
some compatibility issues.

#### Commands learned this week:

Command | Description
--- | ---
`cp -r` | copies directory and its contents
`rm -r` | deletes directory and its contents
`cd /` | changes directory to root
`gzip` | compresses or expands files
`tar` | archives multiple files into a single file
`ls -l` | lists directory contents and their permissions
`chmod` | modifies file permissions
`ps` | lists running processes and their PIDs
`kill` | closes a process
`&` | starts given process in the background
`fg` | brings process into foreground
`ssh` | connects to a remote host
`scp` | copies a file from a remote host


### Week 3: Basic Corpus Processing

> Regular expressions are like black magic.  
> -Hande Celikkanat

This week contained most of the important programs for processing text files. 
Basic regular expressions and other methods of formatting text for qualitative analysis 
were introduced. 
Students learned to convert files from DOS to UNIX format and between different 
character encodings.

**D**uring the last course, encoding was one of my biggest hurdles. 
Windows and the terminal program on my home PC as well as the university Linux server all 
had to be configured properly. 
Luckily this time there were no problems since I did everything on my home PC. 
Writing regular expressions was actually quite a fun exersise in comparison!

#### Commands learned this week:

Command | Description
--- | ---
`file` | determines file type of given file
`iconv` | converts text from one character encoding to another
`dos2unix` | converts text file from dos to unix format
`tr` | translates given characters from input to something else
`sort` | sorts lines in given text files
`uniq` | removes repeating lines from input
`egrep` | prints lines that match regexp pattern
`cut` | removes sections from lines of input

### Week 4: Advanced Corpus Processing

This week, piping commands in `bash` was introduced alongside more complicated 
regular expressions and `sed`, a program using these to modify text.

**I** was already comfortable with writing pipelines, but sed was completely new to me. 
Sometimes I would get frustrated and just use egrep instead. I have a lot to learn...

#### Commands learned this week:

Command | Description
--- | ---
`sed` | transforms input according to given instructions

### Week 5: Scripting and Configuration Files

All the commands taught earlier in the course were used this week as well, 
this time written into convenient script files. 
Students also learned how to manipulate environment variables and set up their own 
bash configurations.

**I** had trouble making some of the scripts work the way I wanted. 
I had also misplaced my old configuration file and had to start from scratch.

#### Commands learned this week:

Command | Description
--- | ---
`printenv` | prints values of given environment variables
`echo` | prints input
`export` | changes value of given environment variable(s)

### Week 6: Installing and Running Programs

This week, students learned all about different package managers and how to use them 
to install, uninstall and update software as well as basic Python commands and 
makefile syntax. 
Inputting commands as root was also introduced.

**I** couldn't get bllip to work. The makefile syntax was way beyond my capabilities as well... 
I'll be reviewing this in the future and updating what I learn here, hopefully.  
I hadn't heard of meld before and it seemed very useful! 
I'll definitely be using it in the future.

#### Commands learned this week:

Command | Description
--- | ---
`sudo` | executes given command as root
`su` | same as above; without arguments starts shell as root
`apt-get` | the default unix package manager
`brew` | alternate package manager
`locate` | search for file with given name
`python` | python language interpreter
`pip` | python package manager
`virtualenv` | creates virtual python environment
`source` | executes commands from given file
`make` | compiles source code according to makefile instructions

### Week 7: Version Control

Week 7 was all about the distributed version control system `git` and one of its most 
popular hosting services, [GitHub](https://github.com/). Students made their own 
repositories and published them on GitHub using the `git` command line.

**G**it proved to be fairly easy to use after a bit of time especially with 
[this video](https://www.youtube.com/watch?v=HVsySz-h9r4). I've already got a few ideas 
that I'd like to try implementing with it. I tried to enable 2-factor authentication on 
Github, but using it with the command line proved to be a bit of a headache, so I decided 
to try it again at a later time.

#### Commands learned this week:

Command | Description
--- | ---
`git` | distributed version control system

### Week 8: Final assignment

The final assignment had the students make their own github.io page with a course report. 
Local testing was done using `jekyll` and page formatting was implemented with Markdown 
syntax in order to make writing the course report simple.

**V**irtualbox decided to destroy my Linux installation so I had to reinstall and configure 
everything before starting the actual assignment. Learning Markdown was the easiest part, 
since the syntax is is minimal and I had already learned LaTeX.  
I spent almost two hours trying to make `jekyll` work, just to find out that the instructions 
clearly said what I did wrong: I had installed `jekyll` with `apt-get` instead of `bundle`. 
I also had to add `gem: "kramdown-parser-gfm"` to the gemfile, 
since it was missing and `bundle exec jekyll serve` refused to work without it.  

#### Commands learned this week:

Command | Description
--- | ---
`jekyll` | generates local website from source
`bundle` | manages dependencies for Ruby
