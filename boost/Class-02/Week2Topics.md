Week 2 focuses on UNIX/Linux origins and the terminal, command-line
interface and basic file system navigation. You should be comfortable
installing and removing and reinstalling Linux Ubuntu Server VMs and any
apt packages before next week.

- Primary responsibilities of any mentor

  1. Help you know what to learn
  1. Help you know where to learn it (curate resources)
  1. Help you when you get stuck

1. What is a "shell" and why do I care?

- Shell - Interactive program (not always command line) to a deeper system. (anything that provides an interface for humans to talk to system)

2. What is the difference between "terminal", "CLI", and "shell"?

- The terminal - terminal emulator based these days on stanard VT100 terminal that was invented to use a digital method of inputting data to replace teletype machine that was used before.
- Command line interface - can be used without a terminal. CLI also known as a REPL. Read, evaluate, print, loop. Anything that takes input on a singel line and prints it back to you. - Basically I type a command and computer prints back something
- Shell - Interactive program (not always command line) to a deeper system (anything that provides an interface for humans to talk to system)

3. What is a REPL? (Read, Evaluate, Print, Loop)

- Read evaluate print loop.

4. Install and configure terminal software (MS Terminal, iTerm2)

5. What is UNIX and Linux? Difference between Unix and Linux.
   Linux was a IN You Face to Linux to Linux Torvald's HS professor. Minux was a free version of Linux. C language was created to make UNIX. Mac OS biggest unix distributor in the world. Unix was invented at AT&T Bell Labs

- What is GNU? Who invented Linux?

- Basic system update and package management and installation

  - Use apt-get anytime you are writing a script.
  - Find out more with man apt
  - NEVER USE `apt` IN A SCRIPT. Use apt-get and apt cache instead.
  - Everytime you are writing code you execute a command

- When to use apt vs apt-get?

  - APT is baseline package for debian packages. Basis for all desktop linux systems that matter (advanced packaging tool)
  - Use apt-get anytime you are writing a script.
  - Find out more with man apt
  - NEVER USE `apt` IN A SCRIPT. Use apt-get and apt cache instead.
  - Everytime you are writing code you execute a command
  - learn more with `man apt-get` and learn more about apt-get

- What is a "package"?
- How do I install software?
- Really simple and essential shell commands
- What do the character's in the prompt mean?
- What is an "inode"? Why everything is "just a file"?
  - An inode is a entry in a table. A table is like a big file with key name and a "value pair" that it points to. A directory is a table of inodes. Those inodes have name. One of those is a file and another is a directory.
- What are UNIX/Linux permissions?
- What does `.` and `..` mean?
- How do I know that `apt` packages are safe?
  - Packages used in apt are very well vetted
  - Packages take a long time to get vetted and this makes them safer
  - Some people don't like that
  - Never just glaze over and hit yes
- What is a shell "history"?

## Other good informaiton

- Most Imporant people in Unix - Ken Thompson, Dennis Richie, Brian Kernighan
- A backdoor is breakin in a computer and provide way to connect over network to that computer so you can enter commands on remote computer.
- Most Imporant people in Unix - Ken Thompson, Dennis Richie, Ryan Cardigan
- Three main distro needed to get a job
  - Ubuntu Server
  - Red Hat
  - SUSE Linux
- First thing you want to do when logging into a linux system is
  - `sudo apt update` and then do a `sudo apt upgrade`
  - this will make sure your system is up to date
  - `sudo apt update` update all the soruces for packages - gets the latest in the list
  - `sudo apt upgrade` upgrade **all** packages to latest

note that `sudo` is do it as root/superuser

## Stuff to learn and look into

- GREP and What it is
- Learn about TTY
- Minux

## Commands Used

- `man` - show manual information about a command
- `sudo` - do it as root (superuser)
- `apt` - use interactively only (use `apt-get` in scripts)
- `sudo apt update` - update all the sources for packages
- `sudo apt upgrade` - upgrade _all_ packages to latest version
- `apt search ^neo` - search for all package starting with `neo`
- `sudo apt install neofetch` - install `neofetch` and dependencies
- `sudo apt remove neofetch` - remove `neofetch`
- `sudo apt autoremove` - automatically remove unused packages
- `ls` - list the files in the (current) directory
- `ls -al` - list all the files including hidden (begin with `.`)
- `hostname` - display name of host computer
- `pwd` - print working directory
- `cd foo` - change into the `foo` directory
- `cd`, `cd ~` - change back to the home directory
- `cd ..` - change into the relative parent directory
- `cd ../..` - change into the relative parent of the parent directory
- `cd -` - change to previous directory
- `cd /` change to the root directory

Related:

- https://github.com/microsoft/terminal/releases (no app store needed)
- https://youtu.be/crtZHNclndQ (cool retro terminal)
- https://www.linuxcommand.org
- https://replit.org
- https://medium.com/@rwxrob/problem-with-repl-it-415f885164f
- "AT&T Archives: The UNIX Operating System" https://youtu.be/tc4ROCJYbm0
- "It's a UNIX system" https://youtu.be/dxIPcbmo1_U
- "Is it time to rewrite the OS in Rust" https://youtu.be/HgtRAbE1nBM
- https://youtu.be/ctGpRWCi8QU
- https://git-scm.org
