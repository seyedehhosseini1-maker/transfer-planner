# Computer Engineering Transfer Planner

## 1. Project Overview

This project is a simple web application that helps students understand how courses from Computer Engineering could be transferred to other programs.

It shows a list of courses (passed, failed, and in progress) and lets the user select a target program. After clicking the "Transfer" button, it displays possible equivalent courses in that program.

The whole project is built using only HTML, CSS, and JavaScript in a single file, as required in the assignment.

---

## 2. How Course Matching Works

The equivalency part is done using a simple mapping in JavaScript.

Basically, each course from my program is matched with a similar course in another program using a predefined object (like a dictionary).

When the user clicks the button:
- Only passed courses are considered
- The program checks if a match exists in the selected program
- If yes, it shows the equivalent course
- If not, it shows "N/A"

It is a simple rule-based system, not an automatic one.

---

## 3. Possible Future Improvement

One improvement that could make this project much more powerful is using AI to match courses automatically.

Instead of manually writing equivalencies, the system could read course syllabi and compare them.

For example:
- It could extract topics from course descriptions
- Compare similarity between courses using NLP methods
- Turn course descriptions into vectors and calculate similarity
- Then suggest matches automatically based on highest similarity

This would make the system more flexible and reduce manual work a lot.

---

## 4. Final Note

This project is a basic prototype of a transfer system, showing how course equivalency can be represented in a simple web application.
