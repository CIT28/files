# CS50 Optimizing
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 1 - Optimizing](https://www.youtube.com/watch?v=qa5-mKVSQHQ)

## Attendance
### Time mark 00:00 to 20:36
- Create a new folder at the same level as viewing and name it optimizing, create a new sql file named q.sql.
- HEADS UP - I have had a student report that once they copied (wget) the movies.db into codespace, github throws an error when trying to push work to github because of the size of the movies.db files. 
    - Here are a couple of suggestions if you run into this issue:
        - Option 1 BEST OPTION - Since we have already created the .gitignore in week 1, so do this step before you to the wget command to copy the movies.db file, you can just add this into that file:
            - ```optimizing/movies.db```
            - Then do the git workflow using ```git add .gitignore```and then ```git commit -m "updating .gitignore"``` and then ```git push``` and now you can use the normal git commands and it will not track the movies.db file. 
            - I did notice I got the following message on the terminal while during the process of doing this update, but it worked fine, here was the message I got, so don't worry:
                <pre>
                The following paths are ignored by one of your .gitignore files:
                optimizing/movies.db
                hint: Use -f if you really want to add them.
                hint: Turn this message off by running 
                hint: "git config advice.addIgnoredFile false"
                </pre>
        - Option 2 - When running git add *, don't add the movies.db and only add the q.sql and the pow.txt. You can do this by changing the * to the specific file(s) like this:
            - ```git add q.sql```
            - ```git add pow.txt```
            - ```git add README.md```
                -  If you have already done the git add * and the movie.db is being tracked you can untrack it this way and then only stage (git add and git commit as shown above), then you can try this:
                - ```git rm --cached movies.db```
                - ```git commit -m "Remove movies.db from tracking``` 
        - Options 4 - You can also do a bit of research on who to handle large files on git. On my setup I had upgraded to the pro level github account and I did not get the error.  

- In the optimizing folder get the movies.db (MAKE SURE TO READ THE ABOVE INFORMATION FIRST)
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
- Output the query to timer.txt     

    - **COMMIT MESSAGE - "timer report done"**

## Time Mark 20:36 to 49:06
- Code along with Carter in the q.sql before Carter discussed covering index, output the q.sql with timer on to the pow.txt.
- Then continue to code along with Carter to code the next covering index and like we did on attendance, determine the percentage decrease of the query without the index compared to the covering index. Using the .print output that to the pow.txt. Mine was 99% decrease WOW!
- Now listen to Carter discuss the B-Tree structure for creating indexes, the associated "cost" and searching algorithm. Then create a README.md add a heading and summary your understanding of concepts covered.  
    - **COMMIT MESSAGE - "how indexes are created and used"**

## Time Mark 49:05 to 59:47
- Now add sub heading for partial index and add your understanding of the how and why of this concept.
- Then code along to code the partial index and see how much faster the query for 2023 was compared to 1998.
- Output the .schema to the pow.txt
- Now add a heading for Vacuum and listen and then write your understanding of this concept and then give the linux command a try.  Heads up if you are running locally you may not have this command - ``du -b movies.db``. Very interesting, my size was different than what Carter's output was. It is good to run this if you are using codespace because it will make the db file size smaller.  Remember this is not an sqlite3 shell command, so you would run it in bash. 
        - **COMMIT MESSAGE - "partial indexes and vacuum"**

## Time Mark 59:47 tp 1:15:51
- Now add a sub heading for concurrency and write your understanding of this concept.
- Now add a sub heading for ACID and write your understanding of this concept. SO IMPORTANT TO UNDERSTAND each of part of ACID.
- In the optimizing folder get the bank.db
    - ```curl -o bank.db https://raw.githubusercontent.com/CIT28/files/main/w16/bank.db```
- Then code along with Carter to code the UPDATE, make sure to not run the UPDATE twice. I did get an runtime error, because of the constraint, but it take the balance to 0 for Alice. 
- Code the UPDATE to give back the money, you can just update the previous query.  
- Now code the transaction do as Carter does by opening another shell and check the account table to see the changes (or not) 
- Now write the UPDATES and then write the TRANSACTION with the ROLLBACK. 
        - **COMMIT MESSAGE - "concurrency,ACID, transactions "**

## Race Conditions and Locks are optional, but recommended to add your db knowledge base

## Grading
-This is how I will grade your work:
1. Did you provide the correct commit history URL for the optimizing (all lowercase) folder = 5 points
2. Did you do all the commits required for this work = 15 points
3. Did you have all the queries in the q.sql file = 30 points 
4. Did you create the pow.txt include all the required output = 20 points
5. Did you include all the required content in the README.md file = 30 points
6. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 

