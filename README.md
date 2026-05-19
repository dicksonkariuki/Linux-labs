# Linux-labs
This repository contains Linux Labs for Devops &amp; Cloud Engineers
# Create app.log,auth.log,system.log files

***touch app.log,auth.log,system.log***

# PART 1 — FIND COMMAND
# Task 1
Find all .log files.

***find . -name "*.log"***(for logs in the current directory)

![alt text](image-4.png)

# Task 2
Find only files containing “app” in filename.

***find . -type f -name "*app*"***

![alt text](image-5.png)

# Part 2 Locate Command 

# Task 3
Locate auth.log.

***locate auth.log***

![alt text](image-6.png)

# Part 3: Grep Command 
# Task 4
Find all ERROR messages in app.log.

***grep"ERROR" app.log***

![alt text](image-2.png)

# Task 5
Find all WARNING messages.

***grep "WARNING"app.log***

![alt text](image-3.png)

# Task 6
Count the number of ERROR entries.
Hint
Use piping with:
wc -l

***grep "ERROR" app.log| wc -l***

![alt text](image-7.png)

# Part 4 :AWK Command 
# Task 7
Print only timestamps from app.log.

***awk '{print$ 2}' app.log***

![alt text](image-8.png)

# Task 8
Print only usernames from successful login entries.

***awk 'NR==2 || NR==5' auth.log***

![alt text](image-9.png)

# Task 9
Extract disk usage percentages from system.log.

***awk 'NR==3 || NR==6' system.log**

![alt text](image-1.png)

# Part 5 -piping 
# Task 10 
Find ERROR logs and count them.

***grep -i "ERROR" app.log | wc -l***

![alt text](image-10.png)

# Task 11
Extract usernames and sort alphabetically.

***cut -d: -f3 app.log | sort***


![alt text](image-11.png)











