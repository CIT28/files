# CS50 Problem Set 1 - Lost Letter Static and Nested Subqueries

https://cs50.harvard.edu/sql/psets/1/packages/

## Attendance

### Setup the .gitignore
- Open your private repo codespace
- Open your terminal and have your current folder  be /workspaces/your-pri
- Open that file and add this into the file 
    - ```*db```
- Complete the git workflow like this:
    - ```git add .gitignore```
    - ```git commit -m "Update .gitignore to ignore all .db files"```
    - ```git push```
- You can copy the message into the terminal to no longer see this message:
    - ```hint: Use -f if you really want to add them.```
    - ```hint: Disable this message with "git config advice.addIgnoredFile false"```

###  New Dataset
- In your codespace create a new folder named ps1 folder and then inside ps1 create another folder name packages.
-  Change the current folder to packages, then use the following command to copy the database file:
    - ```curl -o packages.db https://raw.githubusercontent.com/CIT28/files/main/w8/packages.db```
    - If you completed the update to the gitignore file correct, this database file will be a little grayed out.
    - Create a new query file (w8-q.sql) by copying a previous sql file we have used. Remove any queries in the file and update bash command and pow reference to be pow-ds.txt.

    - In the w8-q.sql write following commands and queries:
        1. Display Tables and Schema in the packages.db
        2. Write queries to output all the columns of each table in the packages db with the first 10 records. Make sure to use .print 'text' to describe each query.
        3. Once you have correct output, complete the  pow and git workflows with commit message:
            - **COMMIT MESSAGE - "new database"**
    - Comment out queries

### Coding Challenge
- Create the README.md in the packages folder and add a heading 1 with text 'Week 8 attendance coding challenge and then heading 2 for each problem below 1 thru 5.
    - Update the w8-q.sql to reference pow of pow-a.txt
    - Make sure you copy your query attempts under the heading for each problem using this syntax:
        - ```backticks your query attempt```
- Write a regular query, static or subquery in the w8-q.sql to answer the following:

1. Retrieves all the information about drivers whose name is "Derek" from the drivers table.
2. Count how many times driver "Derek" performed a "Pick" action in 2023 from the scans table.
3. Count the number of residential addresses in the addresses table
4. Count the number of business addresses in the addresses table
5. Count how many times each type of content appears in the packages table and lists the contents along with their count, sorting them from most to least common.
- After each query complete the poe, pow and git workflow with message:
    - *** Query 1 ***
    - There should be a total of 5 commits and here is a link to the results of having a correct query for each one. [link](results.txt)

## Lost Letter - Static and Nested Queries

### Static Queries

1. Review the problem
    - Clerk, my name’s Anneke. I live over at 900 Somerville Avenue. Not long ago, I sent out a special letter. It’s meant for my friend Varsha. She’s starting a new chapter of her life at 2 Finnegan Street, uptown. (That address, let me tell you: it was a bit tricky to get right the first time.) The letter is a congratulatory note—a cheery little paper hug from me to her, to celebrate this big move of hers. Can you check if it’s made its way to her yet?

    - Unlike the CS50 example here is what you will need to write query(s) to answer 
        - "What time was the package picked up and dropped off include timestamps and related action" .  
    - Here is the final output for both the static and nest queries:
        <pre>
        ┌────────┬────────────────────────────┐
        │ action │         timestamp          │
        ├────────┼────────────────────────────┤
        │ Pick   │ 2023-07-11 19:33:55.241794 │
        │ Drop   │ 2023-07-11 23:07:04.432178 │
        └────────┴────────────────────────────┘
        </pre>

2. Write static queries
    - In the packages folder create a new file named lost-q.sql and copy previous sql file, update pow reference to be pow-lost.txt and update the bash reference.
    - In your README.md file create a heading 2 for "Static Queries for Lost Letter - Proof of Effect.  
    -  Then write the static queries (one at time) to solve the problem, there should be at least 4 queries here. 
    - After each query complete the poe, pow and git workflow with message 
        - **COMMIT MESSAGE - "Lost Letter static queries 1"**
    - Comment out these queries before coming on to the next static query.

## BREAK OPTIONAL  
- If you got this far you can take a break and complete the rest of this work by the Thursday night deadline.  
- To "GET" this break you will submit your commit history for the packages folder now.
- I will do a review and give you feedback.
- If you complete before Thurs morning, then you can submit again your commit history URL and tell me that you are ready for a second review. 


3. Write nested subqueries 
- In your README.md file create a heading 2 for "Nested Queries for Lost Letter - Proof of Effect.  
    -  Then write the nested subquery  to solve the Lost Letter, there should be at 1 nested subquery here. 
    - Same output as the static query
    - Once you have a working query complete the poe, pow and git workflow with message 
        - **COMMIT MESSAGE - "Lost Letter nested query"**



4. Write about your experience
    - Create a new heading in your README.md file "My Experience"
    - Under that heading write paragraph about doing this work.  

## Grading
- Submit your commit history URL the packages folder in your private repo for grading

This is how I will grade your work:
1. Did you provide the correct URL for packages folder commits = 10 points.
2. Did you do all the commits required for this work = 30 points
3. Did your poe show authenticate work and include 'My Experience' =  30 points
4. Did you get the correct output for both static and nested queries = 30 points
- Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 