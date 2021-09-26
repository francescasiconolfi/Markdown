## Table of Contents

[File Editing](https://github.com/francescasiconolfi/Personal-Notes/blob/main/Linux-Commands-I-Actually-Use.md#file-editing)\
[File Movement](https://github.com/francescasiconolfi/Personal-Notes/blob/main/Linux-Commands-I-Actually-Use.md#file-movement)\
[Terminal Navigation](https://github.com/francescasiconolfi/Personal-Notes/blob/main/Linux-Commands-I-Actually-Use.md#terminal-navigation)


## File Editing

### cat
Reads file(s) and copies them to *stdout* (standard output).

**Formatting:**\
Can be used to append or overwrite *stdin* (standard input) or file(s) to another file using the append ('>>') or overwrite ('>') operators\
To use *stdin* directly from keyboard, do not specify files before the append/overwrite operators

### chmod
Changes mode (permissions) of a file/directory.

**Formatting:**\
*Octal Number Representation:* `chmod ugo file`\
where u is the permission specification for the user, g is the permission specification for the group, and o is the permission specification for others/world

##### Table 1. Permission specifications
| Permission | Symbol | Bits |
| --- | --- | --- |
| No access | - | 0 |
| Read | r | 4 |
| Write | w | 2 |
| Execute | x | 1 |

where u, g, and o will each be a sum of any of those bits (i.e. a mode set to 744 will allow read, write, and execute access to user, and only read access to group and world)

*Symbolic Representation:* `chmod sym file`\
where sym is formatted like so: owner operator permission

owner options:
- 'u' for "user" (owner)
- 'g' for "group"
- 'o' for "others" (world)
- 'a' fpr all (default if no owner specified)

operator options:
- '+' to add permission(s)
- '-' to remove permission(s)
- '=' to add permission(s) specified and remove those not

permission options:
- 'r' for "read"
- 'w' for "write"
- 'x' for "execute"

ex. chmod ug+x file wlll add execute permissions to user and group.

### grep
Finds text patterns in files and prints out lines containing the pattern.

**Formatting:**\
`grep pattern file` will filter through *file* for *pattern*.

*Important flags:*\
`-i` ignores case\
`-v` prints out lines that do NOT match the pattern

### tee
Reads *stdin* and copies it to both *stdout* and file(s) specified after (often used with the pipeline operator in a filter).

### uniq
Accepts a sorted list of data and removes any duplicates.

*Important flags:*\
`-d` lists duplicates found

Note: often used in conjunction with "sort".

---

## File Movement

---

## Terminal Navigation

### apropos
Searches list of man pages for command matches based on search term.

### cal
Displays the calender of the current month.

### cd
Changes the current directory to the specified one.

**Formatting:**\
`cd -` changes working directory to previous one\
`cd ~ username` changes working directory to working directory of *username*

### date
Displays the current date and time.

### df
Displays the current amount of free space on disk drives.

*Important flags:*\
`h` for human readability.\
`--total` to see the total usage/availability.

### du
Shows how much space each file takes up.

*Important flag:*\
`-h` for human readability.

### exit
Ends the terminal session.

Note: Can also use <kbd>Ctrl-D</kbd>.

### help
Displays information about shell builtins.

### id
Displays information about your identity.

### ls
Lists contents of current or specified directory or directories.

*Important flags:*\
`-a` (--all) shows hidden entries (starting with '.')\
`-A` (--almost-all) shows almost all entries (not those starting with '.' and '..')\
`-d` (--directory) shows directories\
`-h` (--human-readable) formats it for humans\
`-l` uses long listing format

### man
Enters manual page for specified executable program.

### passwd
Sets or changes your password.

Note: Superuser privileges are required if a user is specified.

### pwd
Displays the name of the current working directory.

### script
Records an entire shell session and stores it in the specified file (or in "typescript" if no file is specified).

### source
Forces bash to reread a specified file.

### su
Starts the shell as another user (superuser if no user is specified).

**Formatting:**\
`su - user`, where '-' starts a login shell, and *user* is any other user on the computer.
`su -c cmd` allows the execution of just *cmd* (command) as superuser.

### sudo
Executes a command as another user (superuser if no user is specified).

*Important flag:*\
`-i` starts a new shell.

### uptime
Shows how long the system has been in use.

*Important flags:*\
`-p` (--pretty) shows the uptime in a pretty format.\
`-s` (--since) shows since what time the system has been up.

### uname
Gives information about the system.

### whatis
Displays name and one line description of keyword.
