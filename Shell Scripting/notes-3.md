# Shell Scripting Notes – Day 3 (Advanced Concepts)

---

## 1. Variables in Shell

### Declaration

name="Vivek"
age=21

### Usage

echo $name
echo $age

### Important Rules

- No space in assignment  
- Use `$` to access variable  

---

## 2. User Input

read name
echo "Hello $name"

---

## 3. Command Line Arguments

echo $1
echo $2

### Example

./script.sh Vivek 21

Output:
Vivek
21

### Special Variables

$# → Number of arguments  
$@ → All arguments  
$? → Exit status  

---

## 4. Exit Status

- 0 → Success  
- Non-zero → Failure  

echo $?

---

## 5. Functions in Shell

my_function() {
  echo "Hello DevOps"
}

my_function

---

## 6. File Handling

### Check if file exists

if [ -f file.txt ]
then
  echo "File exists"
fi

### Check directory

if [ -d folder ]
then
  echo "Directory exists"
fi

---

## 7. String Operations

str="DevOps"

echo ${#str}   # length
echo ${str:0:3} # substring

---

## 8. Arithmetic Operations

a=10
b=5

echo $((a + b))
echo $((a * b))

---

## 9. Case Statement

case $1 in
  start)
    echo "Starting service"
    ;;
  stop)
    echo "Stopping service"
    ;;
  *)
    echo "Invalid option"
    ;;
esac

---

## 10. Cron Jobs (VERY IMPORTANT)

### Edit cron

crontab -e

### Example

* * * * * /home/script.sh

### Format

* * * * *
| | | | |
| | | | └ Day of week
| | | └ Month
| | └ Day
| └ Hour
└ Minute

---

## 11. Log Cleanup Script

#!/bin/bash

find /logs -type f -mtime +7 -delete

👉 Deletes logs older than 7 days

---

## 12. Disk Space Alert Script

#!/bin/bash

usage=$(df -h / | awk 'NR==2 {print $5}' | sed 's/%//')

if [ $usage -gt 80 ]
then
  echo "Disk usage is high: $usage%"
fi

---

## 13. Loop Through Files

for file in *.txt
do
  echo $file
done

---

## 14. While Loop

count=1

while [ $count -le 5 ]
do
  echo $count
  ((count++))
done

---

## 15. Best Practices

- Use meaningful variable names  
- Add comments  
- Use error handling  
- Avoid hardcoding paths  

---

## 16. Final Understanding

✔ Variables & inputs  
✔ Arguments handling  
✔ Functions  
✔ Cron jobs  
✔ Real DevOps scripts  
✔ Automation  

---