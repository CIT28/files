# 💻 CyberChase Part 1 Problem Set (Problem 1 thru 7)

# Setup
## 1. Create your SQL File
* Create a new file named `p1-q.sql` inside your `ps0/cyberchase` folder.
* **Do not** manually copy the old file. Instead, copy the code block below and paste it into your new `p1-q.sql` file.

```sql
-- starting the pow workflow
.mode box
.output '| cat >> pow1.txt'

-- ⬇️ WRITE YOUR QUERIES BELOW THIS LINE ⬇️
-- (Remember to .print 'description' before each query)


-- ⬆️ END OF QUERIES ⬆️

-- changes back to stdout
.output stdout

-- bash command (for reference): sqlite3 cyberchase.db < p1-q.sql
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

```md
# Cyberchase Part 1
```

Then complete your Git workflow in **Terminal 2**.

📌 **Commit message to use:**  
`cyberchase setup ready`

---

# ⚙️ The Workflow (Repeat for **EACH** Problem)

For **every problem** listed below (**1 through 7**), you must perform this exact cycle:

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
- Copy **only** the working SQL query into `p1-q.sql` for the official solution.

---

## 3. ✅ Proof of Work
- In terminal 2 run the POW:
  - `sqlite3 cyberchase.db < p1-q.sql`

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
- Comment out the queries you just wrote in `p1-q.sql`
- Add `--` before each line

## REPEAT FOR EACH PROBLEM

## Problem 1: The Negative Filter

**Task:**  
List the titles of all episodes in Season 1 that do **NOT** contain the word **"The"** in the title.

**Validation:**
- **Columns:** 1 (`title`)
- **Rows:** 21

**Hint:**  
Use `NOT LIKE`.

---

## Problem 2: The Season Premiere

**Task:**  
List the title of the first episode of Season 6.

**Validation:**
- **Columns:** 1 (`title`)
- **Rows:** 1

**Hint:**  
Combine `ORDER BY` with `LIMIT`.

---

## Problem 3: The "Hacker" Audit

**Task:**  
Find the production codes and titles for all episodes that have the word **"Hacker"** in the title, but **exclude** the specific episode titled **"Hackerized!"**.

**Validation:**
- **Columns:** 2 (`production_code`, `title`)
- **Rows:** 5

**Hint:**  
Use a compound condition (`AND`) with a negative check (`!=` or `NOT LIKE`).

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

## Problem 4: The New Year's Pattern

**Task:**  
List the titles of every episode that has ever aired on **New Year's Eve (December 31st)**, regardless of the year.

**Validation:**
- **Columns:** 1 (`title`)
- **Rows:** 1

**Hint:**  
Dates are strings. Pattern match the month and day (`%-MM-DD`).

---

## Problem 5: The "Sniffles" Exclusion

**Task:**  
List all episodes from Season 6 **except** the one titled **"The Sniffles"**.

**Validation:**
- **Columns:** 1 (`title`)
- **Rows:** 10

**Check:**  
Ensure **"The Sniffles"** is **NOT** in your output.

---

## Problem 6: The History Check

**Task:**  
List the titles of all episodes about the topic **"Fractions"** that aired **before the year 2005**.

**Validation:**
- **Columns:** 1 (`title`)
- **Rows:** 1

**Hint:**  
Compare the `air_date` string.

---

## Problem 7: The Clean Count

**Task:**  
Count how many episodes are in Season 2, **excluding** any episodes where the title contains the word **"Hacker"**.

**Requirement:**  
Alias the result column as `clean_episode_count`.

**Validation:**
- **Columns:** 1 (`clean_episode_count`)
- **Rows:** 1
- **Value:** 14

## 🔍 How I Grade Your Work
**Transparency Note:** I verify the **content inside your commits**.
When I view your history, I click on specific commits (e.g., *"Problem 1"*) to ensure the work was actually completed at that step.

**For every commit checkpoint, I check for 3 things:**
1.  **📝 POE (Proof of Effort):** Do I see authenicate effort for each problem in the  `README.md`?
2.  **💻 SQL:** Are the specific queries for that segment present in `p1-q.sql`?
3.  **✅ POW Output:** Does `pow1.txt` show the output results for those specific queries?

*If a commit is empty or missing the associated Notes, SQL, or POW output for that section, points will be deducted.*

---

## 💯 Grading Rubric (100 Points)

**1. Submission URL (10 Points)**
* Did you submit the correct URL to the **folder history** `ps0/cyberchase` 

**2. Commit History (10 Points)**
* Are all required commits present, and do they contain the required **POE + SQL + POW** for that section?
* *Required Commits:*
    * "Problem 1"
    * ...
    * ...
    * "Problem 7"

**3. SQL Source Code (25 Points)**
* Does your final `p1-q.sql` contain the valid SQL syntax for all queries?

**4. Proof of Work Output (15 Points)**
* Does your final `pow1.txt` contain the results **AND** the descriptions?
* *Check:* Did you remember to use `.print` before every query so the output is readable?

**5. Proof of Effort (40 Points)**
* Does your final `README.md` contain all required headers and authenicate attempts?
* *Required Sections:* Problem 1....thru Problem 7.

**6. Scope of Work.**
* Limit your code to the specific SQL concepts covered in this course so far. The goal is to demonstrate your understanding of the current material. Note: Using SQL functions or syntax we haven't covered yet will be flagged as AI-generated code and points will be deducted.  
---

### 🕒 Late Policy
* **Penalty:** Work submitted after the due date receives a **25-point deduction**.
* *Example:* A perfect assignment submitted late will receive **75/100**.