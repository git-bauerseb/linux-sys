## Commands

gzip
 gunzip file.gt
 gzip file

tar xvf
  x: extract
  
	
umask

chmod
  - change permission
  g+r file - add read to group
  644 file - add 110 (read/write) to user, 100 (read) to group, 100 (read) to other

  711/700/755 - directories

fg
bg

cat
  - concatenate files

cd
  - change directory
mkdir
  - create directory
rmdir
  - remove directory

diff

file filename
  - trying to interpret file

find dir -name file -print

locate
  - searches index; much faster

head/tail
  - portin of file or stream

sort
  - sort text file

passwd
  - change password

cp
  - copy file
ls
  - list directory
mv
  - move file
touch
  - change access/modification time of file
rm
  - remove file
echo
  - output to standard output

grep
  - prints lines from file that match expression

less
  - scrolling file

tr pattern1 pattern2
  - replace pattern1 by pattern2

ps
  - list of running processes
  PID TTY STAT TIME COMMAND

udevadm

chvt NUMBER
  - switch to /dev/tty<NUMBER>

dd
 if=/dev/zero of=new_file bs=1024 count=1

 - e.g. dd if=/dev/urandom bs=1k count=1 2>/dev/null | base64

lsscsi
 - list SCSI devices

## Devices

/dev/null -> kernel ignores input

sysfs interface
 - /sys/devices

/dev/sd* -> hard disks

Alt-F1 -> /dev/tty1
Alt-F2 -> /dev/tty2

## Paths/Files

/usr/share/doc -> Documentation for some programs
/etc/sudoers -> let user run sudo commands

## Environment variable

PATH: list of system directories shell searches when trying to locate command

## Shell Navigation

Ctrl-B - Cursor left
Ctrl-F - cursor right
Ctrl-P - previous command
Ctrl-N - next command

Ctrl-U - erase cursor <-> beginning
Ctrl-L - redraw terminal

## Shell

fork() -> create identical copy
exec(progr) -> start progr, replacing current process

Pseudodevice: look like devices to user process
  - e.g. /dev/random

.  -> current dir
.. -> parent dir
/.... -> absolute path
./... -> relative path


Shell Globbing (*/?)
  - use '*' to disallow globbing

Shell variable
Use VAR=VALUE to set variable VAR with value VALUE
  - access: $VAR

Environment variable: Set and passed to programs
  - VAR=VALUE
  - export VAR

command > file -> send output to file
command >> file -> append output to file
com1 | com2 -> send output of com1 to input of com2

com1 2> file -> send stderr to file
2>&1 -> send stderr/stdout to same file

Ctrl-Z - Stop process


Symbolic link: File pointing to another file
 ln -s target linkname
