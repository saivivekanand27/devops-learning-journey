# 🚀 DevOps Learning Journey – Day 6  
## Linux, Operating System & Shell Basics

---

## 1. Agenda of the Session

- What is an Operating System (OS)
- Why Linux is widely used
- Basic Linux Architecture
- Introduction to Shell & Shell Scripting
- Important Linux Commands

---

## 2. What is an Operating System?

### Definition

An Operating System (OS) is:

👉 A bridge between Software and Hardware

### System Flow

User → Application → Operating System → Hardware  
Hardware → OS → Application → User  

### Hardware Components

- CPU  
- RAM  
- Disk (I/O)

### Key Idea

- ❌ Without OS: Software cannot directly interact with hardware  
- ✅ OS manages everything  

---

## 3. Examples of Operating Systems

- Windows  
- Linux  
- macOS  

---

## 4. Why Linux is Popular in DevOps

### 1. Free & Open Source
- No license cost  
- Anyone can modify  

### 2. Security
- More secure than Windows  
- Minimal need for antivirus  

### 3. Performance
- Lightweight  
- Handles high traffic  

### 4. Stability
- Rare crashes  
- Best for production  

### 5. Multiple Distributions

- Ubuntu  
- CentOS  
- Debian  
- Red Hat  
- Alpine  

👉 **80–90% of servers run on Linux**

---

## 5. Linux Architecture (Simplified)

Applications  
↓  
System Libraries  
↓  
Kernel  
↓  
Hardware  

### Kernel (Heart of OS)

Responsibilities:

- Device Management  
- Memory Management  
- Process Management  
- System Calls  

### System Libraries

- Provide functions to applications  
- Example: libc  

### User Layer

- Compilers  
- Tools  
- Applications  

---

## 6. What is Shell?

👉 Shell is a way to communicate with OS using commands  

### Why Shell?

- No GUI in real servers  
- Everything is command-based  

### Example

Windows → Click to create file  
Linux → `touch file.txt`

---

## 7. Shell Types

- bash (recommended)  
- zsh  
- sh  
- ksh  

---

## 8. Connect to Linux Server (EC2)

```bash
ssh -i key.pem ubuntu@<public-ip>

9. Basic Linux Commands
Check Current Directory
pwd
List Files
ls
Detailed List
ls -ltr
Change Directory
cd foldername
Go Back
cd ..
Create File
touch filename
Edit File
vi filename

Steps in vi:

Press i

Type content

Press Esc

Type :wq

View File
cat filename
Create Directory
mkdir foldername
Delete File
rm filename
Delete Folder
rm -r foldername
10. System Monitoring Commands
Memory
free -h
CPU
nproc
Disk
df -h
Full Monitor
top
11. Important Interview Questions

What is OS?

What is Kernel?

Why Linux over Windows?

Public IP vs Private IP

What is Shell?

Linux commands

Monitoring tools (top, free, df)

12. Real DevOps Usage

No GUI

Everything via Shell

Used for:

Server management

Automation

Deployment

13. Shell Scripting (Intro)
What is Shell Script?

👉 File containing multiple commands

Example
#!/bin/bash
echo "Hello DevOps"
Why?

Automate tasks

Manage servers

Deploy apps

14. Key Takeaways

✔ OS connects hardware & software
✔ Linux is fast, secure, free
✔ Kernel is core
✔ Shell is interaction layer
✔ Commands are essential
✔ Automation starts here