Week 2 focuses on UNIX/Linux origins and the terminal, command-line
interface and basic file system navigation. You should be comfortable
installing and removing and reinstalling Linux Ubuntu Server VMs and any
apt packages before next week.

1. Primary responsibilities of any mentor

   1. Help you know what to learn
   2. Help you know where to learn it (curate resources)
   3. Help you when you get stuck
   4. Go into each lesson knowing what the lesson is and what you want to learn
      1. Learn to run the session and ask questions
   5. This is the way Rob does mentoring

2. What is a "shell" and why do I care?

   1. **Shell** - Interactive program (not always command line) to a deeper system. (anything that provides an interface for humans to talk to system). Shell is not the same as a CLI. Interactive proactive that provides access to a deeper system. Anything that provides interface to a human that talkes to inner part of system. You can have a shell in any other system. A layer that is there to talk to a human.

3. What is the difference between "terminal", "CLI", and "shell"?

   1. **The terminal** - Gives you cell based text screen. Terminal emulator based these days on stanard VT100 terminal that was invented to use a digital method of inputting data to replace teletype machine that was used before.
   2. **Command line interface** - can be used without a terminal. CLI also known as a REPL. Read, evaluate, print, loop. Anything that takes input on a singel line and prints it back to you. - Basically I type a command and computer prints back something. And it will prompt you again.
   3. **Shell** - Interactive program (not always command line) to a deeper system (anything that provides an interface for humans to talk to system)

4. What is a REPL? (Read, Evaluate, Print, Loop)

   1. Read evaluate print loop.

5. Install and configure terminal software (MS Terminal, iTerm2)

6. What is UNIX and Linux? Difference between Unix and Linux.
   Linux was a IN You Face to Linux to Linux Torvald's HS professor. Minux was a free version of Linux. C language was created to make UNIX. Mac OS biggest unix distributor in the world. Unix was invented at AT&T Bell Labs

7. What is GNU? Who invented Linux?

8. Basic system update and package management and installation

   1. Use apt-get anytime you are writing a script.
   2. Find out more with `man apt`
      1. `man` is command for manual
   3. NEVER USE `apt` IN A SCRIPT. Use apt-get and apt cache instead.
   4. Everytime you are writing code you execute a command

9. When to use apt vs apt-get?

10. APT is baseline package for debian packages. Basis for all desktop linux systems that matter (advanced packaging tool)
11. Use apt-get anytime you are writing a script.
12. Find out more with man apt
13. NEVER USE `apt` IN A SCRIPT. Use apt-get and apt cache instead.
14. Everytime you are writing code you execute a command
15. learn more with `man apt-get` and learn more about apt-get

16. What is a "package"? (3:15:40)

17. Package is a amount of software that has been packaged up for install.

    1. Like a .msi on windows
       1. It runs an interactive GUI thing
       2. Or chocolately - command line package manager
    2. On mac it makes a disk drive on the system
       1. Or BREW - command line package manager
    3. When you use APT a DPKG is installed.
    4. A DPKG is a dameon file (dameon package)
    5. The files are snap files
    6. Note that like a true software package manager has a few things in common
    7. you can DL, install, and remove stuff

18. How do I install software?

    1. Command line package manager - a way to install, remove, update a software from the command line. It is way more powerful because it can be scripted.
    2. Crash Course in Regular Expression
       1. `^` in regex lockdown this expression to beginning of the string
       2. Use `apt search ^neo` to search everything with Neo inthe name
       3. Use `sudo apt earch neofetch` to install neofetch
       4. use `sudo atp remove neofetch` to remove things named neofetch
       5. use `sudo apt remove neofetch` to remove things names neofetch
       6. `sudo apt autoremove` will remove anything that is taking up disk space that is not being used by what you just installed

19. [Really simple and essential shell commands](#shell-commands-used)
20. What do the character's in the prompt mean?
21. What is an **inode**? Why everything is "just a file"?

    1. Everything is a file because
    2. inode is an entry in a table. Like a key value pair.
    3. A directory is a table of inodes
       1. Different types of inode are plain text files

22. An inode is a entry in a table. A table is like a big file with key name and a "value pair" that it points to. A directory is a table of inodes. Those inodes have name. One of those is a file and another is a directory.

23. What are UNIX/Linux permissions?
24. What does `.` and `..` mean?
    1. In filesystems, we use the double dot (..) to access the parent directory, whereas the single dot (.) represents the current directory.
25. How do I know that `apt` packages are safe?

    1. Packages used in apt are very well vetted
    2. Packages take a long time to get vetted and this makes them safer
    3. Some people don't like that
    4. Never just glaze over and hit yes

26. What is a shell "history"?
    1. Just push the up arrow key.

## Other good informaiton

1. Most Imporant people in Unix - Ken Thompson, Dennis Richie, Brian Kernighan
2. A backdoor is breakin in a computer and provide way to connect over network to that computer so you can enter commands on remote computer.
3. Most Imporant people in Unix - Ken Thompson, Dennis Richie, Ryan Cardigan
4. Three main distro needed to get a job

   1. Ubuntu Server
   2. Red Hat
   3. SUSE Linux

5. First thing you want to do when logging into a linux system is

   1. Note that `sudo` is do it as root/superuser
   2. `sudo apt update` and then do a `sudo apt upgrade`
   3. this will make sure your system is up to date
   4. learn difference between sudo apt update and sudo apt upgrade
   5. `sudo apt update` update all the soruces for packages - gets the latest in the list
   6. `sudo apt upgrade` upgrade **all** packages to latest

6. Keep system updated so it is likely to get hacked
   1. Hard wire is the best method

## Stuff to learn and look into

- GREP and What it is
- Learn about TTY
- Minux

### Shell Commands Used

11. Really simple and essential shell commands

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
