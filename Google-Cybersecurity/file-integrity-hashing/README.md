# File Integrity Verification Using SHA-256

## Overview
Completed as part of the Google Cybersecurity Certificate — Assets, Threats, and Vulnerabilities course.

This hands-on lab focused on using SHA-256 hashing and Linux commands to verify file integrity and identify differences between files that appeared identical.

## Tasks Completed
- Examined file contents using `cat`.
- Generated SHA-256 hashes using `sha256sum`.
- Saved hash values to separate files using output redirection.
- Compared hash values using `cmp`.
- Identified differences between two files with visually identical contents.

## Commands Used

```bash
cat file1.txt
cat file2.txt

sha256sum file1.txt
sha256sum file2.txt

sha256sum file1.txt >> file1hash
sha256sum file2.txt >> file2hash

cmp file1hash file2hash
```

## Key Finding
Although the files appeared identical when displayed in the terminal, their SHA-256 hashes differed, indicating that their underlying contents were not identical.

## Skills Demonstrated
- SHA-256 Hashing
- File Integrity Verification
- Linux Command-Line Operations
- Hash Comparison
- Data Integrity Analysis
