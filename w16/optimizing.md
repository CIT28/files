# CS50 Optimizing
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 1 - Optimizing](https://www.youtube.com/watch?v=qa5-mKVSQHQ)

## Attendance
### Time mark 00:00 to 20:36
- Create a new folder at the same level as viewing and name it optimizing, create a new sql file named q.sql.
- In the optimizing folder get the movies.db
    - ```curl -o movies.db https://raw.githubusercontent.com/CIT28/files/main/w16/movies.db```
- Code along with Carter until time mark 20:36 and order your the code so that you can use the timer output of user to determine how much faster the find Cars title query runs without and index and with using timer and explain query plan. 
- Here is my output of running my query file:
```
Drop Index
Run query to find cars using explain query plan
Timer on
---
QUERY PLAN
`--SCAN movies
Run Time: real 0.000 user 0.000065 sys 0.000024
---
Create index for title
Run Time: real 0.183 user 0.156494 sys 0.021929
---
Explain Query Plan after index
QUERY PLAN
`--SEARCH movies USING INDEX title_index (title=?)
Run Time: real 0.000 user 0.000019 sys 0.000002
---
(0.000065 - 0.000019)/0.000065 * 100 = 70
Index decreased user time to run query by 70% on my local system
```
- How to calculate percent decrease 
    - (Original time - New time) / Original time x 100
- Output the query to time.txt     

    - **COMMIT MESSAGE - "timer report done"**

# Time Mark 20:36 to 49:06
- Code along with Carter in the q.sql before Carter discussed covering index, output the q.sql with timer on to the pow.txt.
- Then continue to code along with Carter to code the next covering index and like we did on attendance, determine the percentage decrease of the query without the index compared to the covering index. Using the .print output that to the pow.txt. Mine was 99% decrease WOW!
- Now listen to Carter discuss the B-Tree structure for creating indexes, the associated "cost" and searching algorithm. Then create a README.md add a heading and summary your understanding of concepts covered.  
    - **COMMIT MESSAGE - "how indexes are created and used"**

# Time Mark 49:05 to ?
- Now add heading for partial index and add your understanding of the how and why of this concept.
- Then code along to code the partial index and see how much faster the query for 2023 was compared to 1998.
- Output the .schema to the pow.txt
- Now add a heading for Vacuum and listen and then write your understanding of this concept and then 