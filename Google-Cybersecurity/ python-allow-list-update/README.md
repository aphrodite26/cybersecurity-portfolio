# Python Algorithm for Updating an IP Address Allow List

## Project Overview

This project was completed as part of the **Google Cybersecurity Professional Certificate — Course 7: Automate Cybersecurity Tasks with Python**.

The objective was to develop a Python algorithm that automates the maintenance of an IP address allow list used to control access to sensitive patient information within a healthcare organization.

The algorithm reads authorized IP addresses from a text file, compares them against a list of addresses that should be removed, and updates the original file accordingly.

## Security Objectives

- Maintain accurate network access permissions.
- Remove IP addresses that are no longer authorized.
- Apply the principle of least privilege.
- Automate repetitive security administration tasks.
- Reduce the risk of outdated access permissions.

## Algorithm Workflow

1. Open the file containing the authorized IP addresses.
2. Read the contents using Python file operations.
3. Convert the contents into a list using `.split()`.
4. Iterate through the list of IP addresses that must be removed.
5. Check for matching addresses and remove them using `.remove()`.
6. Convert the updated list into a string using `.join()`.
7. Write the revised list back to the original file.

## Python Concepts Applied

- File handling with `open()` and `with`
- Reading and writing text files
- String manipulation
- Lists and iteration
- `for` loops
- Conditional statements
- Membership testing with `in`
- List modification using `.remove()`

## Project Documentation

[View the complete Python Algorithm Report](Algorithm_for_file_updates_in_Python.pdf)

The report includes a detailed explanation of each stage of the algorithm, the Python functions and methods used, and their relevance to cybersecurity access control.

## Skills Demonstrated

**Python Programming | Security Automation | Access Control | File Handling | List Manipulation | Least Privilege**
