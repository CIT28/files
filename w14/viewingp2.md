# CS50 Viewing Part 2
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 2 - Viewing](https://www.youtube.com/watch?v=jZwGVuA8PMI)

## Setup
-   In the README.md file add a heading Viewing Part 2
-   Rename view.sql to view-p1.sql and create a new file view-p2.sql.  
    - **COMMIT MESSAGE - "part 2 setup done"**

### Time mark 52.57 to ?
-   Add a sub heading Viewing Part 2 and then add another sub heading for Security and write about how we can use views for securing data.
-   In the viewing folder download the rideshare database file ```curl -o rideshare.db https://raw.githubusercontent.com/CIT28/files/main/w14/rideshare.db```
-   Code along with Carter and write queries and create the view, then output the .schema and the query output to pow2.txt
-   Code the question, and your notes discuss the downside of sqlite here.
    - **COMMIT MESSAGE - "kinda securing views"**

- Pick it back up at 1:00:18 and add a sub heading for Soft Deletes and take a few notes here.
- Here is the mfa schema file should be in your writing folder, but if you need to create it again here the content for that [schema](../w11/writingp1.md#MFA2).
- Now code along and create a temporary view and once you are done, output the .schema and the query to pow1.txt. 
- Carter gives a really good overview of the differnce between the 2 methods here.  So review your content in the first point and update it if needed to help you clarify the different use cases.

    - **COMMIT MESSAGE - "TEMPORARY VIEWs"**

- Pick it back pat 39:09 and add a sub heading for "CTE - Common Table Expression" and write your understanding of this concept. 
- Now code along with Carter DROP the VIEW we created on the previous step and code the CTE.  Once you have the correct output, update your pow1.txt and commit:

    - **COMMIT MESSAGE - "Creating view with CTE"**

- Start back at 44:38 and add a sub heading for "Partitioning" and write your understanding of this concept. 
- Then code along and in your notes tell me why is it might be important to have naming standards?
- Once you have both the partitioned 2022 and 2021 output them to the pow2.txt. 
- Listen to the questions and code along see why you can't update the view output the message to the pow1.txt, then commit with message:
    - **COMMIT MESSAGE - "Partitioning VIEW"**

- Start back at 1:00:22 and add a sub heading for Triggers with Views and subheading under that for Soft Delete and take a few notes to review the concepts.
- Interesting note: I wondered by Carter output of the simple show all query had NULL values showing up, so I did a little investigating and found you can do this in addition to .mode box to get this output: ```.nullvalue NULL```. Give it a try!  
- Once you create the new view then update the pow2.txt with the schema and the query output for current collections.
- Now code the query that we know will not work and then listen to the question.
- Continue and code the trigger and once you are done update your pow2.txt.
- At 1:13 commit with message:
    - **COMMIT MESSAGE - "TRIGGERS and soft deletes"**

- Start back and add a sub heading for Triggers, Views and adding data and take a new notes on how this will work. 
- Continue to code along to code this trigger, once it works then update the pow2.txt with the contents of the "collection" table data and mfa schema.
    - **COMMIT MESSAGE - "TRIGGERS and adding data"**

## Grading
-This is how I will grade your work:
1. Did you provide the correct commit history URL for the viewing (all lowercase) folder = 5 points
2. Did you do all the commits required for this work = 15 points
3. Did you have all the queries in the view-p2.sql file = 30 points
    - make sure you not include notes in your sql file. 
    - I counted 12 queries in my view-p2.sql
4. Did you create the powp2.txt include all the required output = 20 points
5. Did you include all the required content in the README.md file = 30 points
6. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 


