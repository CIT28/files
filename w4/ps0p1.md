# CS50 Problem Set 0 - Part 1
## Cyberchase - Problems 1 thru 7
- https://cs50.harvard.edu/sql/2024/psets/0/cyberchase/

## Setup
- Create a new sql file named p1-q.sql and copy the a-q.sql and remove previous queries and update for new sql filename. 
- In the README.md create a new heading 1 md with text
    - Problem set 0 - Problems 1 thru 7 
- Start the normal terminal sessions

### For each problem you need to do the following
1. Add heading 2 md text for each problem with the following text
    - 'Problem #'
    - add the backticks 
2. Use the SQLITE3 terminal to write your SQL commands to solve the problem. 
    - If you get help from the CS50 AI Duck or other gen ai sources, note this with the ```.print 'what you did to get help'``` in your README.md for this problem
3. Once you have solved with the correct output (see below for test) comoplete the poe workflow. 
    - Refer back to Week 4 Attendance instructions for how to complete the poe workflow.
5. Clear the sqlite terminal with ```.shell clear``` 
    - DON'T DO THIS UNTIL you have copied the effort (SQL commands) you did to get the correct output.
6. Complete the pow and git workflow, commit with message:
        - **COMMIT MESSAGE - "Prob 1 complete"**

**CONTENT FROM CS50 SITE STARTS HERE**

## Schema
Each database has some “schema” 
The tables and columns into which the data is organized. In cyberchase.db you’ll find a single table, episodes. In the episodes table, you’ll find the following columns:

- id, which uniquely identifies each row (episode) in the table
- season, which is the season number in which the episode aired
- episode_in_season, which is the episode’s number within its given season
- title, which is the episode’s title
- topic, which identifies the ideas the episode aimed to teach
- air_date, which is the date (expressed as YYYY-MM-DD) on which the episode “aired” (i.e., was published)
- production_code, which is the unique ID used by PBS to refer to each episode internally

## Specification

For each of the following questions, you should write a single SQL query that outputs the results specified by each problem. Your response must take the form of a single SQL query. You should not assume anything about the ids of any particular episodes: your queries should be accurate even if the id of any particular episode were different. Finally, each query should return only the data necessary to answer the question: if the problem only asks you to output the names of episodes, for example, then your query should not also output each episodes’s air date.

Make sure you commit before moving on to the next problem. 

1. Write a SQL query to list the titles of all episodes in Cyberchase’s original season, Season 1. 
2. List the season number of, and title of, the first episode of every season.
3. Find the production code for the episode “Hackerized!”.
4. Write a query to find the titles of episodes that do not yet have a listed topic.
5. Find the title of the holiday episode that aired on December 31st, 2004.
6. List the titles of episodes from season 6 (2008) that were released early, in 2007.
7. Write a SQL query to list the titles and topics of all episodes teaching fractions.


## How to Test
- Executing 1. results in a table with 1 column and 26 rows.
- Executing 2. results in a table with 2 columns and 14 rows.
- Executing 3. results in a table with 1 column and 1 row.
- Executing 4. results in a table with 1 column and 26 rows.
- Executing 5. results in a table with 1 column and 1 row.
- Executing 6. results in a table with 1 column and 2 rows.
- Executing 7. results in a table with 2 columns and 6 rows.

**CONTENT FROM CS50 SITE END HERE**

## OPTIONAL BREAK!
- If you've completed problems 1 through 3, you can submit your commit history for the cyberchase folder and continue with steps 4 through 7 by the next due date. Be sure to include a commit message indicating that you're taking a break. If you finish early and would like to review your work, let me know in your submission comments.


## Grading
- Submit your commit history URL your cyberchase in your private repo for grading
- This is how I will grade your work:
1. Did you provide the correct URL for cyberchase folder = 10 points.
2. Did you do all the commits required for this work = 30 points
3. Did the commits contain the workflow (poe, pow and git ) data =  60 points
4. Work submitted after the due date will be reduced by 25 points. 