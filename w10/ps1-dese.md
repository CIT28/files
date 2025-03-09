# CS50 Problem Set 1 DESE 
## Department of Elementary and Secondary Education

## Week 10 Attendance 

### Setup
- Inside the folder ps1 folder, make sure it is at the same level as packages create another folder named dese.
-  Change the current folder to dese, then use the following command to copy the database file:
    - ```curl -o dese.db https://raw.githubusercontent.com/CIT28/files/main/w10/dese.db```
    - Create a new query file (dese-q.sql) by copying a previous sql file we have used. Remove any queries in the file and update bash command and pow reference to be pow-ds.txt.
    - Do the normal new dataset queries:
        1. .table
        2. .schema
        3. Code a query for listing the first 10 records of each table
        - **COMMIT MESSAGE - "new dataset"**

### Week 10 Attendance Code Along - Query 1
-  Create a new query file (dese-q.sql) by copying a previous sql file we have used. Remove any queries in the file and update bash command and pow reference to be pow-dese.txt.
    - Create the poe file (README.md) and a heading 1 for DESE query 1 thru 6
    - Then for create a heading 2 md for each query
    - Code along with me and once you have the query tne and you see how I want the pow to be completed. 
        - **COMMIT MESSAGE - "query 1"**  


### Query 2 thru 6
- For each query, you need to:
1. Write the query in the dese-q.sql file and make sure you get the correct output (see below) 
2. In the README.md, authenticate your work by describing how you answered you approached the question, do this under the heading for each question.  
3. Open another terminal session to change the standard output to sent the output to powp2.txt, commit with message:
  - **COMMIT MESSAGE - "1. query, pow  and README.md complete"**
  - Comment out the current query and then work on next query and use the same commit message, just updating the number (ex. "2. query, pow  and README.md complete")

  
# Specification
For each of the following questions, you should write a single SQL query that outputs the results specified by each problem. Your response must take the form of a single SQL query. You should not assume anything about the ids of any particular rows: your queries should be accurate even if the ids were different. Finally, each query should return only the data necessary to answer the question.

1. Your colleague is preparing a map of all public schools in Massachusetts. Write a SQL query to find the names and cities of all public schools in Massachusetts.

    - Keep in mind that not all schools in the schools table are considered traditional public schools. Massachusetts also recognizes charter schools, which (according to DESE!) are considered distinct.

    - Results in a table with 2 columns and 1,761 rows.


2. Your team is working on archiving old data. Write a SQL query to find the names of districts that are no longer operational.

    - Districts that are no longer operational have “(non-op)” at the end of their name.

    - Results in a table with 1 column and 121 rows.

3. The Massachusetts Legislature would like to learn how much money, on average, districts spent per-pupil last year. Write a SQL query to find the average per-pupil expenditure. Name the column “Average District Per-Pupil Expenditure”.

    - Note the per_pupil_expenditure column in the expenditures table contains the average amount, per pupil, each district spent last year. You’ve been asked to find the average of this set of averages, weighting all districts equally regardless of their size.

    - Results in a table with 1 column and 1 row.

4. Some cities have more public schools than others. Write a SQL query to find the 10 cities with the most public schools. Your query should return the names of the cities and the number of public schools within them, ordered from greatest number of public schools to least. If two cities have the same number of public schools, order them alphabetically.

    - Results in a table with 2 columns and 10 rows.

5. DESE would like me to determine in what cities additional public schools might be needed. Help me to problem solve who to find cities with 3 or fewer public schools. My query should return the names of the cities and the number of public schools within them, ordered from greatest number of public schools to least. If two cities have the same number of public schools, order them alphabetically.
    - Results in a table with 2 columns and 201 rows.

6. DESE wants to assess which schools achieved a 100% graduation rate. Write a SQL query to find the names of schools (public or charter!) that reported a 100% graduation rate.

    - Results in a table with 1 column and 9 rows.

## Grading
- Submit your commit history URL your normals in your private repo for grading
- This is how I will grade your work:
    1. Did you provide the correct URL for DESE folder commits = 5 points.
    2. Did you do all the commits required for this work = 65 points
        -  There should be 8 commits, proof of work and authenitcate work in README.md
    3. Did your README.md file show authenicate work =  30 points
    4. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 