# CS50 Writing Part 2
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 1 - Writing](https://www.youtube.com/watch?v=BD08USRd2M8)


### Timemark 1:02 to end
- Continue working in the writing folder, in the README.md add a heading for 'Writing Part 2'.
- Rename the write.sql to write-1.sql and create a new file write-2.sql 
- Recreate the mfa.db from the code in the schema.sql file we used for the last version of the mfa.db. 
    - In case you want to review that, here is a link it from part 1 - [schema](writingp1.md#MFA2)
    - **COMMIT MESSAGE - "setup done"**

- Now make sure you have the same schema and data as Carter and code along to do the update and then code the UPDATE in the write2.sql file, make sure to NOT run until you have the complete query. 
- Then make sure the updated worked and then add a subheading in your README.md file for UPDATE and take a few notes about how this SQL command works, update your pow2.txt and run this command get the votes.csv fiel. 
    -```curl -o votes.csv https://raw.githubusercontent.com/CIT28/files/main/w11/votes.csv```
- Create the votes.db and code the .import into your write-2.sql file and make sure you .import worked and update your pow1.txt file.
- Code the query to tally the votes, update your pow2.txt file and then comment it out. 
    - I moved this talley query to the bottom of the query file, that way it would NOT need to comment and uncommet it each time. Below I say rerun, so just know that is another way to be a bit more productivity with this part of the code along. 
- Code the UPDATE with trim function query, make sure it works, update the pow2.txt and then add a subheading and note how trim works in this query.
- Code the UPDATE with upeer function query, make sure it works, update the pow2.txt and then add a subheading and note how upper works in this query.
- Rerun the tally query, code the 2 UPDATE queries and rerun the tally.  
- Code the UPDATE using LIKE query and then rerun tally, code the UPDATE for the next title.
    - For 'IMAGINTIVE LANDSCAPE', mine was correct after this query, so just make sure your was as well. 
- Code last UPDATE and then re-run tally and update your pow2.txt. 
- Listen to the questions. 
    - **COMMIT MESSAGE - "cleaning data with UPDATE trim and upper functions"**
- Terminate the sqlite shell for votes.db and restart with mfa.db.
- At 1:24, add a subheading to triggers and take a few notes on how is a trigger and the different way it will run and what does BEGIN and END do in this type of query.
- Now code the CREATE transactions table, run it and code the TRIGGER query.
- In your README.md, describe what each line in this query does, does you need to write it as Carter has shown here. 
- Now run the query, then output the .schema to the pow2.txt.
- Now code the DELETE
    - HEADS UP HERE, be careful and write the syntax correctly. I say this because I didn't and had to look up this command: 
    <code>DROP TRIGGER IF EXIST "sell";</code>
- Once you get the transactions table updated, then output the contents and the .schmea to the pow2.txt.
- Listen to the question and the commit with message:
    - **COMMIT MESSAGE - adding TRIGGER to schema"**
- Continue at 1:37 and add a heading for Soft Deletions and describe what it is and why we would implement it. 
- Now code the ALTER TABLE query, then code the UPDATE query, make sure the query works and you see the deleted column updated for 'Farmers working at dawn'.
- Now code the SELECT query, I did noticed mine was 1 row off what Carter had so no worries if you see something similar. 
- Carter makes and very interesting point at the end about best practices, add a sub heading "user data my thoughts" to your README.md and reply to the comment and/or research GDPR and right to be forgotten and give you reply based on what you learned. 
        - **COMMIT MESSAGE - soft deleteion my thoughts"**

## Grading
-This is how I will grade your work:
1. Did you provide the correct commit history URL for the writing (all lowercase) folder = 5 points
2. Did you do all the commits required for this work = 15 points
3. Did you have all the queries in the write.sql file = 30 points
    - make sure you not include notes in your sql file. 
    - You can include, but don't need to include the SELECT * FROM queries that Carter does on the terminal
    - I counted 17 queries in my write-2.sql
4. Did you create the powp2.txt include all the required output = 20 points
5. Did you include all the required content in the README.md file = 30 points
6. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 

