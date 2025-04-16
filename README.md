# Leveraging Large Language Models to Identify and Classify Student Errors in Higher Education Mathematics

This repository accompanies the academic paper:  
**"Leveraging Large Language Models to Identify and Classify Student Errors in Higher Education Mathematics Using the STACK Dataset"**  
by *Dogbalou Motognon Wastalas d’Assise, Alex Rodriguez, Danilo Lewanski, Otieno Herine, Prof Lawi, and Michael Kallweit*

---

## 🧠 Overview

This study explores the use of Large Language Models (LLMs), specifically OpenAI’s GPT-4o, to classify student errors in mathematics assessments within the STACK system. It applies **Newman’s Error Analysis (NEA)** framework to categorize student errors into cognitive stages and explores how LLMs can support scalable, personalized feedback in African university classrooms.

---

## 📁 Repository Structure

- `data/`: Contains the anonymized dataset used for LLM-based error classification.
- `notebooks/`: Python notebooks used for data preprocessing, GPT prompting, and classification.
- `README.md`: Project overview and usage instructions.
- `LICENSE`: Licensing information (default MIT, can be customized).
- `.gitignore`: Standard Python ignores.

---

## 🧪 Dataset Description

**File**: `data_students_errors_topic1.csv`  
A curated sample of incorrect student responses from a STACK assessment on "Plane Curves and Parametric Equations".

| Column Name       | Description                                                   |
|-------------------|---------------------------------------------------------------|
| `student_id`      | Unique anonymized identifier                                  |
| `student_response`| Free-text answer given by student                             |
| `right_answer`    | Correct mathematical response                                 |
| `question`        | Identifier for each question                                  |
| `seed_id`         | Unique variant of the question used in randomized quizzes     |
| `grade`           | Normalized score from 0 to 1                                  |
| `llm_response`    | GPT-generated reasoning about the student's mistake           |
| `error_summary`   | Summary of the mistake in short form                          |
| `error_category`  | One of: Reading, Comprehension, Transformation, Process, Encoding|

---

## ⚙️ How to Reproduce

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/LLM-Student-Error-Analysis.git
   cd LLM-Student-Error-Analysis
