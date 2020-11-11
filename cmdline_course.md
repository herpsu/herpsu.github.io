---
layout: default
---

## The course: Command line tools for linguists

During the course the students get comfortable with both basic and advanced unix commands and programs used in NLP, and the unix environment in general.

### Week 1: Introduction to Command Line Environments

> All of you will have problems.  
> -Hande Celikkanat

The first week was when we were taught about the computer, its physical parts and the unix operating system. we had a lecture about it in zoom. each student installed and/or configured their own unix system, learned to move around in the file system and some basic file manipulation. We also learned to start programs and stop them in different ways.

I already knew some of the commands since I had taken a similar course earlier. I still had to read the manpages a lot though! I had completely forgotten the flags associated with each program.

#### Commands learned this week:

Command | What it does
--- | ---
ls | lists directory contents
pwd | prints name of current directory
whoami | prints current user name
cd | changes directory
wget | downloads from a url
mkdir | creates a folder
cat | prints input
less | prints input, scrollable
touch | creates file
cp | copies file
rm | deletes file
mv | moves or renames file
nano | a simple text editor
emacs | a text editor with more features

### Week 2: Navigating a UNIX System

the UNIX system, copy, move and remove directories, standard system directories and what they contain, how the UNIX system protects the privacy of the users, permissions which determine the files and directories each user can access, processes, process management, control processes from the command line, working on a remote server using, programs ssh and scp, CSC taito or puhti server

Most of the commands were again familiar. The biggest problem this week was to get the permissions to use CSC servers to work... I also had to switch from the Windows Linux subsystem to Virtualbox because of some compatibility issues.

#### Commands learned this week:

Command | What it does
--- | ---
cp -r | copies directory and its contents
rm -r | deletes directory and its contents
cd / | changes directory to root
gzip | compresses or expands files
tar | archives multiple files into a single file
ls -l | lists directory contents and their permissions
chmod | modifies file permissions
ps | lists running processes and their PIDs
kill | closes a process
& | starts given process in the background
fg | brings process into foreground
ssh | connects to a remote host
scp | copies a file from a remote host


### Week 3: Basic Corpus Processing

> Regular expressions are like black magic.  
> -Hande Celikkanat

text processing tools in UNIX, character encodings, convert between different character encodings, UNIX commands which are meant for processing text files and searching in text files, structured text files (example: tables)

On the last course, encoding was one of the biggest hurdles. The Windows and terminal program on my home PC and the university Linux server all had to be configured properly. Luckily this time there were no problems since I did everything on my home PC. Writing regular expressions was actually quite a fun excersize!

#### Commands learned this week:

Command | What it does
--- | ---
file | determines file type of given file
iconv | converts text from one character encoding to another
dos2unix | converts text file from dos to unix format
tr | translates given characters from input to something else
sort | sorts lines in given text files
uniq | removes repeating lines from input
egrep | prints lines that match regexp pattern
cut | removes sections from lines of input

### Week 4: Advanced Corpus Processing

text processing using UNIX commands, command pipelines, sed, more about regular expressions

I was already comfortable with writing pipelines, but sed was completely new to me. Sometimes I would get frustrated and just use egrep instead. I have a lot to learn...

#### Commands learned this week:

Command | What it does
--- | ---
sed | transforms input according to given instructions

### Week 5: Scripting and Configuration Files

scripts, environment variables, setting up a configuration file

I had trouble making some of the scripts work the way I wanted. I had also misplaced my old configuration file and had to start from scratch.

#### Commands learned this week:

Command | What it does
--- | ---
printenv | prints values of given environment variables
echo | prints input
export | changes value of given environment variable(s)

### Week 6: Installing and Running Programs

installing programs, package managers, make

I couldn't make bllip work. The makefile syntax was way beyond my capabilities as well... I hadn't heard of meld before and it seemed very useful! I'll be using it a lot in the future.

#### Commands learned this week:

Command | What it does
--- | ---
sudo | executes given command as root
su | same as above; without arguments starts shell as root
apt-get | the default unix package manager
brew | alternate package manager
locate | search for file with given name
python | python language interpreter
pip | python package manager
virtualenv | creates virtual python environment
source | executes commands from given file
make | compiles source code according to makefile instructions

### Week 7: Version Control

version control, Git, Github

Git proved to be fairly easy to use after a bit of time especially with [this video](https://www.youtube.com/watch?v=HVsySz-h9r4). I've already got a few ideas that I could probably implement with it.  
I tried to enable 2-factor authentication on Github, but using it with the command line proved to be a bit of a headache, so I decided to try it again at a later time.

#### Commands learned this week:

Command | What it does
--- | ---
git | distributed version control system

### Week 8: Final assignment

jekyll, github, etc

Virtualbox decided to destroy my Linux installation so I had to reinstall and configure everything before getting to the actual assignment.  
I also spent almost two hours trying to make jekyll work, just to find out that the instructions clearly say what I did wrong: I had installed jekyll with apt-get instead of bundle.  
I had to add `gem: "kramdown-parser-gfm"` to the gemfile as well, since it was missing and `bundle exec jekyll serve` refused to work without it.  
Learning Markdown was the easiest part, since the syntax is is minimal and I had already learned LaTeX.

#### Commands learned this week:

Command | What it does
--- | ---
jekyll | generates local website from source
bundle | manages dependencies for Ruby
