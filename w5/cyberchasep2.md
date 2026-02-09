# 💻 CyberChase Part 2 Problem Set (Problem 8 thru 13)

# Setup
## 1. Create your SQL File
* Create a new file named `p2-q.sql` inside your `ps0/cyberchase` folder.
* **Do not** manually copy the old file. Instead, copy the code block below and paste it into your new `p2-q.sql` file.
9
```sql
-- starting the pow workflow
.mode box
.output '| cat >> pow2.txt'

-- ⬇️ WRITE YOUR QUERIES BELOW THIS LINE ⬇️
-- (Remember to .print 'description' before each query)


-- ⬆️ END OF QUERIES ⬆️

-- changes back to stdout
.output stdout

-- bash command (for reference): sqlite3 cyberchase.db < p2-q.sql
```
## 2. Open Your Terminals

### Terminal 1 (SQlite3 to write queries)
- Navigate to the `ps0/cyberchase` folder and then run the following command:

- `sqlite3 cyberchase.db`
- `.mode box`

Use this terminal to test queries interactively **before** saving them to your SQL file and to **capture** your query attempts to solve the problem that will be your Proof of Effort (POE).

### Terminal 2 (Bash to complete GIT and POW Workflows)
- Navigate to the `ps0/cyberchase` folder
- Use this terminal for **Git** and **POW** commands

---

## 3. Initial Commit

In your `README.md`, add the following **Heading 1**:

```md2
```

Then complete your Git workflow in **Terminal 2**.

📌 **Commit message to use:**  
`cyberchase setup ready`

---

# ⚙️ The Workflow (Repeat for **EACH** Problem)

For **every problem** listed below (**8 through 13**), you must perform this exact cycle:

---
## 1. Add problem heading to README.md

In your `README.md`, add the following **Heading 2**:

```md
## Problem # 
```

## 🔁 The Loop 

---

### ✅ Attempt
Type your best-guess query in the terminal.

---

### ❌ Fail / Verify

### If it gives an **Error**  
Example: `Parse error: no such column...`

1. **STOP.** Do not clear the screen.  
2. Select the text in the terminal (**your failed query + the error message**).  
3. Paste it into `README.md` **inside a code block** 

### If it gives **Wrong Data**
1. Select the query + the **first few rows** of the wrong result.  
2. Paste it into `README.md`.

---

### 🔧 Refine
Try again until you get the correct result matching the **Validation** criteria.

---

### 🏁 Finalize
Once correct:
- Copy **only** the working SQL query into `p2-q.sql` for the official solution.

---

## 3. ✅ Proof of Work
- In terminal 2 run the POW:
  - `sqlite3 cyberchase.db < p2-q.sql`

---

## 🚀 Git Commit
- Commit your work **immediately after generating the POW**
- Use the following commit message format:

```text
Problem #
```
---

### 🛑 STOP & CLEAN UP
Before moving to the next section:
- Comment out the queries you just wrote in `p2-q.sql`
- Add `--` before each line

## REPEAT FOR EACH PROBLEM

## Problem 8: The "Lost Decade" 

**Task:**  
Find the `air_date` of the very last episode that aired in the year 2009. Alias as last_ep_2009.

**Validation:**
- **Columns:** 1 (`last_ep_2009`)
- **Rows:** 1

---

## Problem 9: The Season Premiere

**Task:**  
Count the total number of episodes that aired in June, July, OR August (of any year). Alias the result as 'summer_episodes'.

**Validation:**
- **Columns:** 1 (`summer_episodes`)
- **Rows:** 1

---

## Problem 10: The Shortest Titles

**Task:**  
List the id and title of the first 10 episodes when sorted by title Z-A (Reverse Alphabetical).

**Validation:**
- **Columns:** 2 (`id`, `title`)
- **Rows:** 10

---
## ☕ The “Thursday Break” Option

Feeling the burn? If you have completed everything above, you may pause here.

### To take the break:
- Submit the **URL to your commit history**
- Make sure the previous commit is visible and pushed to github
- Add a submission comment saying:

> Taking the break, will finish by Thursday!

*(If you are not taking the break, continue below.)*

---

## Problem 11: The "Boss Level"

**Task:**  
List the titles of episodes from Season 5 that did NOT air in the year 2006.

**Validation:**
- **Columns:** 1 (`title`)
- **Rows:** 1

---

## Problem 12: The "Topic Audit"

**Task:**  
Count the number of unique (distinct) topics in the database. Alias as `unique_topic_count`.

**Validation:**
- **Columns:** 1 (`unique_topic_count`)
- **Rows:** `


---

## Problem 13: The "Curriculum Start"

**Task:**  
List the title of the earliest episode (by air date) that mentions 'Math' in its topic.

**Validation:**
- **Columns:** 1 (`title`)
- **Rows:** 1

**Hint:**  
Compare the `air_date` string.

---


## 🔍 How I Grade Your Work
**Transparency Note:** I verify the **content inside your commits**.
When I view your history, I click on specific commits (e.g., *"Problem 8"*) to ensure the work was actually completed at that step.

**For every commit checkpoint, I check for 3 things:**
1.  **📝 POE (Proof of Effort):** Do I see authenicate effort for each problem in the  `README.md`?
2.  **💻 SQL:** Are the specific queries for that segment present in `p2-q.sql`?
3.  **✅ POW Output:** Does `pow2.txt` show the output results for those specific queries?

*If a commit is empty or missing the associated Notes, SQL, or POW output for that section, points will be deducted.*

---

## 💯 Grading Rubric (100 Points)

**1. Submission URL (10 Points)**
* Did you submit the correct URL to the **folder history** `ps0/cyberchase` 

**2. Commit History (10 Points)**
* Are all required commits present, and do they contain the required **POE + SQL + POW** for that section?
* *Required Commits:*
    * "Problem 8"
    * ...
    * ...
    * "Problem 13"

**3. SQL Source Code (25 Points)**
* Does your final `p2-q.sql` contain the valid SQL syntax for all queries?

**4. Proof of Work Output (15 Points)**
* Does your final `pow2.txt` contain the results **AND** the descriptions?
* *Check:* Did you remember to use `.print` before every query so the output is readable?

**5. Proof of Effort (40 Points)**
* Does your final `README.md` contain all required headers and authenicate attempts?
* *Required Sections:* Problem 8....thru Problem 13.

**6. Scope of Work.**
* Limit your code to the specific SQL concepts covered in this course so far. The goal is to demonstrate your understanding of the current material. Note: Using SQL functions or syntax we haven't covered yet will be flagged as AI-generated code and points will be deducted.  
---

### 🕒 Late Policy
* **Penalty:** Work submitted after the due date receives a **25-point deduction**.
* *Example:* A perfect assignment submitted late will receive **75/100**.