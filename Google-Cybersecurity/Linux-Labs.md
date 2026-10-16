# Linux Practical Labs

**Course:** Google Cybersecurity Professional Certificate  
**Module:** Tools of the Trade: Linux and SQL  
**Environment:** Debian-based Linux

## Overview

Completed hands-on Linux labs focusing on Bash commands, package management, file system navigation, log analysis, file management, user administration, and access permissions.

The activities provided practical experience with Linux system administration and security-related operations.

## Completed Labs

### 1. Install Software in a Linux Distribution

- Managed software packages using APT and sudo.
- Installed, removed, and reinstalled nload.
- Installed tcpdump.
- Verified installed packages.

**Example Commands:**

```bash
sudo apt install nload
sudo apt remove nload
sudo apt install nload
sudo apt install tcpdump
apt list --installed
```

These commands demonstrate software installation, removal, and package verification using APT.

**Commands:** `apt`, `sudo apt install`, `sudo apt remove`

### 2. Examine Input/Output in the Linux Shell

- Generated terminal output using echo.
- Performed calculations using expr.
- Cleared terminal output.

**Example Commands:**

```bash
echo "Hello, Linux!"
expr 10 + 5
clear
```

These commands demonstrate basic terminal interaction, arithmetic operations, and output management.

**Commands:** `echo`, `expr`, `clear`

### 3. Navigate the Linux File System

- Navigated directories and located files.
- Examined user records.
- Read server log files.

**Example Commands:**

```bash
pwd
ls
cd /var/log
ls
head /etc/passwd
cat /etc/passwd
```

These commands demonstrate directory navigation, file listing, and reading system information.

**Commands:** `pwd`, `ls`, `cd`, `cat`, `head`

### 4. Filter Files and File Contents

- Searched server logs for error messages.
- Filtered filenames using pipes.
- Searched user records for specific information.

**Example Commands:**

```bash
grep "error" /var/log/syslog
ls | grep ".txt"
grep "root" /etc/passwd
```

The `grep` command searches for matching text, while the pipe operator (`|`) passes the output of one command to another.

**Commands:** `grep`, `|`

### 5. Manage Files and Directories

- Created and removed directories.
- Moved and deleted files.
- Created and edited text files.

**Example Commands:**

```bash
mkdir test_directory
touch notes.txt
mv notes.txt test_directory/
nano test_directory/notes.txt
rm test_directory/notes.txt
rmdir test_directory
```

These commands demonstrate file creation, organization, editing, and deletion.

**Commands:** `mkdir`, `rmdir`, `mv`, `rm`, `touch`, `nano`

### 6. Manage File Permissions

- Examined file and directory permissions.
- Identified hidden files.
- Modified permissions to restrict access.
- Applied least-privilege principles.

**Example Commands:**

```bash
ls -l
ls -la
chmod 600 notes.txt
ls -l notes.txt
```

The `chmod 600` command restricts file access to the owner, allowing read and write permissions while removing access for group members and others.

**Commands:** `ls -l`, `ls -la`, `chmod`

### 7. Manage Users and Groups in Linux

- Created a new Linux user.
- Assigned a primary group.
- Changed file ownership.
- Added a user to a supplementary group.
- Removed a user account.
- Deleted an unused group.
- Practiced managing user access throughout the employee lifecycle.

**Example Commands:**

```bash
sudo useradd analyst1
sudo usermod -g developers analyst1
sudo chown analyst1 report.txt
sudo usermod -aG security analyst1
sudo userdel analyst1
sudo groupdel security
```

These commands demonstrate user account administration, group membership management, and file ownership changes. The examples assume that the referenced groups and files already exist.

**Commands:** `sudo`, `useradd`, `usermod`, `chown`, `userdel`, `groupdel`

## Skills Practiced

- Linux command-line operations.
- Software and package management.
- File system navigation.
- Searching and filtering log files.
- File and directory management.
- Linux permissions and least privilege.
- User and group administration.
- Basic Linux system security.

---

See [Linux File Permissions](File_permissions_in_Linux.pdf) for the detailed portfolio project.

*Completed as part of the Google Cybersecurity Professional Certificate. Command examples illustrate the techniques practiced during the labs.*

