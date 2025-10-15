# Linux File Manipulation and System Management Tutorial

##  Introduction
Linux is a powerful open-source operating system widely used in servers, development, and embedded systems.  
This tutorial covers **file manipulation** and **basic system management** commands essential for beginners and professionals.

---

##  1. File Manipulation

### 1.1 Navigating Directories
```bash
pwd                 # Show current directory
ls                  # List files
ls -l               # Long listing with permissions
cd /home/user/      # Change directory
cd ..               # Go one level up
touch file1.txt         # Create empty file
nano file2.txt          # Open file in nano editor
vi file3.txt            # Open file in vi editor
cat file1.txt           # Display content
less file1.txt          # Scroll through file
head -n 10 file1.txt    # Show first 10 lines
tail -n 10 file1.txt    # Show last 10 lines
tail -f logfile.log     # Live updates
cp file1.txt copy_file.txt   # Copy file
mv file1.txt newname.txt     # Rename/Move file
rm file1.txt                 # Delete file
mkdir new_folder             # Create directory
rmdir old_folder             # Remove empty directory
rm -r folder_name            # Remove directory with files
cp -r dir1 dir2              # Copy directory with contents
ls -l
┌─────────────────────┐
        │ User runs:          │
        │ touch file          │
        └─────────┬───────────┘
                  │
                  ▼
      ┌─────────────────────────┐
      │ Where is command run?   │
      │ Current directory = ?   │
      └─────────┬───────────────┘
                │
   ┌────────────┴─────────────┐
   │ Inside / (root dir)?     │
   └───────┬─────────┬────────┘
           │Yes       │ No
           ▼          ▼
 ┌────────────────┐   ┌─────────────────────┐
 │ Normal user     │   │ Inside /home/user   │
 │ has no write    │   │ User has permission │
 │ permission here │   │ File created        │
 └───────┬────────┘   └───────────┬─────────┘
         │                        │
         ▼                        ▼
 Permission Denied       File Created 
