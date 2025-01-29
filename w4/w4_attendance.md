# Week 4 Attendance
## Getting to know cyberchase database and learning the new authentic workflow
- https://cs50.harvard.edu/sql/2024/psets/0/cyberchase/

### Setup
- Create a new folder at the same level querying, name it ps0 (short for "Problem Set 0") and then inside that folder create another folder named cyberchase.   
- In the terminal change the current folder to cyberchase, then use the following command to copy the database file:
    - ```curl -o cyberchase.db https://raw.githubusercontent.com/CIT28/files/main/w4/cyberchase.db```
    - Create a file to store the queries name it a-q.sql and copy the contents of the p4-q.sql in the querying folder
        - Remove any previous queries and update the content to reference cyberchase instead of longlist, pow-a.txt instead of pow4.txt
        - Change any references from p4-q.sql to a-q.sql
    - Create a README.md and using heading 1 markdown (md) style have this heading text 
        - 'Week 4 Attendance' 
      - **COMMIT MESSAGE - "setup done"**
### Learn the Proof of Effort (poe) workflow
- Start the terminal sessions 
    1. Start a SQLITE3 session using the new database reference, make sure to have the current folder be cyberchase. 
    2. Start another Bash session (to run pow and git commands), make sure to have the current folder be cyberchase. 
- In the README.md, after the heading 1 
    - Using heading 2 md style have this text 
    - 'Query 1' 
    - Then on a next line have this:
        - 3 backticks <code>```</code>
        - blank line
        - 3 backticks <code>```</code> 

- Now in your SQLITE3 terminal attempt this query:
    - Query 1 - Write a query to list all data in the episodes table in the cyberchase database. Format your output for readability. 
        - Successful output will have 140 records and 7 columns
        - Between the backticks (done above) copy the commands and code you wrote in SQLITE3 terminal to get successful output
        - DO NOT INCLUDE SUCCESSFUL OUTPUT, just the commands you wrote
        - THIS IS THE NEW POE WORKFLOW
        - Complete the pow and the git workflow and commit with message:
            - %sure is how sure you got this correct
            - **COMMIT MESSAGE - "query 1 and workflows done %sure"**
        -run this command to clear your terminal ```.shell clear``` before starting the next query. 
    - In the README.md, after the heading 2 from Query1
        - Using heading 2 md style have this text 
        - 'Query 2'
        - Then on a next line have this:
            - 3 backticks <code>```</code>
            - blank line
            - 3 backticks <code>```</code> 
        - Query 2 - Write a query to list all the episode title that have 'or' in their text.
            - Successful output will be 19 titles and 1 column
            - Between the backticks (done above) copy the commands and code you wrote in SQLITE3 terminal to get successful output
            - DO NOT INCLUDE SUCCESSFUL OUTPUT, just the commands you wrote
            - THIS IS THE NEW POE WORKFLOW
            - Complete the poe workflow
            - Complete the pow and git workflow and commit with message: 
                - **COMMIT MESSAGE - "query 2 and workflows done %sure"**
