# CS50 Problem Set 1 Part 1 
## Department of Elementary and Secondary Education
## 1 thru 6

### Setup
- Inside the folder ps1 folder, make sure it is at the same level as packages,  then create another folder named dese.
-  Change the current folder to dese, then use the following command to copy the database file:
    - ```curl -o dese.db https://raw.githubusercontent.com/CIT28/files/main/w6/dese.db```
    - Create a file to store the queries name it p1-q.sql and a README.md include heading "DESE 1 thru 6" and commit with message:
        - **COMMIT MESSAGE - "setup complete"**

### Steps
1. In your README.md file have a heading "Get to know the packages dataset"
    
    - Review https://cs50.harvard.edu/sql/2024/psets/1/packages/

    - Write at least 2 queries, in the p1-q.sql, that help you get to know the database. Create a subheading for "playing around w statics queries" 
    - Don't work on the Lost Letter problem yet. 
    - Write queries one line at time (static query) and have a sub heading for each query and the text should reflect what the query is "doing".  
    - Make sure your static queries includes at least 2 tables, once you have a working queries, output to proof of work (pow1.txt) file and then commit with message:
    - **COMMIT MESSAGE - "playing around queries - static"**

2. Now add a heading "playing around w nested queries"
    - Comment out static queries from above and then take static queries from step 1 and refactor into nested query, once you have working query, update the proof of work file and then commit with message:
        - **COMMIT MESSAGE - "playing around queries - nested"**

3. Review the problem
    - Clerk, my name’s Anneke. I live over at 900 Somerville Avenue. Not long ago, I sent out a special letter. It’s meant for my friend Varsha. She’s starting a new chapter of her life at 2 Finnegan Street, uptown. (That address, let me tell you: it was a bit tricky to get right the first time.) The letter is a congratulatory note—a cheery little paper hug from me to her, to celebrate this big move of hers. Can you check if it’s made its way to her yet?

    - Unlike the CS50 example here is what you will need to write queries to answer -  "What time was the package picked up and dropped off include timestamps and related action" .  

4. Write static queries
    - In your README.md file create a heading for "Static Queries for Lost Letter" and write about how you would approach the problem.  
    - Then in the create a comment line for he queries you will write in the p1-q.sql, -- Lost Letter Static Queries. 
    -  Then write the queries to solve the problem, there should be at least 4 queries here and once you have working code, update the proof of work file (pow1.txt) and commit with message
        - **COMMIT MESSAGE - "Lost Letter static queries"**

5. Write nested queries
    - In your README.md file create a heading for "Nested Queries for Lost Letter". 
    - Then in the create a comment line for he query you will write in the p1-q.sql, -- Lost Letter Static Queries. Then write the query to solve the problem (only 1 nested query here) and once you have working code, update the proof of work file (pow1.txt) and commit with message
            - **COMMIT MESSAGE - "Lost Letter nested query"**

6. Write about your experience
    - Create a new heading in your README.md file "My Experience"
    - Under that heading write paragraph about doing this work.  

## Grading
- Submit your commit history URL the packages folder in your private repo for grading
- This is how I will grade your work:
    1. Did you provide the correct URL for packages folder commits = 5 points.
    2. Did you do all the commits required for this work = 65 points
        -  There should be 5 commits, 1 for the setup and 4 that show the current query (or quweries) (uncommented), proof of work and autenciate work in README.md and output the correct data. 
    3. Did your README.md file show authenicate work =  30 points
    4. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 