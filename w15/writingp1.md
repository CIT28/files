## CS50 Writing Part 1

📺 **Watch Lecture**  
Right-click and select **“Open in new tab”** to view [CS50 SQL - Lecture 1 - Writing](https://www.youtube.com/watch?v=BD08USRd2M8)

---

### Markdown Legend

Use these Markdown syntaxes in your `README.md` file:

- **Headings**
  - `#` for H1
  - `##` for H2
- **Outline**
  - `*` or `-` for bullet points

---

## Setup

1. Create a new folder name it `writing` at the same level as `designing`
2. Create a new file `p1-q.sql` by copying a previous query file.
   - Remove any old queries.
   - Update to have `pow-p1.txt` output file.
3. Add an H1 heading to your `README.md`:  
   ```markdown
   # Writing Part 1
   ```
---
📍 Timestart: 00:00 to 21:00
### Inserting Data with INSERT INTO

- Add a ## heading `INSERT INTO` to your `README.md`:

- Take notes on how to add data to a table. Include these points:
   - MFA tracks artwork using a `collections` table.
   - How works `INSERT INTO `
   - Why `title` and `accession_number` cannot be NULL
   - Why `accession_number` must be UNIQUE

- Create the database `mfa.db` in the writing folder. 
- Include the `.print` to describe the SQL 
- Write SQL that Carter shows to create the collections table and run it.
- After it runs successfully comment out the SQL and output `.schema` to the pow-1.txt. 

💾 **Commit Message:** `"notes on INSERT INTO and collection table created."`

### INSERT Rows and Constraints

#### Add Rows with INSERT INTO
- Add rows to `collections` using `INSERT INTO`.
- Use Carter’s examples to insert:
- Use `SELECT * FROM collections;` to verify.
- Include a `.print` description in your SQL for each insert.
- Output the results to `pow-p1.txt`.

💾 **Commit Message:** `"added first rows to collections"`


#### Auto-increment ID and Constraint Violations
- Insert "Spring Outing" without specifying `id`, let SQLite auto-increment.
- Try inserting a duplicate `accession_number` and observe the UNIQUE constraint error.
- Try inserting NULL for `title` or `accession_number` and observe the NOT NULL constraint error.
- Use `.print` to explain each test in your SQL.
- Output any relevant schema and errors to `pow-p1.txt`.

💾 **Commit Message:** `"explored constraints: unique and not null"`

#### Insert Multiple Rows at Once
- Use a single `INSERT INTO` with multiple sets of values.
- Verify using `SELECT * FROM collections;`
- Add `.print` to describe this SQL block.
- Output results to `pow-p1.txt`.

💾 **Commit Message:** `"inserted multiple rows with one statement"`

📍 Timestart 21:00 

### Importing Data from CSV

- You will need the following file in your `writing` folder:
    -  ```curl -o mfa.csv https://raw.githubusercontent.com/CIT28/files/main/w15/mfa.csv```

#### Import CSV Into Existing Table
- Remove the existing `mfa.db`, no need to include these in your sql file.
- Create a new `mfa.db` and recreate the `collections` table from SQL already written by uncommenting the `CREATE TABLE...` from previous work.
- Add a new H2 heading:
   ```markdown
   ## Importing CSV
   ```
   - Take notes on how import works.
- Add a `.print` description in your SQL.   
- Write the command and arguments for `.import` excluding the header row in your p1-q.sql and copy it into the terminal to run
- Use `.schema` and `SELECT * FROM collections;` to verify data was imported and and run the pow and git workflow:

💾 **Commit Message:** `"imported mfa.csv into collections table"`

#### Import CSV Without Primary Key Using Temp Table
- Edit `mfa.csv` to remove the `id` column (primary key).
- Import the CSV into a new temp table
- Use `.schema` to verify `temp` table was created using header row.
- Use `SELECT * FROM temp;` to confirm data.
- Output schema and table results to `pow-p1.txt`.

💾 **Commit Message:** `"imported CSV without id into temp table"`

#### Insert from Temp Table and Cleanup
- Write SQL to DELETE the `collections` table
- Insert data from `temp` into `collections`
- Confirm rows inserted correctly using `SELECT * FROM collections;`.
- Drop the temp table.
- Add a `.print` to describe the insert process from temp to collections.
- Output final schema and results to `pow-p1.txt`.
- Listen to the questions.

💾 **Commit Message:** `"moved temp table data into collections with primary keys"`

## BREAK OPTIONAL  
- If you got this far you can take a break and complete the rest of this work by the Thursday night deadline.  
- To "GET" this break you will submit your commit history for the writing folder now.
- I will do a review and give you feedback.
- If you complete before Thurs morning, then you can submit again your commit history URL and tell me that you are ready for a second review. 


### DELETE FROM
📍 Timestart: 37:00

#### Deleting a Single Row
- Write the SQL to delete the 'Spring outing'.
- Verify deletion
- Also delete with NULL condition:
   - Did it work? Mine did not and I'm guessing yours did not. 
   - Anything idea why? 
   - Note your thoughts or what you did to figure it out in your README.md, then watch this video from me - https://youtu.be/xztU0Wpuw1c
- Use `.print` to explain the purpose of each deletion.
- Output updated table to `pow-p1.txt`.

💾 **Commit Message:** `"deleted Spring outing and rows with NULL acquired"`


####  Deleting Multiple Rows Using Date
- Delete all artwork acquired before 1909
- Explain in your SQL why this date matters (MFA moved in 1909).
- Confirm the result 
- Add a `.print` to describe the deletion criteria.
- Output results to `pow-p1.txt`.

💾 **Commit Message:** `"deleted rows acquired before 1909"`


#### ✅ Deletion Notes and Cautions
- Take notes on how:
  - `DELETE FROM` requires a `WHERE` clause to avoid clearing the table.
  - Dates in SQLite can be compared using `YYYY-MM-DD` format.
  - Removing rows permanently affects the table’s structure (IDs are not reused).
- Use `.print` in your SQL to reflect this summary.
- Add note that `DELETE` is irreversible unless wrapped in a transaction.

💾 **Commit Message:** `"added notes on DELETE FROM best practices"`


## Grading Rubric

| Criteria                                                                | Points |
|-------------------------------------------------------------------------|--------|
| ✅ Correct commit history URL for `writing` folder                      | 10     |
| ✅ All required commits are included                                    | 20     |
| ✅ All queries are present in `p1-q.sql`                                | 25     |
| ✅ Correctly created `pow-p1.txt` with required output                  | 20     |
| ✅ Complete and accurate `README.md` content                            | 25     |
| ❗ Late submissions will be penalized 25 points                         |        |
|-------------------------------------------------------------------------|--------|
**Example:** If submitted late but otherwise complete, you will receive 75/100.




