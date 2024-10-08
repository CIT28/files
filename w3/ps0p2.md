# CS50 Problem Set 0 Part 1 
## Cyberchase 8 thru 13

## Setup
- You will use the same folder ps0 that we used in part 1.
- Create a file to store the queries name it p2-q.sql and then the README.md with a heading for each problem 8 thru 7, commit with message:
      - **COMMIT MESSAGE - "setup complete"**

### For each problem you need to do the following
- For each problem, you need to:
1. Write the query in the p2-q.sql file and make sure you get the correct output (see below) 
2. In the README.md, authenicate your work by copying the steps you took to get the correct output, do this under the heading for each problem.    
3. Open another terminal session to change the standard output to sent the output to powp2.txt, commit with message:
  - **COMMIT MESSAGE - "8. query, pow and README.md complete"**
  - Comment out the current query and then work on next query and use the same commit message, just updating the number (ex. "9. query, pow and README.md")


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

8. Write a query that counts the number of episodes released in the last 6 years, from 2018 to 2023, inclusive.
  - You might find it helpful to know you can use BETWEEN with dates, such as BETWEEN '2000-01-01' AND '2000-12-31'.
9. Write a query that counts the number of episodes released in Cyberchase’s first 6 years, from 2002 to 2007, inclusive.
10. Write a SQL query to list the ids, titles, and production codes of all episodes. Order the results by production code,   from earliest to latest.
11. List the titles of episodes from season 5, in reverse alphabetical order.
12. Count the number of unique episode titles.
13. Write a SQL query to explore a question of your choice. This query should:
 - Involve at least one condition, using WHERE with AND or OR


## How to Test
- Executing 8.sql results in a table with 1 column and 1 row.
- Executing 9.sql results in a table with 1 column and 1 row.
- Executing 10.sql results in a table with 3 columns and 140 rows.
- Executing 11.sql results in a table with 1 column and 10 rows.
- Executing 12.sql results in a table with 1 column and 1 row.


## Grading
- Submit your commit history URL your cyberchase in your private repo for grading
- This is how I will grade your work:
  1. Did you provide the correct URL for cyberchase folder = 5 points.
  2. Did you do all the commits required for this work = 65 points
      -  There should be 7 commits, 1 for the setup and 6 that show the current query (uncommented), proof of work and autenciate work in README.md
  3. Did your README.md file show authenicate work =  30 points
  4. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 
