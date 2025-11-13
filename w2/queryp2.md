# CS50 Query Part 2 
## Part of the attendance post for this week's work

Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 0 - Querying](https://youtu.be/vHYeChEf2lA?si=hKFR9GDxKMU2JEYo)

## Setup
- From your codespace terminal make sure your current directory is the querying folder and then copy the following command and paste into the terminal:
- ```curl -o longlist.db https://raw.githubusercontent.com/CIT28/files/main/w2/longlist.db```

- Now create a new file named p2-q.sql and copy this code into that file, I'll go over what is happening in each line of this code:
```
-- starting the pow workflow
-- changes terminal output for readability 
.mode box
  
-- changes terminal output from standard output (stdout) to pow.txt file
.output '| cat >> pow.txt'
  
-- updates the pow.txt with content in single quotes
.print 'first query'  
  
-- SQL command (query) to view all the column contents in the longlist table   
-- Copy your SQL command below here

SELECT * FROM "longlist";
  
-- After each commit comment out the queries written and then continue to write your queries in this part of the file

-- changes back to stdout    
.output stdout  

-- bash command sqlite3 longlist.db < p2-q.sql
```
- Before you start watching the video in your README.md file use a h1 (#) and this text - "Week 2 Querying Part 2", then commit with message:
  - **COMMIT MESSAGE - "setup ready"** 

## Timemark 12:25 to 21:49
- After watching my video, start at 12:25 and then follow along with the Carter and write the SQL commands (query) in the terminal and once query runs without error copy it into query file (p2-q.sql) for this one there will be 3 queries. Complete the proof of work (pow) and git workflow and commit with message:
  - **COMMIT MESSAGE - "SELECT command"**

- Continue from 16:32 and listen to the questions asked and add any question(s) here you might have encounter and make sure you answer why we use style for our SQL commands in the README.md file at 19:37. Complete git workflow and commit with message:
  - **COMMIT MESSAGE - "questions and style"**

- Comment out previous queries  
- Continue coding along from 19:37 and learn the LIMIT SQL command and once you reach 21:49 there should be 2 queries for this commit, then complete the pow and git workflow and commit with message:
  - **COMMIT MESSAGE - "LIMIT command"**
  
- Complete instructions in canvas for attendance post requirements.
