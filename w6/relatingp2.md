## CS50 Relating Part 2
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 0 - Relating](https://www.youtube.com/watch?v=_2t18Hy9Z0Y)

## Setup
- Continue working in the relating folder usng the  then create the README.md and p2-r.sql files.
- get sealoins data
- ```curl -o sea_lions.db https://raw.githubusercontent.com/CIT28/files/main/w6/sea_lions.db```
- Before you start taking notes in your README.md file use a h1 (#) and this text - "Week 6 Relating Part 2" and commit with message:
    - **COMMIT MESSAGE - "db and README.md ready"**

## Timemark 55:50 to end

- Start watching 55:50 and in your README.md file use a heading for "JOINs" and then under that heading take a few notes on what JOIN does in our query. No need to write the query yet
- At 59:13, open the sea_loins.db by running the sqlite3 terminal with that db reference.  In the p2-r.sql write queries 3 queries, once you get it to output the correct data, open another terminal and change run the sqlite3 shell and run this command .output powp2.txt and run the queries. 
- At 1:02 make a new sub-heading named "Inter JOINs" and take notes on how they work and listens to question(s).
- Start back at 1:06  in your README.md and add a sub heading "Left, Right and Full Joins" and then code along with the example in your query file of the LEFT and RIGHT JOINs. 
- Then take a few notes in your README.md file for how the different JOINs logic works and add the additional details from the questions asked, Carter didn't update any code on that last question, but take note of the temp nature of the resulting table. Make sure to note that these are part of the family of OUTER JOIN. 
- Finish by coding the NATURAL example and take note of how it works as well.  
- There are a total of 4 queries here, so make sure you have updated your pow file and then commit with message:
    - **COMMIT MESSAGE - "Types of JOINs"**
## Consider Taking a break here!  

- Start watching 1:17 and in your README.md add a sub heading for "Sets", and take a few notes the different sets and SQL keywords (EXCEPT, INTERSECT).
- Now code along and code along with longlist.db, then write the first 2 queries, no need to output to proof of work file, but comment then out before writing the UNION queries and then output to the proof of work file. 
    - Thanks for Breanna for pointing this out! When changing db in sqlite3 you loss the .output, so you can name this proof of work file. pow2ll.txt (longlist ll)
- Finish writing the last 2 queries, update the proof of work file and add some notes from the quesitons asked, then at 1:31 commit with message:
    - **COMMIT MESSAGE - "Sets w EXCEPT INTERSECT"**
- Start wataching at 1:31 and in your README.md add a sub heading for "GROUP BY", then code along writing the 3 queries using GROUP BY make sure to have by AVG and COUNT here and the last example from the question and then watch until the end.  
    - **COMMIT MESSAGE - "GROUP BY"**

## Grading
This is how I will grade your work:
  1. Did you provide the correct commit history URL for relating folder = 5 points
  2. Did you do all the commits required for this work = 20 points
  3. Did you have all the queries in the p2-r.sql file = 25 points
  3. Did you create the powp2.txt file correctly and include all the required output = 20 points
  4. Did you include all the required content in the README.md file = 30 points
  5. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 