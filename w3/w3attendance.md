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
## Challenge 1: The Top Rated Books

**Goal**
Find the highest-scoring books in the dataset.

**Context**
A reader wants to know which books are the "best of the best" based on their rating score. We need to provide a curated short-list of the highest-rated entries.

**The Task**
Write a query that retrieves the `title` and `rating` from the `longlist` table. The results must be ranked by rating, starting with the highest score. To keep the list concise, the output should contain only the top 5 results.

**Requirements**
1. Print the label: `'Top Rated Query'`
2. Select the `title` and `rating` columns.
3. Sort the results so the highest ratings appear at the top.
4. Ensure only the first 5 rows are displayed.

**Expected Output**
```text
Top Rated Query
┌────────────────────────────────┬────────┐
│             title              │ rating │
├────────────────────────────────┼────────┤
│ The Eighth Life                │ 4.52   │
│ A New Name: Septology VI-VII   │ 4.5    │
│ The Other Name: Septology I-II │ 4.19   │
│ The Years                      │ 4.18   │
│ Still Born                     │ 4.14   │
└────────────────────────────────┴────────┘
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


## Challenge 2: The "Goldilocks" Length

**Goal**
Filter results to find values that fall within a specific numerical range.

**Context**
A reader is looking for a book that isn't too short, but also isn't a massive 1,000-page commitment. They want something "just right"—specifically, books that have between 200 and 300 pages.

**The Task**
Write a query that selects the `title` and `pages` from the `longlist` table. You need to filter the results to show only books where the page count is 200 or more, but no higher than 300 (inclusive).

**Requirements**
1. Print the label: `'Page Range Query'`
2. Select the `title` and `pages` columns.
3. Filter the results to include only books with a page count ranging from 200 to 300.

**Expected Output**
```text
Page Range Query
┌────────────────────────────────────────────┬───────┐
│                    title                   │ pages │
├────────────────────────────────────────────┼───────┤
│ Standing Heavy                             │ 252   │
│ Pyre                                       │ 224   │
│ Still Born                                 │ 200   │
│ Ninth Building                             │ 272   │
│ Love in the Big City                       │ 217   │
│ The Book of Mother                         │ 224   │
│ More Than I Love My Life                   │ 288   │
│ Phenotypes                                 │ 232   │
│ A New Name: Septology VI-VII               │ 228   │
│ Cursed Bunny                               │ 251   │
│ An Inventory of Losses                     │ 256   │
│ Summer Brother                             │ 285   │
│ The Perfect Nine                           │ 240   │
│ The Adventures of China Iron               │ 200   │
│ The Discomfort of Evening                  │ 282   │
│ The Enlightenment of The Greengage Tree    │ 256   │
│ The Memory Police                          │ 277   │
│ Hurricane Season                           │ 229   │
│ Little Eyes                                │ 256   │
│ Mac and His Problem                        │ 224   │
│ Celestial Bodies                           │ 243   │
│ Drive Your Plow Over the Bones of the Dead │ 270   │
│ Love in the New Millennium                 │ 288   │
│ Mouthful of Birds                          │ 228   │
│ The Years                                  │ 232   │
│ Frankenstein in Baghdad                    │ 272   │
└────────────────────────────────────────────┴───────┘
```


This prevents **duplicate output** in your text file.

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
* Does your final `pow-w3.txt` contain the results **AND** the descriptions? (Mine was 41 lines)
* *Check:* Did you remember to use `.print` before every query?

**5. Notes  (10 Points)**
* Does your final `README.md` contain required?


---