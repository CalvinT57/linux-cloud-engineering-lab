# Linux Cloud Engineering Lab

## Overview

This repository documents my hands-on Linux learning journey with a focus on cloud engineering, system administration, networking, services, remote access, and troubleshooting.

Rather than only memorizing Linux commands, I am building a working Linux environment and using it to practice tasks that relate directly to real cloud and infrastructure roles.

## Lab Environment

- Host System: macOS
- Virtualization: UTM
- Guest OS: Ubuntu Linux
- Remote Access: SSH
- Web Server: Nginx
- Linux Hostname: `linux-lab`

## What I Have Completed

- Installed Ubuntu Linux in UTM
- Updated the Linux system using `apt`
- Practiced Linux file and directory navigation
- Created, copied, moved, renamed, and deleted files
- Reviewed Linux logs in `/var/log`
- Used `journalctl` to inspect system activity
- Checked for failed services with `systemctl`
- Installed and enabled OpenSSH
- Connected remotely from macOS to Ubuntu using SSH
- Verified Linux networking and the VM IP address
- Installed Nginx
- Verified the Nginx service was running
- Accessed the Nginx web server from the macOS browser

## Commands Practiced

```bash
pwd
ls
ls -la
cd
mkdir
touch
cp
mv
rm
cat
echo
grep
tail
whoami
hostname
ip addr
journalctl
systemctl
ssh
sudo
apt
```

## System Logging and Troubleshooting

I explored Linux log files stored under:

```bash
/var/log
```

I used commands such as:

```bash
journalctl -n 20
journalctl -p err -n 20
systemctl --failed
```

This helped me understand how Linux administrators review system activity, identify errors, and troubleshoot services.

## SSH Remote Administration

I installed the OpenSSH server on Ubuntu:

```bash
sudo apt install openssh-server
```

I verified that the SSH service was running:

```bash
systemctl status ssh
```

I then connected remotely to the Ubuntu VM from macOS using SSH.

This gave me hands-on experience with remote Linux administration, which is commonly used when managing cloud servers and virtual machines.

## Nginx Web Server

I installed Nginx on the Ubuntu system:

```bash
sudo apt install nginx -y
```

I verified that the Nginx service was running:

```bash
systemctl status nginx
```

I then accessed the web server from the macOS host using the Ubuntu VM's private IP address.

This allowed me to validate that the Linux server was successfully hosting a web service that could be reached from another system.

## What I Learned

This lab helped me understand how Linux is used for server administration, remote access, networking, service management, package management, logging, and troubleshooting.

It also gave me hands-on experience managing a Linux server remotely and deploying a working web service.

I am continuing to build this environment as I develop Linux and cloud engineering skills.

## Next Steps

- Linux users and groups
- File permissions and ownership
- UFW firewall configuration
- SSH hardening
- Bash scripting
- Cron jobs
- Nginx configuration
- Git
- Docker
- Cloud deployment
- Infrastructure automation
