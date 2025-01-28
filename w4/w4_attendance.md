# Week 4 Attendance
## Getting to know cyberchase database and learning the new authentic workflow
- https://cs50.harvard.edu/sql/2024/psets/0/cyberchase/

### Setup
- Create a new folder at the same level querying, name it ps0 (short for "Problem Set 0") and then inside that folder create another folder named cyberchase.   
- Change the current folder to cyberchase, then use the following command to copy the database file:
    - ```curl -o cyberchase.db https://raw.githubusercontent.com/CIT28/files/main/w4/cyberchase.db```
    - Create a file to store the queries name it w4a-q.sql and copy the contents of the p4-q.sql in the querying folder
        - Remove any previous queries and update the content to reference cyberchase instead of longlist, pow-w4a.txt instead of pow4.txt
    - Create a README.md and using heading 1 md style have this heading text 
        - 'Week 4 Attendance' 
      - **COMMIT MESSAGE - "setup done"**
### Learn the Authentic workflow
- Start the terminal sessions 
    1. Start a SQLITE3 session using the new database reference 
    2. Start another Bash session (to run pow and git commands)
- In the README.md, after the heading 1 
    - Using heading 2 markdown (md) style have this text 
    - 'Query 1' 
    - Then on a next line have this:
        - 3 backticks <code>```</code>
        - blank line
        - 3 backticks <code>```</code> 

- Now in your SQLITE3 terminal attempt this query:
    - Query 1 - Write a query to list all data in the episodes table in the cyberchase database. Format your output for readability. 
        - Successful output would be 140 records and 7 columns
        - Between the backticks (done above) copy the commands and code in the SQLITE3 terminal to get successful output
        - DO NOT INCLUDE THE OUTPUT, just the commands you wrote
        - THIS IS THE NEW AUTHENTIC WORKFLOW
        - Complete the pow and the git workflow and commit with message:
            - %sure is how sure you got this correct
            - **COMMIT MESSAGE - "query 1 and workflows done %sure"**
    - Query 2 - Write a query to list all the episode title that have 'or' in their text.
        - Successful output will be 19 titles and 1 column
        - Complete the authentic workflow
        - Complete the pow and git workflow and commit with message: 
            - **COMMIT MESSAGE - "query 2 and workflows done %sure"**