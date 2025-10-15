<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 26 16 AM" src="https://gist.github.com/user-attachments/assets/866378f3-24b5-4857-a885-20265b16cdaa" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 27 23 AM" src="https://gist.github.com/user-attachments/assets/4bd928f9-f317-4dd9-a63b-3a5fdfadd552" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 28 33 AM" src="https://gist.github.com/user-attachments/assets/83a3ee46-087f-4148-b731-ad9137775b45" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 30 31 AM" src="https://gist.github.com/user-attachments/assets/327203f0-c8c4-48b8-ba01-4b6b54f71d64" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 32 38 AM" src="https://gist.github.com/user-attachments/assets/286e00f0-eecf-4fca-8637-a9f95b6a8ea5" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 38 25 AM" src="https://gist.github.com/user-attachments/assets/4c0bc152-6cd1-466f-9ed4-31d06da4ddd3" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 36 49 AM" src="https://gist.github.com/user-attachments/assets/2be3e8a1-cf07-46bd-be84-73f3052b6b78" />
<img width="1710" height="1107" alt="Screenshot 2025-10-15 at 11 34 13 AM" src="https://gist.github.com/user-attachments/assets/43af74b1-e9a5-407d-9653-64a732940fd8" />
## Objective

To understand and implement different types of loops (`for`, `while`, and `until`) in shell scripting to automate repetitive tasks and efficiently process data.

---

## Software & Tools Required

- OS: Linux (Ubuntu preferred)
- Shell: Bash
- Editor: vi, nano, or any text editor

---

## Theory

Shell loops are fundamental constructs used to execute commands repeatedly until a condition is met or over a predefined list. They help reduce manual effort in repetitive tasks such as iterating over files or reading input.

### 1. For Loop

Executes a block of code for each item in a list.

```bash
for i in 1 2 3
do
  echo $i
done
count=1
#### 2. While Loop
while [ $count -le 3 ]
do
  echo $count
  ((count++))
done
x=1
##### 3.  until
until [ $x -gt 3 ]
do
  echo $x
  ((x++))
done