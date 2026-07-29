# Web Directory Enumeration (TryHackMe - Room 404)

## Objective
Discover hidden directories and files on a web server.

## Tools
- Gobuster
- curl
- Firefox
- Nmap

## Basic Enumeration

Check the website:

```bash
curl http://TARGET:PORT
```

View headers:

```bash
curl -I http://TARGET:PORT
```

## Gobuster

Basic usage:

```bash
gobuster dir -u http://TARGET:PORT -w WORDLIST
```

Example:

```bash
gobuster dir \
-u http://TARGET:PORT \
-w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt
```

Extensions:

```bash
-x php,html,txt,bak
```

Exclude custom 404 pages:

```bash
--exclude-length SIZE
```

## Useful Wordlists

DirBuster:
- directory-list-2.3-small.txt
- directory-list-2.3-medium.txt
- directory-list-2.3-big.txt

SecLists:
- Discovery/Web-Content/common.txt
- Discovery/Web-Content/raft-medium-directories.txt

## Useful Files

- /robots.txt
- /sitemap.xml

## HTTP Status Codes

- 200 OK
- 301 Redirect
- 302 Redirect
- 403 Forbidden
- 404 Not Found

## Lessons Learned

- Enumeration starts with identifying the correct target and port.
- Choosing the correct wordlist is critical.
- Using an unrelated wordlist (e.g. apache-user-enum) can produce no results.
- Inspect page source, robots.txt, and sitemap.xml for additional clues.
