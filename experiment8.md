<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 53 17 AM" src="https://gist.github.com/user-attachments/assets/725335bc-cbc0-4c70-8eba-cd5c0e20beb6" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 54 13 AM" src="https://gist.github.com/user-attachments/assets/0a5bef60-f610-4ac2-9957-fcc6b7930192" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 55 10 AM" src="https://gist.github.com/user-attachments/assets/7f17a1ac-86ee-478e-a18f-f6f0e8df799c" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 56 31 AM" src="https://gist.github.com/user-attachments/assets/81107449-1f1c-4b91-a16f-352a4f1dd2d3" />
# Experiment 8: Shell Programming (Continuation)

## Objective
To continue exploring shell programming concepts in Linux by implementing control structures, loops, and basic shell utilities.

---

## Theory

Shell scripting allows automation of tasks in Unix/Linux systems.  
In continuation of the previous experiment, this session focuses on:

- **Conditional statements** (`if`, `if-else`, `if-elif-else`)
- **Looping constructs** (`for`, `while`, `until`)
- **Case statements**
- **User-defined functions**
- **Command line arguments**

---

## Programs and Examples

### 1. Using Conditional Statements
```bash
#!/bin/bash
echo "Enter a number:"
read num
if [ $num -gt 0 ]; then
  echo "Number is positive"
elif [ $num -lt 0 ]; then
  echo "Number is negative"
else
  echo "Number is zero"
fi



## 2. Process Monitoring and Resource Usage
Linux provides commands to monitor processes and system resources:

- `top` → live view of processes, CPU, and memory usage.
- `htop` → user-friendly version of `top` (if installed).
- `ps aux` → snapshot of all processes.
- `free -h` → shows memory usage in human-readable format.
- `uptime` → shows system load averages.

**Example Commands:**
```bash
top
ps aux
free -h
uptime
# Experiment 8: Shell Programming (Continuation)

---

## 3. Process Communication

Processes in Linux can communicate with each other using:

1. **Files** – one process writes to a file and another reads from it.  
2. **Pipes (`|`)** – pass the output of one command as the input to another.  
3. **Sockets** – enable communication between processes, even across networks (advanced concept, not covered in this lab).

---

### Example: Using Pipes
A common example of process communication is using pipes:

```bash
ps aux | grep bash
# Experiment 8: Shell Programming (Continuation)

---

## 4. Process Synchronization

### Concept
- When multiple processes run in parallel, conflicts may occur if they access the same resources.  
- **Process synchronization** ensures that processes execute in a controlled manner.  
- In shell scripting, the most common way of synchronizing is by using the **`wait`** command.

---

### `wait` Command
- `wait` makes the shell pause until all background jobs are finished.  
- Useful when a script launches background tasks but needs
# Experiment 8: Shell Programming (Continuation)

---

## 5. Background Processes and Job Control

### Concept
- In Linux, processes can be run in the **foreground** (default) or the **background**.  
- Running jobs in the background allows the user to continue using the terminal while the process executes.  
- Linux provides commands to manage these jobs efficiently.

---

### Running a Background Process
- Add `&` at the end of a command to run it in the background.

**Example:**
```bash
sleep 30 &