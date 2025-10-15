<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 53 10 AM" src="https://gist.github.com/user-attachments/assets/655ac6a5-7e22-4b17-b022-78d1c203577b" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 51 23 AM" src="https://gist.github.com/user-attachments/assets/755a7ea9-79fd-48aa-88cf-8f0691cd8b8f" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 49 10 AM" src="https://gist.github.com/user-attachments/assets/1d6d2f85-2dcd-4c70-83e7-d806ae6fdcff" />
# Experiment 7: Shell Programming, Process and Scheduling

## Aim
To understand process management in Linux using shell programming and study process scheduling.

---

## Objectives
- Learn to create and manage processes using shell commands.  
- Explore foreground and background execution of processes.  
- Implement shell programs that demonstrate process scheduling.  
- Observe the use of commands like `ps`, `top`, `kill`, `jobs`, `nice`, and `renice`.

---

## Theory
A **process** is a running instance of a program in Linux. Each process has:
- **PID** (Process ID)  
- **PPID** (Parent Process ID)  
- **State** (Running, Sleeping, Zombie, etc.)  

Processes can run in the **foreground** (blocking the terminal) or in the **background** (appending `&`).  
Linux uses a **priority-based scheduler** where priorities are controlled by `nice` and `renice`.  

---

## Commands Used
- `ps` → Displays active processes  
- `top` → Shows real-time process usage  
- `jobs` → Lists background jobs  
- `fg` / `bg` → Moves jobs to foreground or background  
- `kill <pid>` → Terminates a process  
- `nice -n <value> <command>` → Starts a process with priority  
- `renice <value> -p <pid>` → Changes priority of a running process