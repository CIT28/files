## CS50 Relating Part 1
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture - Relating](https://www.youtube.com/watch?v=_2t18Hy9Z0Y)

## Setup
### Week 6 Attendance 
1. Create a new folder at the same level querying, name it relating.
2. In the terminal change the current folder to relating, then use the following command to copy the database file:
    - ```curl -o longlist.db https://raw.githubusercontent.com/CIT28/files/main/w6/longlist.db```
3. In the relating folder create the file we will use for notes - README.md, using heading 1 markdown (md) style and have this heading text:
    - 'Week 6 Relating Part 1' 
    - below that create a heading 2 with this heading text:
    - 'Week 6 Attendance
4. In the relating folder create a file a-q.sql and copy the contents of the p1-q.sql from the cyberchase folder into this file.
    - Update the a-q.sql to reference the pow-ds.txt and bash command at the end to be a-q.sql.
    - Remove all previous queries
5. Setup the SQLITE3 and Bash terminals
     - **COMMIT MESSAGE - "setup done"**
6. Code along with me

### Start here for Relating Part 1 
- In the relating folder create a file p1-q.sql and copy the contents of the a-q.sql.
    - Update the p1-q.sql to reference the pow-p1.txt and bash command at the end to be p1-q.sql.
    - Remove all previous queries
- Start the terminal sessions   
- In the README.md file add heading 2 md style and have this heading text:
    - 'Overview of Relating Concepts'
    - **COMMIT MESSAGE - "updates done"**

## Take notes from timestamp 00:00 to 26:40
- In the README.md file organize your notes in the following using heading 3 md style.
    - "Relating", "Entity Relationship Diagrams (ERD)" and "Keys"
        - For each heading take notes that will help you understand the content and concepts cover and help me see you took the time to understand the concepts. 
        - After the Relating content commit with message:
            - **COMMIT MESSAGE - "Relating"**
        - After the ERD content commit with message:
            - **COMMIT MESSAGE - "ERD"**            
        - After the key content commit with message:
            - **COMMIT MESSAGE - "Keys"** 


## 1:N Subqueries - Starting at timestamp 26:50
- Notes 
    - In the README.md file add heading 2 md style and have this heading text:
        - '1:N Subqueries'
        - Then under that heading take a few notes on subquery and describe how we approaching writing them. 
        - No need to write the query yet, just follow along. 
        - Make sure to note which part of the subquery runs first and the syntax that is used to show the subquery
- Code Along - From timestamp 33:58
    - Make sure the p1-q.sql is setup correctly to output to the pow-p1.txt and bash command at the bottom is correct for p1-q.sql
    - In the SQLITE3 terminal (or in the query file), code along with Carter and write the 2 static queries. 
        - Once the queries runs without error make sure they are in the p1-q.sql file.
        - Use the .print 'what does this query to' to describe each query.
        - Complete the pow and git workflow, then
            - **COMMIT MESSAGE - "1:N static queries"**
- Code Along - From timestamp 35:58
    - In the SQLITE3 terminal (or in the query file), code along with Carter and write a subquery from the static query above. 
        - Once the subquery runs without error make sure it is in the p1-q.sql file.
        - Use the .print 'what does this query to' to describe each query.
        - Complete the pow and git workflow, then
            - **COMMIT MESSAGE - "1:N subquery"**
- Code Along - From timestamp 37:25
    - Code both the static query and subquery (either on the terminal or in the query file)
        - There will be 2 static query and 2 versions of the subquery
        - Once your have the query running without error.
        - Use the .print 'what does this query to' to describe each query.
        - Complete the pow and git workflow, then
            - **COMMIT MESSAGE - "1:N static and subquery"**

## BREAK OPTIONAL  
- If you got this far you can take a break and complete the rest of this work by the Thursday night deadline.  
- To "GET" this break you will submit your commit history for the relating folder now.
- I will do a review and give you feedback.
- If you complete before Thurs morning, then you can submit again your commit history URL and tell me that you are ready for a second review. 

## M:N Subquery
- Code Along - From timestamp 40:31
    - Write combination of static queries and subquery  (either on the terminal or in the query file)
        - There will be total of 3 queries here
        - Once your have the query running without error.
        - Use the .print 'what does this query to' to describe each query.
        - Complete the pow and git workflow, then
            - **COMMIT MESSAGE - "M:N static and subquery"**
        - Listen to the questions

- Code Along - From timestamp 47:35
    - Listen to concepts of how to use IN SQL commands
    - Code along write combination of static queries and subquery  (either on the terminal or in the query file)
        - There will be total of 3 queries here
        - Once your have the query running without error.
        - Use the .print 'what does this query to' to describe each query.
        - Complete the pow and git workflow, then
            - **COMMIT MESSAGE - "M:N subquery using IN"**    


# Grading
This is how I will grade your work:
1. Did you provide the correct URL for relating folder commit history = 10 points
2. Did you do all the commits required for this work = 20 points 
    - Make sure you commits include queries, pow and any related notes
3. Did you have all the queries in the p1-q.sql file = 25 points
4. Did you create the powp1.txt file include all the required output and short description of each query = 25 points
5. Did you include all the required content in the README.md file = 20 points
6. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 