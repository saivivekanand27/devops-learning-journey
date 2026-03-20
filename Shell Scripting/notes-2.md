# Shell Scripting Notes – Day 2 (Advanced + DevOps Use Cases)

---

## DevOps Use Case: Node Health Check

As a DevOps engineer, a common task is checking server (node) health.

### Includes:

- CPU usage  
- Memory usage  
- Disk usage  
- Running processes  

---

## Sample Node Health Script

```bash
#!/bin/bash

echo "Checking CPU Usage"
top

echo "Checking Memory Usage"
free -m

echo "Checking Disk Usage"
df -h
Explanation

echo → Improves readability

top → CPU usage

free -m → Memory usage

df -h → Disk usage

Good Practices in Shell Scripting
1. Always Use Shebang
#!/bin/bash

Tells system to use bash interpreter

Required when running using ./script.sh

2. Use echo for Readability
echo "===== CPU ====="
3. Debugging using set -x
set -x

Shows each command before execution

Commands for Node Health
CPU
top
Memory
free -m
Disk
df -h
Processes
ps -ef
How to Execute Script
chmod +x script.sh
./script.sh
Debug Mode
set -x

Prints each command

Useful for troubleshooting

Processes & PID
List processes
ps -ef
Filter process
ps -ef | grep nginx

grep filters output

grep Command
grep "text" file.txt

Used to:

Search text in files

Filter output

Pipe (|)
command1 | command2

Output of command1 becomes input of command2

Example
ps -ef | grep java
Interview Point (Pipe)

Pipe checks only the last command status

This can hide errors

awk Command
awk '{print $4}' file.txt

Used for:

Extracting columns

Combined Example
grep "employee" file.txt | awk '{print $4}'
set -e
set -e

Stops script immediately if any command fails

Problem without it

Script continues even if error occurs

set -o pipefail
set -o pipefail

Ensures failure if any command in pipe fails

Combined Best Practice
set -e
set -o pipefail
set -x
DevOps Use Case: Log Analysis

Logs are:

Very large

Stored remotely (S3, GitHub, etc.)

curl Command
curl <url>

Used to:

Fetch data

Call APIs

Retrieve logs

Example
curl log_url | grep ERROR
wget Command
wget <url>

Downloads files

curl vs wget
curl	wget
Shows output	Downloads file
API calls	File download
find Command
find / -name filename

Searches entire system

sudo and su
Switch user
su username
Root access
sudo su -

sudo gives temporary admin access

if-else in Shell
if [ $a -gt $b ]
then
  echo "A is greater"
else
  echo "B is greater"
fi
Notes

No spaces in variable assignment

fi ends the if block

for Loop
for i in {1..10}
do
  echo $i
done

Used for repeating tasks

trap Command
trap "echo Don't press Ctrl+C" SIGINT

Handles signals

Signals

Ctrl + C → SIGINT

kill → SIGKILL

Real DevOps Use Case

If a script stops midway, it may cause data inconsistency.

Solution
trap "cleanup code" SIGINT
Final Summary

Node monitoring script

Debugging using set -x

Error handling using set -e, pipefail

grep, awk, pipe usage

curl, wget

find command

sudo usage

loops (if, for)

trap signals