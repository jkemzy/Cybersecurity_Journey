# Linux Fundamentals Part 3

## Overview

This room introduced package management, services, networking basics, SSH, and task automation.

---

# Package Management

Update repositories

```bash
sudo apt update
```

Upgrade installed software

```bash
sudo apt upgrade
```

Install software

```bash
sudo apt install package
```

Remove software

```bash
sudo apt remove package
```

---

# Services

View service status

```bash
systemctl status ssh
```

Start a service

```bash
sudo systemctl start ssh
```

Enable a service

```bash
sudo systemctl enable ssh
```

---

# SSH

Connect remotely

```bash
ssh user@ip
```

---

# SCP

Copy files securely

```bash
scp file.txt user@ip:/home/user/
```

---

# Download Files

Using wget

```bash
wget URL
```

Using curl

```bash
curl URL
```

---

# Cron Jobs

Edit cron jobs

```bash
crontab -e
```

View cron jobs

```bash
crontab -l
```

Example

```cron
0 2 * * * /home/user/backup.sh
```

Runs every day at 2:00 AM.

---

# Networking

Useful commands

```bash
ip addr
hostname
ping
```

---

# Key Takeaways

- apt manages software packages.
- SSH allows secure remote access.
- SCP securely transfers files.
- Cron automates repetitive tasks.
- systemctl manages services.

---

# Commands Learned

- apt
- systemctl
- ssh
- scp
- wget
- curl
- crontab
- hostname
- ping
- ip

---

# Skills Gained

- Package management
- Service administration
- Remote access
- Automation
