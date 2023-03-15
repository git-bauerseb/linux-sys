## Commands

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

## Paths/Files

/usr/share/doc -> Documentation for some programs

## Environment variable

PATH: list of system directories shell searches when trying to locate command

## Shell Navigation

Ctrl-B - Cursor left
Ctrl-F - cursor right
Ctrl-P - previous command
Ctrl-N - next command

Ctrl-U - erase cursor <-> beginning

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
  - 
