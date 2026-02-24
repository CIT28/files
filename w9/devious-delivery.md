# Week 9: Devious Delivery - Nested Subqueries & JOINs

## Note on setup
We are will working in the packages database and folder for this week. 

## 1. The Mystery: Devious Delivery
Review the problem context:
> "Deliverer of the mail, I made my way from Fiftyville and handed over a certain box. My associate has been expecting it, but it seems to have grown wings! It’s the kind of parcel that would add a bit more… **quack** to someone’s bath times. Can you find where it was dropped off?"

Unlike the standard CS50 examples, you must write a specific subquery to answer: **"What was the Drop off address?"**

**Expected Output for Nested Subquery:**
<pre>
┌──────────────────┐
│     address      │
├──────────────────┤
│ 7 Humboldt Place │
└──────────────────┘
</pre>

---

## 2. Part A: Nested Subquery
1. **Setup:**
   * In your `README.md`, create a `## Heading 2` titled: `Nested Subquery for Devious Delivery - Proof of Effect`.
   * Inside your `packages` folder, create a new file named `dd-q.sql` and copy `lost-letter.sql` and remove previous queries.  
   * **Note:** Ensure you update your internal SQL references and bash scripts to point to `pow-dd.txt` so you don't overwrite previous work.
   * **COMMIT MESSAGE:** `Setup Ready`
2. **The Task:**
   * Write a **single nested subquery** to solve the mystery.
   * Document your "proof of effort" (failed attempts or logic changes) in your `README.md` (PoE).
3. **Workflow:**
   * Once working, complete your Git workflow with the message:
   * **COMMIT MESSAGE:** `Devious Delivery nested subquery`

---

## 3. Part B: JOIN Query
1. **Setup:**
   * In your `README.md`, create a `## Heading 2` titled: `Join Query for Devious Delivery - Proof of Effect`.
2. **The Task:**
   * Write a `JOIN` query to solve the mystery. 
   * **Note:** The output requirement for the JOIN is different; it must show both the address and the contents.


**Expected Output for JOIN:**
<pre>
┌──────────────────┬─────────────────────┐
│ Drop Off Address │ Contents of Package │
├──────────────────┼─────────────────────┤
│ 7 Humboldt Place │ Duck debugger       │
└──────────────────┴─────────────────────┘
</pre>

3. **Workflow:**
   * Once working, complete your Git workflow with the message:
   * **COMMIT MESSAGE:** `Devious Delivery Join Query`

---

## Grading Rubric (100 Points Total)
| Criteria | Points |
| :--- | :--- |
| **Correct URL** (Packages folder commit history) | 5 pts |
| **Required Commits** (Must match exact messages) | 20 pts |
| **Authentic PoE** (README shows the steps/process) | 45 pts |
| **Correct Output** (From both nested subquery and JOIN) | 30 pts |

> **Late Policy:** Submissions after the deadline incur a **25-point reduction**. Max score for late work is 75/100.