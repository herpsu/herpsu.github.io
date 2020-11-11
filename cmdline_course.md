---
layout: default
---

## The course: Command line tools for linguists

During the course the students get comfortable with both basic and advanced unix commands and programs used in NLP, and the unix environment in general.

## Week 1: Introduction to Command Line Environments

> All of you will have problems.  
> -Hande Celikkanat

The first week was when we were taught about the computer, its physical parts and the unix operating system. we had a lecture about it in zoom. each student installed and/or configured their own unix system, learned to move around in the file system and some basic file manipulation.

I already knew some of the commands since I had taken a similar course earlier. I still had to read the manpages a lot though! I had completely forgotten the flags associated with each program.

### Commands learned this week:

Command | What it does
--- | ---
ls | y
pwd | x
whoami | x
cd | x
wget | x
less | x
mkdir | x
cat | x
touch | x
cp | x
rm | x
mv | x
Esc | x
Ctrl-c | x
Ctrl-d | x
Ctrl-x | x
Ctrl-c | x
nano | x
emacs | x

## Week 2: Navigating a UNIX System

the UNIX system
copy, move and remove directories
standard system directories and what they contain
how the UNIX system protects the privacy of the users
permissions which determine the files and directories each user can access
processes
process management
control processes from the command line
working on a remote server using
programs ssh and scp
CSC taito or puhti server

Most of the commands were again familiar. The biggest problem this week was to get the permissions to use CSC servers to work... I also had to switch from the Windows Linux subsystem to Virtualbox because of some compatibility issues.

### Commands learned this week:

Command | What it does
--- | ---
cp -jotain | x
mv -jotain | x
rm -r | x
cd / | x
gzip | y
tar | x
ls -jotain | x
chmod | x
ps | x
kill | x
& | starts process in bg
fg | x
ctrl+z | x
ssh | x
scp | x


## Week 3: Basic Corpus Processing

> Regular expressions are like black magick  
> -Hande Celikkanat

text processing tools in UNIX
character encodings
convert between different character encodings
UNIX commands which are meant for processing text files and searching in text files
structured text files
example: tables

On the last course, encoding was one of the biggest hurdles. The Windows and terminal program on my home PC and the university Linux server all had to be configured properly. Luckily this time there were no problems since I did everything on my home PC. Writing regular expressions was actually quite a fun excersize!

### Commands learned this week:

Command | What it does
--- | ---
file | y
iconv | x
dos2unix | x
tr | x
sort | x
uniq | x
egrep | x
cut | x

## Week 4: Advanced Corpus Processing

text processing using UNIX commands
command pipelines
the sed command
more about regular expressions

I was already comfortable with writing pipelines, but sed was completely new to me. Sometimes I would get frustrated and just use egrep instead. I have a lot to learn...

### Commands learned this week:

Command | What it does
--- | ---
sed | y

## Week 5: Scripting and Configuration Files

scripts
environment variables
useful variables,
setting up a configuration file

I had trouble making some of the scripts work the way I wanted. I had also misplaced my old configuration file and had to start from scratch.

### Commands learned this week:

Command | What it does
--- | ---
printenv | x
echo | x
export | x

## Week 6: Installing and Running Programs

installing programs
package managing programs
make

I couldn't make bllip work. The makefile syntax was way beyond my capabilities as well... I hadn't heard of meld before and it seemed very useful! I'll be using it a lot in the future.

### Commands learned this week:

Command | What it does
--- | ---
sudo | x
su | y
apt-get | x
brew | x
locate | x
python | x
pip | x
virtualenv | x
source | x
deactivate | x
make | x

## Week 7: Version Control

version control
jekyll
Git
Github

Virtualbox decided to destroy my Linux installation so I had to reinstall and configure everything before getting to the actual 

### Commands learned this week:

Command | What it does
--- | ---
git | y
