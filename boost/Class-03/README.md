Help with timestamps
Boost sessions moved to Sunday
How to connect to our VM (secure shell)

- where are all my files and why are they there?
- How do I remove add and rename file and directories?
- How do I edit files?
- What is NAT and Bridged? - Learn more about NAT
  - NAT is network address translation - Host is like a house with WIFI, every vm that runs on host computer is protected and has it's own IP. Thing that connects to internet from house is the Router (like mail and it goes to router and gets routed to internet and comes back. Basically mail sorts it)
  - Bridged - We will pretend that this vm is not inside but next to it. As far as networking is concernted, it is sitting next to your computer.
  - 10. IP addresses are reserved IP addresses
    - All an IP address is is an address to your house (a way to get to your computer)
    - It's an address to your computer (IP is the thing that give us our connection)
    - If it's bridged, it gets a brand new IP address
      - a bridged interface will use the same physical inteface with a different IP and MAC address
    - `ip a` gives you the ip address
- Why can't I use the 127. address?
  - "There's no place like home"
  - If you try to connect to anything with 127 then it would try to connect to your current computer
- How can you test ssh connection to localhost? 01:27:50
- What is TTY1 - (there are 7 consoles) note that tty are not encrypted
- What is pts/0 is the ssh connection

  - Reason we have two connections becasue of the different consoles we have connected to it
  - Note the "-" means as if we plugged a serial connection directly to the computer

- How can I see stuff scrolling off screen? -`| less` or `| more1` - see scrolled output in terminal
- What packages need to be installed to connect with SSH? 01:57:40

- hacking, debugging is largely about eliminating variables so we can get to problem
- ## PUTTY for ssh access?

## Commands

- `ip a` show all ip addresses or `ipconfig /all` on windows
- `clear` clears the screen
- `which ssh` display full path to ssh program
- `type ssh` display what type of thing it is - type will tell you if it is a command
- `who` - display who is logged in and how
- `w` - display longer of who is logged in
- `whoami` - print effective user name/ID
- `users` - short name of all logged in users
- `last` - summary of last logged in users
- `id` - display user and group names and ids for self
- `exit` - exit the cutteny program or login or shell
<!-- - try less or more tipics more -->
- | less or | more - see scrolled output in terminal (q to quite)
- <CTRL>c to interrupt whatever (exit)
- <CTRL>d send "end of data/file"

## Related

## NOTES

00:36:46 Talk about how SSHD is better backdoor to install because it is harder to find

## Recap

- Difference between console and Terminal
  - console is actual console or a physical one or one that is digital
    - Literally the thing you would see
