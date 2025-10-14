# CS50 Problem Set 1 Moneyball
## 1 thru 5

## Setup
- Inside the folder ps1 folder, make sure it is at the same level as packages and dese, there create another folder named moneyball.
- 
```
ps1/
   /packages
   /dese
   /moneyball
```   

-  Change the current folder to moneyball, then use the following command to copy the database file:
    - ```curl -o moneyball.db https://raw.githubusercontent.com/CIT28/files/main/w11/moneyball.db```
  - Create a new query file (ds-q.sql) by copying a previous sql file we have used. Remove any queries in the file and update bash command and pow reference to be pow-ds.txt.
    - Do the normal new dataset queries:
        1. .table
        2. .schema
        3. Code a query for listing the first 10 records of each table
    -  Create a new query file (mball-q.sql) by copying a previous sql file we have used. Remove any queries in the file and update bash command and pow reference to be pow-mb.txt.
    - Create a new poe file (README.md) and have a heading 1 md for each problem 1 thru 5.
        - **COMMIT MESSAGE - "setup for moneyball complete"**

### Follow instructions in Week 11 Attendance

### For each problem you need to do the following 

- For each query, you need to:
    - Use the poe file to show your attempts and thinking progress
    - Write the query in the mball-q.sql file and make sure you get the correct output (see below)
    - Use .print to identify each query and related count
    - Once you have the correct output, run the pow and include both query output and count (like we did in week 10)
        - **COMMIT MESSAGE - "1. query, poe, pow complete"** 
    - Comment out the current query and then work on next query and use the same commit message, just updating the number (ex. "2. query, poe, pow complete")

## BREAK OPTIONAL  
- If you get query 1, 2 and 3 done than you can take a break and complete the rest of this work by the Thursday night deadline.
- To "GET" this break you will submit your commit history for the packages folder now.
- I will do a review and give you feedback.
- If you complete before Thurs morning, then you can submit again your commit history URL and tell me that you are ready for a second review. 


# Specification
https://cs50.harvard.edu/sql/2024/psets/1/moneyball

- For each of the following questions, you should write a single SQL query that outputs the results specified by each problem. Your response must take the form of a single SQL query. You should not assume anything about the ids of any particular rows: your queries should be accurate even if the ids were different. Finally, each query should return only the data necessary to answer the question.

1. You should start by getting a sense for how average player salaries have changed over time. Write a SQL query to find the average player salary by year.

  - Sort by year in descending order.
  - Round the salary to two decimal places and call the column “average salary”.
  - Your query should return a table with two columns, one for year and one for average salary.
  - Results in a table with 2 columns and 17 rows.

2. Your general manager (i.e., the person who makes decisions about player contracts) asks you whether the team should trade a current player for Cal Ripken Jr., a star player who’s likely nearing his retirement. Write a SQL query to find Cal Ripken Jr.’s salary history.

  - Sort by year in descending order.
  - Your query should return a table with two columns, one for year and one for salary.
  - Results in a table with 2 columns and 17 rows.

3. Your team is going to need a great home run hitter. Ken Griffey Jr., a long-time Silver Slugger and Gold Glove award winner, might be a good prospect. In 3.sql, write a SQL query to find Ken Griffey Jr.’s home run history.

  - Sort by year in descending order.
  - Note that there may be two players with the name “Ken Griffey.” This Ken Griffey was born in 1969.
  - Your query should return a table with two columns, one for year and one for home runs.
  - Results in a table with 2 columns and 13 rows.

4. You need to make a recommendation about which players the team should consider hiring. With the team’s dwindling budget, the general manager wants to know which players were paid the lowest salaries in 2001. Write a SQL query to find the 50 players paid the least in 2001.

  - Sort players by salary, lowest to highest.
  - If two players have the same salary, sort alphabetically by first name and then by last name.
  - If two players have the same first and last name, sort by player ID.
  - Your query should return three columns, one for players’ first names, one for their last names, and one for their salaries.
  - Results in a table with 3 columns and 50 rows.

5. It’s a bit of a slow day in the office. Though Satchel no longer plays, write a SQL query to find all teams that Satchel Paige played for.

  - Your query should return a table with a single column, one for the name of the teams.
  - Executing results in a table with 1 column and 3 rows.

## Grading
- Submit your commit history URL the moneyball folder in your private repo for grading

This is how I will grade your work:
1. Did you provide the correct URL for moneyball folder commits = 5 points.
2. Did you do all the commits required for this work = 20 points
3. Did your poe show authenticate work =  45 points
4. Did you get the correct output each query and include second query with the count result = 30 points
- Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 