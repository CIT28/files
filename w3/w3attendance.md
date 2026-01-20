# Week 3 Attendance Coding Challenge

## 1. Create your SQL File
* Create a new file named `w3-q.sql` inside your `querying` folder.
* **Do not** manually copy the old file. Instead, copy the code block below and paste it into your new `w3-q.sql` file.

```sql
-- starting the pow workflow
.mode box
.output '| cat >> pow-w3.txt'

-- ⬇️ WRITE YOUR QUERIES BELOW THIS LINE ⬇️
-- (Remember to .print 'description' before each query)


-- ⬆️ END OF QUERIES ⬆️

-- changes back to stdout
.output stdout

-- bash command (for reference): sqlite3 longlist.db < w3-q.sql
```
## 2. Open Your Terminals

### Terminal 1 (SQlite3 to write queries)
- Navigate to the `querying` folder and then run the following command:

- `sqlite3 longlist.db`

Use this terminal to test queries interactively **before** saving them to your SQL file.

### Terminal 2 (Bash to complete GIT and POW Workflows)
- Navigate to the `querying` folder
- Use this terminal for **Git** and **POW** commands

---
## 3. Initial Commit

In your `README.md`, add the following **Heading 1**:

```md
# Week 3 Attendance
```

Then complete your Git workflow in **Terminal 2**.

📌 **Commit message to use:**  
`week 3 attendance query file and README.md ready`

---
## Challenge 1: The "2021 Hardcovers"

**Goal**
Find the highest-scoring books in the dataset.

**Context**
We need to find a list of specific physical books for a display. We are looking for books released in 2021 that were printed in the hardcover format.

**The Task**
Write a query that retrieves the `title` and `author` from the `longlist` table. You need to filter the results to only include books where the year is exactly 2021 AND the format is 'hardcover'.

**Requirements**
1. Print the label: `'2021 Hardcover Query'`
2. Select the `title` and `author` columns.
3. Filter the results: 
  * Year must be 2021
  * Format must be 'hardcover'

**Expected Output**
```text
┌───────────────────────────────────────┬───────────────────┐
│                 title                 │      author       │
├───────────────────────────────────────┼───────────────────┤
│ The War of the Poor                   │ Éric Vuillard     │
│ When We Cease to Understand the World │ Benajamín Labatut │
│ An Inventory of Losses                │ Judith Schalansky │
│ At Night All Blood is Black           │ David Diop        │
│ I Live in the Slums                   │ Can Xue           │
│ The Perfect Nine                      │ Ngũgĩ wa Thiong'o │
└───────────────────────────────────────┴───────────────────┘
```

### 2. Code on the sqlite3 terminal and then copy the query into `w3-q.sql`
- **Test:** Write and refine your query in the SQLite terminal until it matches the expected output.
- **Save:** Copy your final query into `w3-q.sql`.
- **Document:** In your `README.md`:
    - Confirm that your output matched the expected results.
    - **If you could not get the correct output:** Describe the approaches you tried and where you got stuck and include your final query in `w3-q.sql`

### 3. ✅ Checkpoint
- In terminal 1 run the POW:
  - `sqlite3 longlist.db < w3-q.sql`

-   Commit your work

📌 In terminal 2 **Commit message to use:**  
`Code Challenge 1`

### 🛑 STOP & CLEAN UP
Before moving to the next section:
- Comment out the queries you just wrote in `w3-q.sql`
- Add `--` before each line


## Challenge 2: The 2020 Originals

**Goal**
Filter for "empty" or NULL values combined with other criteria.

**Context**
A researcher is looking for books that were written in their original language (not translated) and published in the year 2020. In our database, if a book has no translator, that column is `NULL`.

**The Task**
Write a query that selects the `title` and `author` from the `longlist` table. Filter the results to find books where the `translator` is empty (NULL) AND the `year` is 2020.

**Requirements**
1. Print the label: `'2020 Originals Query'`
2. Select the `title` and `author` columns.
3. Filter the results: 
  * Translator must be `NULL`
  * Year must be 2020

**Expected Output**
```text
2020 Originals Query
┌─────────────────────────────────────────┬────────────────┐
│                  title                  │     author     │
├─────────────────────────────────────────┼────────────────┤
│ The Enlightenment of The Greengage Tree │ Shokoofeh Azar │
└─────────────────────────────────────────┴────────────────┘
```


### 2. Code on the sqlite3 termianl and then copy into `w3-q.sql`
- **Test:** Write and refine your query in the SQLite terminal until it matches the expected output.
- **Save:** Copy your final query into `w3-q.sql`.
- **Document:** In your `README.md`:
    - Confirm that your output matched the expected results.
    - **If you could not get the correct output:** Describe the approaches you tried and where you got stuck and include your final query in `w3-q.sql`

### 3. ✅ Checkpoint
- Run the POW:
  - `sqlite3 longlist.db < w3-q.sql`
- Commit your work

📌 **Commit message to use:**  
`Code Challenge 2`


**1. Submission **
* Nothing to submit, as part of my review of attendance I will look at your private repo, so make sure you push your code to github.

**2. Commit History (10 Points)**
* Are all required commits present, and do they contain the required **Notes + SQL + POW** for that section?
* *Required Commits:*
    * "Code Challenge 1"
    * "Code Challenge 2"

**3. SQL Source Code (40 Points)**
* Does your final `w3-q.sql` contain the valid SQL syntax for both queries?

**4. Proof of Work Output (20 Points)**
* Does your final `pow-w3.txt` contain the results **AND** the descriptions? (Mine was 16 lines)
* *Check:* Did you remember to use `.print` before every query?

**5. Notes  (10 Points)**
* Does your final `README.md` contain required?


---