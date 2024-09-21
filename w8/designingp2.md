## CS50 Designing Part 2
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 1 - Designing](https://www.youtube.com/watch?v=QzRW6bfv3Fo)

## Setup
-- We will continue working in the schema.sql file for this work, before we start copy the queries into a new file named p1-d.sql.  

## Timemark 53:35

- Start watching 53:35 and in your notes add a sub heading for Column Contraints and take notes on each one. 
- Before you start coding run the DROP TABLE by coping it from the p1-d.sql or run them on the terminal to remove the previous pages. 
- Then copy the last queries from the p1-d.sql into the schema before starting to code the column contraints with Carter. 
- What contraints apply to primary key and foriegn key.
- Make sure to listen to the question(s).
- at 1:00:19 make sure you syntax is good by  ```.read schema.sql``` and fix any error you have, then output the ```.schema``` to powp2.txt. 
     - **COMMIT MESSAGE - "column constraints"**

- Watch and learn about to alter the schema for CharlieCard concept into the schema. 
- Before we start coding along I noticed that Carter was using a previous version of the schema queries, therefore make sure you have that before you coding along. 
- Here are the steps you need to take to get this setup:
    1. Drop the existing tables (.schema then DROP TABLE)
    2. Comment out previous queries in the schema.sql file and copy this into that file:
    ```
        CREATE TABLE "riders" (
            "id" INTEGER,
            "name" TEXT
        );

        CREATE TABLE "stations" (
            "id" INTEGER,
            "name" TEXT,
            "line" TEXT
        );

        CREATE TABLE "visits" (
            "rider_id" INTEGER,
            "station_id" INTEGER
        );
    ```
    3. ```.read schema.sql```
    4. Comment out this code and write the alter sql commands in your schema.sql and comment out after each one as been run. 
- Now at 1:03:54 code along to DROP TABLE the riders table, notice Carter is doing this command in the terminal and not in the file. Because I want us to have a reference you will be doing this work in your schema.sql file. 
- In your notes add a sub heading for Alterning Tables and list the different technique. 
- Include the mistakens and related SQL for a total of 5 queries. 
- Output the .schema to your powp2.txt.
- Then DROP all the tables (terminal or sql file) and uncomment the schema.sql to match what Carter, and commit message
     - **COMMIT MESSAGE - "altering tables"**

- Before you start coding along you will to bring back the schema to match what Carter is using.  It in your sql file, so find it and uncomment it. 
- Now code along and update the schema.sql and then listen to the questions. 
- Carter will discuss the different techniques we have learned and now implemented into this schema, so in your notes add a sub heading Summary and write how we using the different techniques we learned, either in paragraph or bullet form. 
- Now run your query file and make sure you don't have any syntax issues and then .schema to the proof of work file and the commit with message: 
    - **COMMIT MESSAGE - "updating schema"**

## Grading
- This is how I will grade your work:
    1. Did you provide the correct commit history URL for the designing folder = 5 points
    2. Did you do all the commits required for this work = 20 points
    3. Did you have all the queries in the schema.sql file and did your queries run = 25 points
        - make sure you not include notes in your sql file. 
        - you should also have a ps1p4.sql file as well
    4. Did you create the powp2.txt include all the required output = 20 points
    5. Did you include all the required content in the README.md file and comoplete the ICA = 30 points
    6. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 
