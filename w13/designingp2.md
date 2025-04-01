## CS50 Designing Part 2
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 1 - Designing](https://www.youtube.com/watch?v=QzRW6bfv3Fo)

### Markdown legend
- Heading
    - h1 ```#```
    - h2 ```##```
- Outline
    - ```*```
    - ```-```

## Setup
- We will continue working in the designing folder, so create your p2-q.sql by copying a previous query, remove any queries update bash command and pow-p2.txt. 
- Add md h1 README.md 'Designing Part 2'


## Tidemark 53:35

- Start watching 53:35 add md h2 'Column Constraints' and take notes for each one using outline md syntax. 
- Before you start coding run the DROP TABLE by coping it from the p2-d.sql or run them on the terminal to remove the previous tables. 
- Then copy the last queries from the p1-d.sql into the schema before starting to code the column constraints with Carter. 
- Add md h2 'Constraints primary key and foreign key" and take notes on this concept.
- Make sure to listen to the question(s).
- At 1:00:19 run the sql and fix any error you have, then output the ```.schema``` to pow-p2.txt and ``.print 'column constrains example'
     - **COMMIT MESSAGE - "column constraints"**

- Watch and learn about to ALTER the schema for CharlieCard concept into the schema. 
- Before we start coding along I noticed that Carter was using a previous version of the schema queries, therefore make sure you have that before you coding along. 
- Here are the steps you need to take to get this setup:
    1. Drop the existing tables with DROP TABLE
    2. Copy this into the p2-q.sql:
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
    3. Run the queries
    4. Comment out this code and write the ALTER sql commands in your p2-q.sql and comment out after each one that has been run.

- Now at 1:03:54 code along to DROP TABLE the riders table, notice Carter is doing this command in the terminal and not in the file. Because I want us to have a reference you will be doing this work in your schema.sql file. 
- Add md h2 'Altering Tables' and list the different technique. 
- Include the mistakes and related SQL for a total of 5 queries. 
- Output the .schema to your pow-p2.txt.
- Then write the sql to DROP all the tables, run the sql and then uncomment the p2-q.sql to match Carter, and commit message
     - **COMMIT MESSAGE - "ALTER tables"**

- Before you start coding along you will to bring back the schema to match what Carter is using.  
- Now code along and then listen to the questions and note them. 
- Carter will discuss the different techniques we have learned and now implemented into this schema, so in your notes add md h 'Summary' and write how we use the different techniques we learned, either in paragraph or bullet form. 
- Now run SQL and make sure you don't have any syntax issues and run ```.schema``` and complete the pow and the commit with message: 
    - **COMMIT MESSAGE - "updating schema"**

## Grading
This is how I will grade your work:
1. Did you provide the correct commit history URL for designing folder = 10 points
2. Did you do all the commits required for this work = 20 points
3. Did you have all the queries in the p2-q.sql file = 25 points
4. Did you create the pow-p1.txt file correctly and include all the required output = 20 points
5. Did you include all the required content in the README.md file = 30 points
- Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 