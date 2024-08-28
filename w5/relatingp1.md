## CS50 Relating Part 1
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 0 - Querying](https://www.youtube.com/watch?v=_2t18Hy9Z0Y)

## Setup
- I'll cover how to looks at .tables and schemes. 
- Create a new folder named relating at the same level as querying, then create the README.md and p1-r.sql files.
- From your codespace terminal make sure your current directory is relating folder and then copy the following command:
    - ```wget https://cdn.cs50.net/sql/2023/x/lectures/1/src1.zip```
    - Then you need to unzip the src1.zip with this:
    - ```unzip src1.zip```
- Before you start taking notes in your README.md file use a h1 (#) and this text - "Week 5 Relating Part 1" and commit with message:
    - **COMMIT MESSAGE - "src1 unzipped, query file and README.md ready"**
- Cover how to start sqlite3 with src1 files. 


## Timemark 26:35 to ?

- Start watching 26:35 and in your README.md file use a heading for "writing subquery one-to-many" and then under that heading take a few notes on subqueries and describe how we approaching writing them. No need to write the query yet, just follow along. Make sure to note which part of the subquery runs first and the syntax that is used to show the subquery and capture the questions. 
- Now code along in your p1-r.sql write the 2 queries and then comment them out before going on to do the subquery, once you get it to output the correct data, open another terminal and change run the sqlite3 shell and run this command .output powp1.txt and run the query. 
- Then start watching again at 37:25 as Carter writes another query and yes write each on seperately once it is working more do comment that out and write another query for average reting.  Once you get the average rating, output to the proof of work file.  At 40:26 you should have 7 queries in your p1-r.sql, then commit with message:
    - **COMMIT MESSAGE - "subqueries w one-to-many and notes"**
- Start back at 40:26 in your README.md and add a heading "writing nested subqueries with many-to-many" and under that heading write the approaching to writing this type of query. 
- Now code along in your p1-r.sql and make sure you write each query that will be in th nested query and once you get nested query creating the corret output, output to the proof of work file.  Listen to the question and take a few notes in your README.md file about your understanding of the "IN" SQL command. Then code up the example,  yes write each on seperately and once you get the correct output, update your proof of work file and then in your README.md write about indention styles and when to use "IN" and the difference between "IN" and =.  Listen to the last question and then commit with message:
    - **COMMIT MESSAGE - "subqueries w many-to-many and notes"**