# Week 9: Devious Delivery - Nested Subqueries & JOINs

## Note on setup
We are will working in the packages database and folder for this week. 

## 1. The Mystery: Devious Delivery
Review the problem context:
> "Good day to you, deliverer of the mail. You might remember that not too long ago I made my way over from the town of Fiftyville. I gave a certain box into your reliable hands and asked you to keep things low. My associate has been expecting the package for a while now. And yet, it appears to have grown wings and flown away. Ha! Any chance you could help clarify this mystery? Afraid there’s no “From” address. It’s the kind of parcel that would add a bit more… quack to someone’s bath times, if you catch my drift."

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
   * Inside your `packages` folder, create a new file named `dd-q.sql` and copy contents of `lost-letter.sql` and remove previous queries.  
   * **Note:** Ensure you update your internal SQL references and bash scripts to point to `pow-dd.txt` so you don't overwrite previous work.
   * **COMMIT MESSAGE:** `Setup Ready`
2. **The Task:**
   * Write a **single nested subquery** to solve the mystery.
   * Document your "proof of effort" (failed attempts or logic changes) in your `README.md` (PoE).
3. **Workflow:**
   * Once working, complete your Git workflow with the message:
   * **COMMIT MESSAGE:** `Devious Delivery nested subquery`

---

## BREAK OPTIONAL  
- If you got this far you can take a break and complete the rest of this work by the Thursday night deadline.  
- To "GET" this break you will submit your commit history for the packages folder now.
- I will do a review and give you feedback.
- If you complete before Thurs morning, then you can submit again your commit history URL and tell me that you are ready for a second review. 

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