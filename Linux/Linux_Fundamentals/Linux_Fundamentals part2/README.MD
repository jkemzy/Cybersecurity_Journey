# Linux Fundamentals Part 2

## Overview

This room focused on Linux permissions, users, groups, searching for files, and managing running processes.

---

# Learning Objectives

- Understand users and groups
- Learn Linux permissions
- Search files efficiently
- Monitor and manage processes

---

# Users

Display the current user

```bash
whoami
```

Switch user

```bash
su username
```

Run commands as administrator

```bash
sudo command
```

---

# File Permissions

Display permissions

```bash
ls -l
```

Permission example

```
-rwxr-xr--
```

Meaning:

- r = Read
- w = Write
- x = Execute

Permission groups:

- Owner
- Group
- Others

---

# Changing Permissions

```bash
chmod 755 script.sh
chmod +x script.sh
```

---

# Changing Ownership

```bash
chown user file.txt
```

---

# Searching Files

```bash
find /home -name notes.txt
```

---

# Searching Text

```bash
grep "password" file.txt
```

Useful options

```bash
grep -r
grep -i
```

---

# Viewing Processes

```bash
ps
```

Real-time process monitoring

```bash
top
```

Terminate a process

```bash
kill PID
```

---

# Command History

```bash
history
```

---

# Locate Files

```bash
locate filename
```

---

# Wildcards

```
*
?
[]
```

Examples

```bash
ls *.txt
```

---

# Key Takeaways

- Linux permissions protect files.
- sudo provides administrative privileges.
- grep searches inside files.
- find searches the filesystem.
- Processes can be monitored and terminated.

---

# Commands Learned

- sudo
- whoami
- chmod
- chown
- grep
- find
- ps
- top
- kill
- locate
- history

---

# Skills Gained

- Permission management
- Process management
- Searching files
- User administration
