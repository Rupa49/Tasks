# AI Fundamentals: Learning Journey (Weeks 1 to 3)

A beginner-friendly collection of my Artificial Intelligence and Machine Learning tasks, moving from the basics of AI, to handling data with Python, to building a first Machine Learning model.

**Author:** Your Name
**Tools:** Python, Jupyter Notebook, VS Code, NumPy, Pandas, Matplotlib, Scikit-learn

---

## Project Overview

| Week | Topic | What I built |
|------|-------|--------------|
| 1 | AI Fundamentals and Python | Intro to AI report, environment setup, Python programs, Netflix case study, rule-based chatbot |
| 2 | Data Handling with Python | NumPy, Pandas, data cleaning, Matplotlib charts, student performance analysis |
| 3 | Machine Learning Basics | ML concepts report, dataset preparation, train-test split, Logistic Regression model, Pass/Fail predictor |

---

## Week 1: Introduction to AI and Python

- **Task 1:** What AI is; ANI vs AGI vs ASI; AI vs ML vs Deep Learning; real-life uses; advantages and limitations
- **Task 2:** Installed Python, VS Code, Jupyter Notebook, NumPy and Pandas, and ran a first program
- **Task 3:** Python basics (variables, data types, user input, operators) using pass/fail, temperature conversion and age eligibility examples
- **Task 4:** Case study of the **Netflix Recommendation System** (input, processing, output, benefits)
- **Task 5:** A **rule-based chatbot** built with `if-elif` statements

## Week 2: Data Handling and Visualization

- **Task 1:** NumPy arrays, indexing, slicing, shape, math operations, `mean()`, `max()`, `min()`, `sum()`
- **Task 2:** Pandas DataFrames, loading CSVs, filtering rows, selecting columns, basic statistics
- **Task 3:** Data cleaning: missing values, duplicate rows and wrong data types, with before and after analysis
- **Task 4:** Matplotlib charts: bar, line, histogram and scatter plot
- **Task 5 (Mini Project):** Student performance analysis on 120 students

**Key findings from the mini project**

| Metric | Result |
|--------|--------|
| Average marks | 47.37 |
| Highest / Lowest | 76.0 / 13.3 |
| Passed / Failed | 89 / 31 |
| Study hours vs marks correlation | 0.85 (strong) |

Students who studied more hours scored clearly higher marks, while gender made almost no difference.

## Week 3: Machine Learning Basics

- **Task 1:** Report on ML fundamentals: features and labels, training and testing data, supervised vs unsupervised learning, classification vs regression
- **Task 2:** Dataset preparation: loading, checking, filling missing values, separating `X` and `y`
- **Task 3:** Train-test split (80/20) and feature scaling with `StandardScaler`
- **Task 4:** First ML model using **Logistic Regression**
- **Task 5 (Mini Project):** **Student Pass/Fail Predictor**

**Mini project details**

- **Features:** Study Hours, Attendance, Previous Marks, Assignment Score
- **Target:** Result (Pass or Fail)
- **Model:** Logistic Regression (a Decision Tree was tried for comparison)
- **Accuracy:** **85%** on 40 unseen test students
- **Most influential features:** Assignment Score and Previous Marks

Example prediction:

```
Study Hours: 6
Attendance: 85%
Previous Marks: 72
Assignment Score: 75

Prediction: PASS
```

---

## Repository Structure

```
.
├── README.md
├── requirements.txt
├── Week 1/
│   └── Week_1.pdf
├── Week 2/
│   ├── week_2.pdf
│   ├── notebooks/
│   ├── datasets/
│   └── charts/
└── Week 3 - AI/
    ├── Week3_Report.pdf
    ├── Week3_ML.ipynb
    ├── Dataset.csv
    ├── Screenshots/
    └── Mini_Project/
```

---

## How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Install the libraries**
   ```bash
   pip install -r requirements.txt
   ```

3. **Start Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

4. Open any `.ipynb` file and choose **Kernel, then Restart & Run All**.

   The notebooks load their CSV files by file name, so keep each notebook in the same folder as its dataset or update the path in the `read_csv` line.

To run the command-line predictor from Week 3:

```bash
cd "Week 3 - AI/Mini_Project"
python student_pass_fail_predictor.py
```

---

## Notes

- The datasets are small **practice datasets** created for learning, so the results show the workflow and not real-world conclusions.
- The model is trained on limited data, so accuracy may change with a different split or a larger dataset.

## What I Learned

- How AI, Machine Learning and Deep Learning relate to each other
- Working with data using NumPy and Pandas, and cleaning messy datasets
- Visualizing data to find patterns
- Why data is split into training and testing sets
- Building, training and evaluating a first Machine Learning model

## Future Improvements

- Use a larger, real-world dataset
- Try more models (Random Forest, KNN) and compare them
- Add cross-validation, precision and recall
- Build a small web app for the Pass/Fail predictor

---

*Made as part of my AI learning program.*
