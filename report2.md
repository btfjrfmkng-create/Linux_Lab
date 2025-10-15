#  Experiment 2: Linux File Systems, Permissions, and Essential Commands

##  Table of Contents
1. [Theory: Understanding Linux File Systems](#theory-understanding-linux-file-systems)  
2. [File Permissions](#file-permissions)  
3. [Users and Ownership](#users-and-ownership)  
4. [Basic Navigation Commands](#basic-navigation-commands)  
5. [File Operations](#file-operations)  
6. [File Viewing and Editing](#file-viewing-and-editing)  
7. [User Management](#user-management)  
8. [System Information](#system-information)  
9. [Practice Exercises](#practice-exercises)  

---

## 1. Theory: Understanding Linux File Systems
Linux uses a hierarchical file system structure:  
- Root directory `/`  
- Subdirectories like `/home`, `/etc`, `/usr`, `/var`  
- Everything in Linux is treated as a **file**, including devices.  
- **Absolute paths** start from `/`; **relative paths** start from the current directory.

---

## 2. File Permissions
Linux file permissions control access to files and directories:  
- **Permission types**:  
  - `r` – Read  
  - `w` – Write  
  - `x` – Execute  
- **Permission classes**:  
  - `u` – User (owner)  
  - `g` – Group  
  - `o` – Others  
- **View permissions**:  
  ```bash
  ls -l