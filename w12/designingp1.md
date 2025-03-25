## CS50 Designing Part 1
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 1 - Designing](https://www.youtube.com/watch?v=QzRW6bfv3Fo)

### Markdown legend
- Heading
    - h1 ```#```
    - h2 ```##```
- Outline
    - ```*```
    - ```-```
## Complete for Week 12 attendance

### 1. Attendance Code along 
- Create a new folder ```designing``` at the same level as querying and relating.
- In ```designing``` create a new file ```README.md``` and create new query file named w12-q.sql and copy previous query file and update for pow of pow-a.txt and update the bash command for w12-q.sql query file.
    - **COMMIT MESSAGE - "w12 setup done"**
- Code along with me to see how the SQL we are going to write this week will be different!
    - **COMMIT MESSAGE - "coding along done"**

### 2. Take notes from Beginning to 20:16
- In your README.md, add md h1 w/ text:
    - 'Designing Part 1'
- Add md h2 w/ text:
    - 'Overview'
    - 'MTBA'
    - 'Normalization'
- Then watch and take notes for each section, as part of grading I will review your notes.
- At 20:16 commit with message:
    - **COMMIT MESSAGE - "intro to designing"**
- Follow instructions in canvas 

### 20:16 to 27:02 CREATE TABLE

- Create a new query file p1-q.sql by copying a previous query, remove any queries update bash command and pow-p1.txt.
- Start watching 20:16, first create the new database mbta.db. 
    - In the ```designing``` folder using bash ```sqlite3 mbta.db```
    - I was not asked if I wanted to create a new database. 
    - The new database file will not show up until you run the first ```CREATE TABLE``` query.  
- Write the first query and run it, then make SURE to comment out the following queries. There will be 3 queries, therefore 3 tables. 
- At 27:02, comment out the last query and have the ```.schema``` in p1-sql, complete the pow and git workflows commit with message:
    - **COMMIT MESSAGE - "CREATE TABLE"**


## 27:02 to 37:52 Data Types and Storage Classes
- At 27:35, in your README.md file using md h2 for 'Storage Classes' takes notes on the different classes and note the difference between data type and storage classes. 
- Add md h2 'My Answer' and tell me do we need to specific data types in our schema?
- Add md h2 'Examples and Understanding' and have the examples and your understanding of the trade off that was discussed and/or do some additional research to add to your understanding.  
- Add md h2 'Type Affinities' and take notes on this concept, cover how it differs from Storage Classes.  
- Add md h2 'For Example', after watching the example of how type affinities work, come up with your own example and describe that in your notes.  
- At 37:52, commit with message:
    - **COMMIT MESSAGE - "data types and storage classes notes"**

## BREAK OPTIONAL  
- If you got this far you can take a break and complete the rest of this work by the Thursday night deadline.  
- To "GET" this break you will submit your commit history for the designing folder now.
- I will do a review and give you feedback.
- If you complete before Thurs morning, then you can submit again your commit history URL and tell me that you are ready for a second review. 

## 38:10 to 53:35 Table Constrains
- At 38:10, code along and code the ```DROP TABLE``` in the p1-q.sql, make sure to comment out the CREATE TABLES before running the to ``DROP (delete) the tables. 
- You can copy the queries from before then update with new data affinities, but DO NOT remove previous queries and comment out the ``1DROP TABLES``` so that you don't delete the tables in the schema. 
- Carter is doing showing the ```.read schema.sql```, I think I'll talk about this next week.  
- Once you have new tables created comment out queries and uncomment or include ```.schema``` then run pow workflow, and make sure to listen to the question.  
- In README.md tell me if you have heard of boolean and if not do some research to understand this term and update your notes with your new (or existing) understanding. 
- Your p1-q.sql will have 3 queries for this section then at 45:43 complete git workflow:
    - **COMMIT MESSAGE - "DROP TABLE and type affinities"**

- At 45:14 Add md h2 'Table Constraints' and take notes on this VERY important concept and make sure you describe how it works. (this might be easier to do once you have updated the p1-q.sql file) 
- Copy the CREATE TABLE queries from the previous step, uncomment them and then code along update as Carter does the table constraints. 
- Make sure to note in the README.md file the different type of constraints and include the SQL in your notes using the ```PRIMARY KEY``` different examples and explain row id. 
 - Now code along with the FOREIGN KEY table constrains. 
 - Listen carefully to the questions.
 - Code along with the last question adding the visits id, then DROP TABLES that were created before and run the query file and output ``.schema``` for the pow workflow.
 - At 53:35 there should be 3 queries commits with message:
    - **COMMIT MESSAGE - "table constrains and schema update"**

## Grading
This is how I will grade your work:
1. Did you provide the correct commit history URL for designing folder = 10 points
2. Did you do all the commits required for this work = 20 points
3. Did you have all the queries in the p1-q.sql file = 25 points
4. Did you create the pow-p1.txt file correctly and include all the required output = 20 points
5. Did you include all the required content in the README.md file = 30 points
- Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 