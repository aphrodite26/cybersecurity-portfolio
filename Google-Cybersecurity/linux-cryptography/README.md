# Linux Cryptography Lab — File Decryption

## Overview
Completed as part of the Google Cybersecurity Certificate — Assets, Threats, and Vulnerabilities course.

This hands-on lab focused on using Linux commands to locate hidden files, decrypt a Caesar cipher, and recover an encrypted file using OpenSSL.

## Tasks Completed
- Explored directories and identified hidden files using `ls`, `ls -a`, and `cat`.
- Decrypted a Caesar cipher using the `tr` command.
- Decrypted an AES-256-CBC encrypted file using OpenSSL.
- Recovered and read the original file contents.

## Commands Used

**Caesar Cipher Decryption**
```bash
cat .leftShift3 | tr "d-za-cD-ZA-C" "a-zA-Z"
```

**AES-256-CBC File Decryption**
```bash
openssl aes-256-cbc -pbkdf2 -a -d -in Q1.encrypted -out Q1.recovered -k <password>
```

## Skills Demonstrated
- Linux Command-Line Operations
- Hidden File Discovery
- Basic Cryptography
- Caesar Cipher Decryption
- AES-256-CBC File Decryption
- OpenSSL

## Outcome
Successfully decrypted the hidden instructions and recovered the encrypted file using Linux command-line tools.
