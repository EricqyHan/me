# What we are doing today

- Where are all my files and why are they there?
- What is a home directory? - 00:21:44
  - It is where all your user files go. Where your files live.
  - You need it because it contains your files and your configuration
    - You have a place with permissions for your users and not touch system files
    - Primary reason is to make the system more safe these days and separate user from everything else
- How to list current directory permissions?
  - ``
- What are permisions and why do I care? - 00:30:00
- How do I remove, add , and rename files and directories
- How do I edit files?
- Everything is an inode ("file")
- change ther permissions on a file - 01:08:13

- Dangers of 'setuid'

What is difference between console and terminal.

- IP address is like numbers on a house
  - DHCP - dynamic host control protocol
- Console is hardware or simulated connection to hardware. How you call a keyboard and display attached to your server
- Terminal is running on a console, can also have a remote terminal using ssh
  - terminal is the software interface with the user

## Organization of the files

- Home directory is where all the files for the user lives

Even if it is one user on the system, we need the premissions

## commands

`ls` - list files
`cd` changes directory
`ls -la` list all premissions of current directory
`ls -ld .` look directory permissions on current directory
`stat foo` see all details about the `foo` inode
`sudo adduser 'gilfoyle'` add user gilfoyle
`sudo passwd foo` - change password for foo
`sudo passwd` - change own password
`stat -c '%a` to see octal permissions
`chmod +x foo` - make foo file executable by user, group, other
`chmod o-r foo` - make foo unreadable by other
`echo foo` - write foo to standard output
`cat foo` - write foo file to standard output 
`whoch foo` - print full file path to executable foo

## Relate4d

https://www.picoctf.org/
