- What are we doing today?
  - Go into each lesson knowing what the lesson is and what you want to learn
  - Learn to run the session and ask the questions
- Way Rob does Mentoring is

What is difference between terminal, cli, shell
Terminal - thing gives you cell based text screen. Terminal emulator
CLI - Command Line Interface - AKA a REPL, a read evaluate, print, loop. Anything that takes in an input on a single line and does something and prints back to you. And prompts you again.

Shell - shell is not the same as CLI. Interactive proactive that provides access to a deeper system. Anything that provides interface to a human that talkes to inner part of system. You can have a shell in any other system. A layer that is there to talk to a human.

What is GNU - replaced all told that were invented to go with linux

Keep system updated so it is likely to get hacked
Hard wire is the best method

- `ls -al` - will whow all files including hidden(beginning with .)

- back in the OG day, everything had to be 8 characters or less

What is an inode? Why everything is just a file?

- Everything is a file because
- inode is an entry in a table. Like a key value pair.
- A directory is a table of inodes
  - Different types of inode are plain text files

Directory structure - textual representation of a file path

How to install softare (03:15:40)
What is a package - a package is a amount of software that has been packaged up for install.

- like a .msi
- it runs an interactive GUI thing
- on mac it makes a disk drive on the system
  - or BREW - command line package manager
  - or chocolately - command line package manager

What is a DPKG - dameon package is the actual name

`sudo apt search neo` will find anything with the word "neo" in name

learn difference between sudo apt update and sudo apt upgrade

Crash Course in Regular Expression
`^` in regex lockdown this expression to beginning of the string

Use `apt search ^neo`

`sudo apt remove neofetch` - to remove neofetch
`sudo apt autoremove` - will remove anything that is taking up disk space that is not being used by what you just installed
