# CS50 Problem Set 1 Part 4
## Moneyball 
## 6 thru 10

## Code along OR new level for authenticate
- I will have covered the different paths available to students in this week's attendance video.

### Setup (same for both)
- Continue working in the ps1/moneyball folder.
    - Create a file to store the queries name it p4-q.sql and a README.md include heading "Moneyball 6 thru 10" and commit with message:
        - **COMMIT MESSAGE - "setup complete"**

### For each problem you need to do the following (Authenticate)
- For each problem, you need to:
1. Write the query in the p4-q.sql file and make sure you get the correct output (see below) 
2. In the README.md, authenticate your work by describing how you answered you approached the question, do this under the heading for each question.  
3. Open another terminal session to change the standard output to sent the output to powp4.txt, commit with message:
  - **COMMIT MESSAGE - "5. query, pow  and README.md complete"**
  - Comment out the current query and then work on next query and use the same commit message, just updating the number (ex. "6. query, pow and README.md complete")

### For each problem you need to do the following (Code Along)
- For each problem, you need to:
1. Write the query in the p4-q.sql file code along with each video, I'll provide a list below.
2. In the README.md, make sure include any required answer and/or comment I cover in the video and make sure you complete the required commits. 
3. Open another terminal session to change the standard output to sent the output to powp3.txt, commit with message:
  - **COMMIT MESSAGE - "query 5 step ?"** and whatever message I show in the video. 
  - Comment out the current query and then work on next query and use the same commit message, just updating the number (ex. "6. query step ? ")
  - Make sure you right click and open in a new tab or window. 

    6. https://youtu.be/WrIA1_iaZIk
    7. https://youtu.be/Kxt4jVeS57I
    8. https://youtu.be/pPLuMETZ6rE
    9. https://youtu.be/Ay6XTWD7u-0
    10. https://youtu.be/3ssyacYciWU


# Specification
https://cs50.harvard.edu/sql/2024/psets/1/moneyball/#schema

For each of the following questions, you should write a single SQL query that outputs the results specified by each problem. Your response must take the form of a single SQL query. You should not assume anything about the ids of any particular rows: your queries should be accurate even if the ids were different. Finally, each query should return only the data necessary to answer the question.

6. Which teams might be the biggest competition for the A’s this year? Write a SQL query to return the top 5 teams, sorted by the total number of hits by players in 2001.

    - Call the column representing total hits by players in 2001 “total hits”.
    - Sort by total hits, highest to lowest.
    - Your query should return two columns, one for the teams’ names and one for their total hits in 2001.
    - Results in a table with 2 columns and 5 rows.

7. You need to make a recommendation about which player (or players) to avoid recruiting. Write a SQL query to find the name of the player who’s been paid the highest salary, of all time, in Major League Baseball.

    - Your query should return a table with two columns, one for the player’s first name and one for their last name.
    - Results in a table with 2 columns and 1 row.

8. How much would the A’s need to pay to get the best home run hitter this past season? Write a SQL query to find the 2001 salary of the player who hit the most home runs in 2001.

    - Your query should return a table with one column, the salary of the player.
    - Results in a table with 1 column and 1 row.

9. What salaries are other teams paying? In 9.sql, write a SQL query to find the 5 lowest paying teams (by average salary) in 2001.

    - Round the average salary column to two decimal places and call it “average salary”.
    - Sort the teams by average salary, least to greatest.
    - Your query should return a table with two columns, one for the teams’ names and one for their average salary.
    - Results in a table with 2 columns and 5 rows.

10. The general manager has asked you for a report which details each player’s name, their salary for each year they’ve been playing, and their number of home runs for each year they’ve been playing. To be precise, the table should include:

    - All player’s first names
    - All player’s last names
    - All player’s salaries
    - All player’s home runs
    - The year in which the player was paid that salary and hit those home runs
    - Write a query to return just such a table.

    - Your query should return a table with five columns, per the above.
    - Order the results, first and foremost, by player’s IDs (least to greatest).
    - Order rows about the same player by year, in descending order.
    - Consider a corner case: suppose a player has multiple salaries or performances for a given year. Order them first by number of home runs, in descending order, followed by salary, in descending order.
    - Be careful to ensure that, for a single row, the salary’s year and the performance’s year match.
    See cs50 website for table example
    - Executing results in a table with 5 columns and 14,915 rows.

## Grading
- Submit your commit history URL your normals in your private repo for grading
- This is how I will grade your work:
    1. Did you provide the correct URL for moneyball folder commits = 5 points.
    2. Did you do all the commits required for this work = 65 points
        - Authenicate: There should be 6 commits, proof of work and authenitcate work in README.md
        - Code along: Make sure you do all the commits covered in the video for each query. 
    3. Depending on which path you take here is how this will be grade:
        - Authenicate: Did your README.md file show authenticate work = 30 points
        - Code Along: Did your README.md gave required content and correct commits = 30 points
    4. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 