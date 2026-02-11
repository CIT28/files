## CS50 Relating Part 2
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture - Relating](https://www.youtube.com/watch?v=_2t18Hy9Z0Y)

## Setup
- Continue working in the relating folder, in the README.md add a heading 1 with the following content:
    'Week 7 Relating Part 2"
- Make sure you are in the relating folder and run this command to get sea_loins db:
    - ```curl -o sea_lions.db https://raw.githubusercontent.com/CIT28/files/main/w7/sea_lions.db```
- Copy the p1-q.sql content into a new file p2-q.sql, remove previous queries and update for pow-p2.txt and update the bash command with the sea_lions.db, then commit with message:
    - **COMMIT MESSAGE - "setup ready"**

## Joins - Starting at 55:50 to 1:17:00
- Notes 
    - In the README.md file add heading 2 md style and have this heading text:
        - 'JOIN'
    - Then under that heading take some notes to help you understand the concept of how JOIN works. No need to write the query yet
- Code Along - From timestamp 59:01
    - Setup the terminals and run sqlite3 with the sea_lions.db reference.
    - Write the "regular" query and the join query along with Carter in the p2-q.sql.
    - Use the .print 'what does this query to' to describe each query.
    - Once you have working output complete pow and git workflow and commit with message:
        - **COMMIT MESSAGE - "JOIN query"** 
- Notes
    - In the README.md file add heading 2 md style and have this heading text:
        - 'INNER JOIN'
    - Then under that heading take note on how INNER JOIN work and capture the questions and answers. 
    - Add heading 2 md style and have this heading text:
        - 'LEFT, RIGHT and FULL JOIN'
        - We will come back here later to fill in some content
- Code Along and Notes - From timestamp 1:06:53
    - Comment out the queries written so far
    - Code the LEFT,  RIGHT, and FULL JOIN query
    - Update the heading we create above and take and add the text of 'OUTER' to the heading and take notes on how each one works. 
    - Make sure to include in your notes answer this question: "How is left and right determined", not necessary for 3 table, but for 2 as we have done here.
    - Also include the answer to "do we get back a separate table" question, no need to write the last query here. 
    - Then add to the heading we are been building for these join type, add the text of 'NATURAL' and take a few notes on what a natural join is and then code along. 
    - Complete the pow and git workflow with commit message:
        - **COMMIT MESSAGE - "LEFT, RIGHT, FULL and NATURAL JOIN query"** 

## BREAK OPTIONAL  
- If you got this far you can take a break and complete the rest of this work by the Thursday night deadline.  
- To "GET" this break you will submit your commit history for the relating folder now.
- I will do a review and give you feedback.
- If you complete before Thurs morning, then you can submit again your commit history URL and tell me that you are ready for a second review. 

## Sets - Starting at 1:17:00
- Notes
    - In the README.md file add heading 2 md style and have this heading text:
        - 'Sets'
    - Then under that heading take note on how sets work and what is INTERSECT, UNION and EXCEPT as it relates to sets (results)
- Code Along - From timestamp 1:20:30
    - Make sure you update the p2-q.sql file to now reference the longlist.db instead of the sea_loins.db, make sure have the correct reference to the longlist.db by running .tables.
    - Code with queries all 9 queries for this section. 
    - At 1:31 take note of the final comment about when these types of queries would not work, then complete the pow and git workflows and commits with message:
        - **COMMIT MESSAGE - "Sets w EXCEPT INTERSECT"**

## Groups - Starting at 1:31:15
- Notes
    - In the README.md file add heading 2 md style and have this heading text:
        - 'Groups'
    - Then under that heading take notes on the concepts of groups

- Code Along
    - Write the queries for this section, for this part will be 3 queries here and then update your notes regarding group above.
    - Listen to the questions code the queries for a total of 5 queries here.
    - Complete the pow and git workflows and commit with message:
         - **COMMIT MESSAGE - "GROUP BY"**


## Grading
This is how I will grade your work:
1. Did you provide the correct commit history URL for relating folder = 10 points
2. Did you do all the commits required for this work = 20 points
3. Did you have all the queries in the p2-q.sql file = 25 points
4. Did you create the pow-p2.txt (my pow had 1328 lines) file correctly and include all the required output = 20 points
5. Did you include all the required content in the README.md file = 30 points
***MAKE SURE each commit includes the queries, pow and notes for that work.***
- Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 