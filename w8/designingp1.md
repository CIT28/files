## CS50 Designing Part 1
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 1 - Designing](https://www.youtube.com/watch?v=QzRW6bfv3Fo)

## Setup
- The video will cover the setup for this week, you do need to create a new sql file named schema.sql and also have a pow terminal ready. 

## Timemark 20:16

- Start watching 20:16, first create the new database mbta.db as shown in the video. ```sqlite3 mbta.db```, unlike what happens when Carter does the command, I was not asked if I wanted to create a new database. 
- The new database file will not show up until you run the first CREATE TABLE query.  Once you run ```.read schema.sql```make SURE to comment out queries that have been run because they will create an error if you try to run them a second time. There will be 3 queries, therefore 3 tables. 
- At 27:02, open the terminal with your pow1.txt and run ```.schema```, then commit with message:
    - **COMMIT MESSAGE - "CREATE TABLE command"**

- At 27:35, take notes in your README.md file using a sub heading for Storage Classes and make notes on the different classes and note the difference between data type and storage classes. 
- Give a sub heading named "My Answer" and tell me do we need to specific data types in our schema?
- Now add a sub heading and have the examples and your understanding of the trade off that was discussed and/or do some additional research to add to your understanding.  
- Now add a sub heading for Type Affinites and take notes on this concept and how make sure cover how it differs from Storage Classes.  
- After watching the example of how type affinites work, come up with your own example and describe that in your notes.  
- At 37:52, commit with message:
    - **COMMIT MESSAGE - "data types, storage classes and type affinites notes"**

- At 38:10, code along and code the DROP TABLE in the schema.sql, make sure to comment out the CREATE TABLES before running the ```.read schema.sql``` to DROP (delete) the tables. 
You can copy the queries from before then update with new data affinites, but DO NOT remove previous queries and comment out the DROP TABLES so that you don't delete the tables your schema has created. 
- Nice that CS50 is now using query file!!
- Once you have new tables created output .schema to proof of work, and make sure to listen to the question.  
- In your notes tell me if you have heard of boolean and if not do some research to understand this term and update your notes with your new (or existing) understanding. 
- Your schema.sql should have 3 queries then at 45:43 commit with message:
    - **COMMIT MESSAGE - "DROP TABLE and type affinities"**

- At 45:14 add a subheading Table Constraints and take notes on this VERY important concept and make sure you describe how it works. (this might be easier to do once you have updated the schema.sql file) 
- Copy the CREATE TABLE queries from the previous step, uncomment them and then code along update as Carter does the table constraints. 
- Make sure to note your file the different type of constraints and include the SQL in your notes using the ```PRIMARY KEY``` different examples and explain them and note row id. 
 - Now code along with the FOREIGN KEY table constrains. 
 - Listen carefully to the questions.
 - Code along with the last question adding the visits id, then DROP TABLES that were created before and run the query file and output to the proof of work.
 - At 53:35 there should be 3 queries commits with message:
    - **COMMIT MESSAGE - "table constrains and schema update"**

## Grading
This is how I will grade your work:
    1. Did you provide the correct commit history URL for the designing folder = 5 points
    2. Did you do all the commits required for this work = 20 points
    3. Did you have all the queries in the schema.sql file = 25 points
        - make sure you not include notes in your sql file. 
    4. Did you create the powp1.txt include all the required output = 20 points
    4. Did you include all the required content in the README.md file = 30 points
    6. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 