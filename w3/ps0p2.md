# CS50 Problem Set 0 Part 1 
## Cyberchase 8 thru 13

## Setup

In the video I will walk how to complete this work:
### Create Proof of Work and SQL Files for Each Problem
- You will use the same folder ps0 that we used in part 1.
- For each problem, you need to create:
  1. A proof of work file (e.g., pow8.txt) containing the required output.
  2. An SQL file named after each problem (e.g., 8.sql) that generates the output.
 
### Test Your SQL File
- Before committing your changes, test your SQL file by running the following commands in the sqlite3 command line:
    - ```sqlite3 cyberchase.db```
    - ```.read 8.sql```
    - Verify that the output is correct and matches the contents of your proof of work file.
- Then commit after each one with this message:
- ex. **COMMIT MESSAGE - "terminal output, pow8 .txt and 8.sql complete"**


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

8. In 8.sql, write a query that counts the number of episodes released in the last 6 years, from 2018 to 2023, inclusive.
  - You might find it helpful to know you can use BETWEEN with dates, such as BETWEEN '2000-01-01' AND '2000-12-31'.
9. In 9.sql, write a query that counts the number of episodes released in Cyberchase’s first 6 years, from 2002 to 2007, inclusive.
10. In 10.sql, write a SQL query to list the ids, titles, and production codes of all episodes. Order the results by production code,   from earliest to latest.
11. In 11.sql, list the titles of episodes from season 5, in reverse alphabetical order.
12. In 12.sql, count the number of unique episode titles.
13. In 13.sql, write a SQL query to explore a question of your choice. This query should:
 - Involve at least one condition, using WHERE with AND or OR


## How to Test
- Executing 8.sql results in a table with 1 column and 1 row.
- Executing 9.sql results in a table with 1 column and 1 row.
- Executing 10.sql results in a table with 3 columns and 140 rows.
- Executing 11.sql results in a table with 1 column and 10 rows.
- Executing 12.sql results in a table with 1 column and 1 row.


## Grading
- Submit your commit history URL your ps0 in your private repo for grading
- This is how I will grade your work:
1. Did you provide the correct URL for ps0 folder - 15 points.
2. Did you do all the commits required for this work - 25 points - There should be 6 commits, 6 sql files and 6 pow.txt files.
3. Did your SQL files create the correct output - 40 points
4. Did you proof of work files show autheicate work - 20 ppoints
