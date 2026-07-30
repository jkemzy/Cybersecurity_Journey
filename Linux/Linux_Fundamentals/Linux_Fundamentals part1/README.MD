# Linux Fundamentals Part 1

## Overview

This room introduced the Linux operating system, the command line, and basic file system navigation. The focus was on becoming comfortable using the terminal instead of a graphical interface.

---

## Linux File System

Linux stores everything under the root directory (`/`).

Common directories:

| Directory | Purpose |
|-----------|---------|
| / | Root directory |
| /home | User home folders |
| /etc | Configuration files |
| /var | Logs and variable data |
| /tmp | Temporary files |
| /bin | Essential commands |
| /usr | User applications |

---

## Navigation Commands

### pwd

Displays the current working directory.

```bash
pwd
```

### ls

Lists files and directories.

```bash
ls
ls -l
ls -la
```

### cd

Changes directories.

```bash
cd Documents
cd ..
cd ~
cd /
```

---

## File Management

Create a directory

```bash
mkdir notes
```

Create a file

```bash
touch notes.txt
```

Copy files

```bash
cp file.txt backup.txt
```

Move or rename files

```bash
mv old.txt new.txt
```

Delete files

```bash
rm file.txt
```

Delete folders

```bash
rm -r folder
```

---

## Reading Files

```bash
cat file.txt
```

Other useful commands:

```bash
less
head
tail
```

---

## Helpful Commands

```bash
clear
history
man
```

---

## Key Lessons

- Linux is case-sensitive.
- Everything begins at `/`.
- Hidden files begin with `.`.
- Terminal skills are essential for cybersecurity.

---

## Commands Practiced

- pwd
- ls
- cd
- mkdir
- touch
- cp
- mv
- rm
- cat
- clear
- man
