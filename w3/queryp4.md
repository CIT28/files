## CS50 Query Part 4
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 0 - Querying](https://youtu.be/vHYeChEf2lA?si=hKFR9GDxKMU2JEYo)

## Setup
- Create a new folder named w3, which will be at the same folder level as w1 and copy the querying.md file from w2 into w4. Like before, you don't need to copy the longlist.db, but you would need to use this command to open it from w1:
```sqlite3 ../w1/longlist.db```
- Make sure you are in the w4 folder for this command to work. 
## Timemark 46:01 to the end
- Start watching in 46:01 and take notes on the operators covered in your querying.md file
- Then follow along with the video and complete the SQL to learn about the RANGE command, create a sql file named range.sql and in there write each sql statement that is covered in this part of the video, make sure you run it from the command line: ```.read range.sql``` 
- There will be 4 different sql statement covered there, comment out ```/* SQL */``` once you know it run correctly.
- Listen to the questions asked and add any question here you might have encounter. If you don't have questions then capture at least 2 of the questions asked in your querying.md file.
- Continue to follow along with the video and write the upated LIKE statements and once working add that into your range.sql file. 
- Make sure to take note of the difference between LIKE and = in your querying.md file. For this work you should have 6 SQL statement and the last one will be uncommitted one.  
- Copy all the terminal output into a new file named pow1.txt, stop at 53:10.
- **COMMIT MESSAGE - "terminal output from RANGE and QA"**
- Stop and start your sqlite terminal session to clear the output.  
- Start watching in 53:10 and take notes on the ORDER BY commands that will be covered in thie video, do this in your querying.md file. 
- Then follow along with the video and complete the SQL to learn about the ORDER BY command, create a sql file named orderby.sql and in there write each sql statement that is covered in this part of the video, make sure you run it from the command line: ```.read order.sql```.   
- Continue following along with the video, making sure you are adding new sql statement and running them from the command line for your pow file.  
- Copy all the terminal output into a new file named pow2.txt, stop after the conclusion.
- There should be 7 sql statement in your orderby.sql file.  
- **COMMIT MESSAGE - "terminal output from ORDER BY commands**
- Stop and start your sqlite terminal session to clear the output.  
- Start watching in 1:02 and take notes on the aggregate SQL commands that will be covered in thie video, do this in your querying.md file. 
- Then follow along with the video and complete the SQL to learn about the aggregate sql commands, create a sql file named aggregate.sql and in there write each sql statement that is covered in this part of the video, make sure you run it from the command line: ```.read aggregate.sql```. I did noticed that only when I used the ```.mode box``` did I see the heading on the ROUND output.  
- Add to your begining comment above regarding a more complete explaination of aggregate commands.
- Continue following along with the video, making sure you are adding new sql statement and running them from the command line for your pow file.  
- Interesting point about how MAX and MIN does not really work on the title column and using the DISTINCT together with the count.   
- Copy all the terminal output into a new file named pow3.txt, stop after the conclusion.
- There should be 13 sql statement in your aggregate.sql file.    
- **COMMIT MESSAGE - "terminal output from aggregate SQL commands**
- Submit your commit history URL your w3 in your private repo for grading
## Grading
This is how I will grade your work:
  1. Did you provide the correct URL for w3 folder - 15 points
  2. Did you do all the commits required for this work - 25 points
  3. Did you create the pow1.txt, pow2.txt and include all the required output - 35 points
  4. Did you include all the required content in the the markdown file and did you have all the sql statements in the 3 sql files (range.sql, orderby.sql and aggrgate.sql) - 45 points
  5. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 

