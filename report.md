# Computer Engineering Transfer Planner

## 1. Project Overview

This project is a simple web application that helps students simulate a transfer from one academic program to another. It shows how completed courses from the current program can be mapped to equivalent courses in a target program.

The system is implemented using only HTML, CSS, and JavaScript in a single file, as required by the assignment.

---

## 2. Features

The application includes the following features:

- Displays a full list of courses from the Computer Engineering program
- Shows whether each course is passed or not
- Provides a dropdown menu to select a target program
- Implements a "Transfer" button that generates an equivalency table
- Shows equivalent courses in the selected program
- Uses simple UI styling for readability

---

## 3. Equivalency Algorithm (IMPORTANT PART)

The equivalency between courses is determined using a **rule-based mapping system**.

### Logic:

1. A JavaScript object (`equivalencies`) stores mappings between:
   - Current program courses (keys)
   - Target program courses (values)

2. When the user selects a target program:
   - The system checks each **passed course only**
   - It searches for a matching key in the selected program's mapping

3. If a match is found:
   - The equivalent course name is displayed

4. If no match is found:
   - The system displays `"N/A"`

### Example:

- "Introduction to Programming (ENG)" → "Introduction to Programming"
- "Algorithms and Data Structures (ENG)" → "Algorithms and Data Structures"
- "Computer Organization (ENG)" → "Computer Architecture"

### Important Note:

The system does NOT perform automatic AI-based matching. It uses predefined logic to ensure fast and deterministic results.

---

## 4. System Design

The application is built using:

- HTML → structure
- CSS → styling
- JavaScript → logic

All components are embedded in a single file to meet assignment requirements.

---

## 5. Future Improvements (MOST IMPORTANT SECTION - 5 POINTS)

A major future improvement would be to implement **automatic syllabus-based course matching using AI**.

### Idea:

Instead of manually defining equivalencies, the system could:

1. Load official course syllabi from both programs
2. Extract key information such as:
   - Learning outcomes
   - Topics covered
   - Credits
   - Weekly content structure

3. Use Natural Language Processing (NLP) or AI models to compare similarity between courses

### Possible Algorithm:

- Convert syllabus text into embeddings (vector representation)
- Compute similarity scores between courses
- Match courses with highest similarity above a threshold
- Automatically generate equivalency table

### Benefits:

- Removes manual mapping effort
- More accurate and scalable
- Can support many programs automatically
- Adapts when course content changes

### Conclusion:

AI-based syllabus comparison would significantly improve academic transfer systems by making them automatic, scalable, and more precise.

---

## 6. Conclusion

This project demonstrates how a simple web application can simulate academic program transfer and course equivalency using basic web technologies.