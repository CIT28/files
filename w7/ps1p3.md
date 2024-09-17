# CS50 Problem Set 1 Part 3
## Moneyball 
## 1 thru 5

## Code along OR new level for authenticate
- I will have covered the different paths available to students in this week's attendance video.

### Setup (same for both)
- Inside the folder ps1 folder, make sure it is at the same level as packages create another folder named moneyball.
-  Change the current folder to dese, then use the following command to copy the database file:
    - ```curl -o moneyball.db https://raw.githubusercontent.com/CIT28/files/main/w7/moneyball.db```
    - Create a file to store the queries name it p3-q.sql and a README.md include heading "Moneyball 1 thru 5" and commit with message:
        - **COMMIT MESSAGE - "setup complete"**

### For each problem you need to do the following (Authenticate)
- For each problem, you need to:
1. Write the query in the p3-q.sql file and make sure you get the correct output (see below) 
2. In the README.md, authenticate your work by describing how you answered you approached the question, do this under the heading for each question.  
3. Open another terminal session to change the standard output to sent the output to powp1.txt, commit with message:
  - **COMMIT MESSAGE - "1. query, pow  and README.md complete"**
  - Comment out the current query and then work on next query and use the same commit message, just updating the number (ex. "2. query, pow  and README.md complete")

### For each problem you need to do the following (Code Along)
- For each problem, you need to:
1. Write the query in the p3-q.sql file code along with each video, I'll provide a list below.
2. In the README.md, make sure include any required answer and/or comment I cover in the video and make sure you complete the required commits. 
3. Open another terminal session to change the standard output to sent the output to powp3.txt, commit with message:
  - **COMMIT MESSAGE - "query 1 step ?"** and whatever message I show in the video. 
  - Comment out the current query and then work on next query and use the same commit message, just updating the number (ex. "2. query step ? ")
  - Make sure you right click and open in a new tab or window. 

    1. https://youtu.be/MRjYZOrz3zk
    2. https://youtu.be/3XsD1HTh8d0
    3. https://youtu.be/iUpyZUATYUI
    4. https://youtu.be/pY6rUZ1UF0Q
    5. https://youtu.be/iy2fF0HzQZg
    6. https://youtu.be/WrIA1_iaZIk
    7. https://youtu.be/Kxt4jVeS57I
    8. https://youtu.be/pPLuMETZ6rE
    9. https://youtu.be/Ay6XTWD7u-0
    10. ?


# Specification
For each of the following questions, you should write a single SQL query that outputs the results specified by each problem. Your response must take the form of a single SQL query. You should not assume anything about the ids of any particular rows: your queries should be accurate even if the ids were different. Finally, each query should return only the data necessary to answer the question.

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

5. It’s a bit of a slow day in the office. Though Satchel no longer plays, in 5.sql, write a SQL query to find all teams that Satchel Paige played for.

  - Your query should return a table with a single column, one for the name of the teams.

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