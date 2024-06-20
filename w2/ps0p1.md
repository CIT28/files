# CS50 Problem Set 0 Part 1 
## Cyberchase 1 thru 7

## Setup
In the video I will walk how to complete this work
- Creata a few folder and name it ps0 (problem set 0) at the same level as w1 and w2.  
- Then make sure you pwd is in the ps0 folder and use this command to copy the database file. 
    - ```curl -o cyberchase.db https://raw.githubusercontent.com/CIT28/files/main/w2/cyberchoase.db```
- For each problem you need to show a proof of work file (etc pow1.txt). 
- Once you have the SLQ creating the output required, see How to Test below, then create your pow.txt file and then create a sql file named for each problem, etc 1.sql. 
- Make sure you sql file runs by doing the following command in the sqlite3 command line:
    - ```sqlite3 cyberchase.db```
    - ```.read 1.sql```
- Then commit after each one with this message:
- **COMMIT MESSAGE - "terminal output, pow1.txt and 1.sql complete"**




## Schema
Each database has some “schema” 

the tables and columns into which the data is organized. In cyberchase.db you’ll find a single table, episodes. In the episodes table, you’ll find the following columns:

- id, which uniquely identifies each row (episode) in the table
- season, which is the season number in which the episode aired
- episode_in_season, which is the episode’s number within its given season
- title, which is the episode’s title
- topic, which identifies the ideas the episode aimed to teach
- air_date, which is the date (expressed as YYYY-MM-DD) on which the episode “aired” (i.e., was published)
- production_code, which is the unique ID used by PBS to refer to each episode internally

# Specification

For each of the following questions, you should write a single SQL query that outputs the results specified by each problem. Your response must take the form of a single SQL query. You should not assume anything about the ids of any particular episodes: your queries should be accurate even if the id of any particular episode were different. Finally, each query should return only the data necessary to answer the question: if the problem only asks you to output the names of episodes, for example, then your query should not also output each episodes’s air date.

1. In 1.sql, write a SQL query to list the titles of all episodes in Cyberchase’s original season, Season 1.
2. In 2.sql, list the season number of, and title of, the first episode of every season.
3. In 3.sql, find the production code for the episode “Hackerized!”.
4. In 4.sql, write a query to find the titles of episodes that do not yet have a listed topic.
5. In 5.sql, find the title of the holiday episode that aired on December 31st, 2004.
6. In 6.sql, list the titles of episodes from season 6 (2008) that were released early, in 2007.
7. In 7.sql, write a SQL query to list the titles and topics of all episodes teaching fractions.

# How to Test
- Executing 1.sql results in a table with 1 column and 26 rows.
- Executing 2.sql results in a table with 2 columns and 14 rows.
- Executing 3.sql results in a table with 1 column and 1 row.
- Executing 4.sql results in a table with 1 column and 26 rows.
- Executing 5.sql results in a table with 1 column and 1 row.
- Executing 6.sql results in a table with 1 column and 2 rows.
- Executing 7.sql results in a table with 2 columns and 6 rows.