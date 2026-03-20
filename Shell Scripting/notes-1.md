# 🐧 Shell Scripting Notes (Zero to Hero)

---

## Introduction

- Shell scripting is used to automate tasks in Linux.
- It is very important for DevOps engineers.
- It helps in handling repetitive and large-scale operations.
- Covers basics, commands, scripting, and real-world DevOps usage.

---

## Purpose of Scripting & Automation

- Automation means reducing manual effort.
- Used in both daily life and software systems.

### Example

- Writing numbers manually → possible for small range  
- Increasing numbers (1000, 10000...) → not practical  

### Conclusion

👉 Use shell scripting to automate repetitive tasks.

---

## How to Create a File

```bash
touch file.sh

Creates an empty file

.sh is the extension for shell scripts

How to List Files & Folders
ls
Important Command
ls -ltr

Displays:

File permissions

Owner

Size

Timestamp

Sorted by time (latest at bottom)

man Command
man ls

Displays documentation/manual of commands

vi / vim Editor
vim file.sh
Steps

Press i → enter insert mode

Write content

Save & Exit

Esc :wq! → Save and exit

Esc :q! → Exit without saving

Difference: touch vs vim
Command	Purpose
touch	Creates empty file
vim	Create + edit file
Copy Content in vim

yy → copy line

p → paste

Shebang (#!)
#!/bin/bash

Must be the first line of script

Purpose

Defines which shell executes the script

Shell Types
Shell	Description
bash	Most commonly used
sh	Basic shell
dash	Lightweight & faster
ksh	Advanced scripting shell
Insert Command (vim)

i → insert mode

Esc → exit insert mode

echo Command
echo "Hello World"

Prints output to terminal

Execute Shell Script
sh file.sh

OR

./file.sh
Grant Permissions
chmod 777 file.sh
chmod Explanation
Value	Meaning
4	Read
2	Write
1	Execute

👉 7 = Full access (4+2+1)

Examples
chmod 777 file.sh
chmod 444 file.sh
chmod 700 file.sh
chmod 111 file.sh
History Command
history

Shows previously executed commands

Commands Covered So Far

touch

ls

ls -ltr

man

vim

cat

echo

chmod

history

File & Directory Commands
Create Folder
mkdir folder_name
Change Directory
cd folder_name
cd ..
Present Working Directory
pwd
Delete Files & Folders
rm file
rm -rf folder
Simple Shell Script Example
#!/bin/bash

mkdir Abhishek
cd Abhishek
touch file1
touch file2
Run Script
chmod 777 script.sh
./script.sh
Verify Output
ls
cd Abhishek
ls
Shell Scripting in DevOps
Scenario

DevOps engineers manage multiple servers.

Problems

High CPU usage

Memory issues

System monitoring

Solution

Write scripts to:

Check system health

Monitor CPU & memory

Automate tasks

Automation

Use cron jobs to schedule scripts

Check CPU & RAM
nproc
free
top
top Command
top

Displays:

CPU usage

Memory usage

Running processes

Process IDs

Comments in Shell Script
# This is a comment
Advanced Topics Mentioned

Trap signals (Ctrl + C handling)

Cron jobs

Intermediate & advanced scripting

Final Understanding

✔ Shell scripting = automation tool for Linux
✔ Widely used in DevOps
✔ Saves time and effort
✔ Essential for managing large-scale systems