# AI & Machine Learning Internship: Learning Journey

A beginner-friendly collection of my Artificial Intelligence and Machine Learning tasks. It starts with the basics of AI, moves on to handling data with Python, and then to building, evaluating and comparing Machine Learning models.

**Author:** Your Name
**Tools:** Python, Jupyter Notebook, VS Code, NumPy, Pandas, Matplotlib, Scikit-learn

---

## Progress

| Week | Topic | Status |
|------|-------|--------|
| 1 | AI Fundamentals and Python | Completed |
| 2 | Data Handling with Python | Completed |
| 3 | Machine Learning Basics | Completed |
| 4 | ML Algorithms and Model Evaluation | Completed |
| 5 to 6 | Coming soon | In progress |

---

## Week 1: Introduction to AI and Python

- **Task 1:** What AI is, ANI vs AGI vs ASI, AI vs ML vs Deep Learning, real-life uses, advantages and limitations
- **Task 2:** Set up Python, VS Code, Jupyter Notebook, NumPy and Pandas, and ran a first program
- **Task 3:** Python basics (variables, data types, user input, operators) with pass/fail, temperature conversion and age eligibility examples
- **Task 4:** Case study of the **Netflix Recommendation System** (input, processing, output, benefits)
- **Task 5:** A **rule-based chatbot** built with `if-elif` statements

## Week 2: Data Handling and Visualization

- **Task 1:** NumPy arrays, indexing, slicing, shape, math operations, `mean()`, `max()`, `min()`, `sum()`
- **Task 2:** Pandas DataFrames, loading CSV files, filtering rows, selecting columns, basic statistics
- **Task 3:** Data cleaning: missing values, duplicate rows and wrong data types, with before and after analysis
- **Task 4:** Matplotlib charts: bar, line, histogram and scatter plot
- **Task 5 (Mini Project):** Student performance analysis of 120 students

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
- **Task 5 (Mini Project):** **Student Pass/Fail Predictor** with **85%** accuracy on 40 unseen test students. Assignment Score and Previous Marks were the most influential features.

Example prediction:

```
Study Hours: 6
Attendance: 85%
Previous Marks: 72
Assignment Score: 75

Prediction: PASS
```

## Week 4: ML Algorithms and Model Evaluation

- **Task 1:** Report on four algorithms: Logistic Regression, Decision Tree, KNN and Linear Regression (how each works, uses, advantages, limitations)
- **Task 2:** Classification models (Logistic Regression, Decision Tree, KNN) on the **Breast Cancer Wisconsin** dataset (UCI Machine Learning Repository, loaded through scikit-learn)
- **Task 3:** **Linear Regression** to predict student final marks, with actual vs predicted graphs
- **Task 4:** Model evaluation: accuracy, precision, recall, confusion matrix, MAE, MSE, RMSE and R2, plus a comparison table
- **Task 5 (Mini Project):** Student Pass/Fail prediction comparing three models

**Classification results: breast cancer (114 test patients, positive class = Malignant)**

| Model | Accuracy | Precision | Recall | Missed cancers |
|-------|----------|-----------|--------|----------------|
| Logistic Regression | **96.49%** | 97.50% | 92.86% | 3 |
| KNN | 95.61% | 97.44% | 90.48% | 4 |
| Decision Tree | 91.23% | 94.44% | 80.95% | 8 |

Logistic Regression was the best model. For cancer detection, recall is especially important because missing a real cancer is worse than a false alarm.

**Regression results: Linear Regression on student marks (40 test students)**

| MAE | MSE | RMSE | R2 |
|-----|-----|------|----|
| 3.40 | 16.63 | 4.08 | 0.905 |

The model explains about 90% of the variation in final marks, and a typical prediction is off by about 4 marks.

**Mini project results: Student Pass/Fail (80 test students)**

| Model | Accuracy | Precision | Recall |
|-------|----------|-----------|--------|
| Logistic Regression | **88.75%** | 90.91% | 92.59% |
| Decision Tree | 87.50% | 90.74% | 90.74% |
| KNN | 85.00% | 88.89% | 88.89% |

---

## Repository Structure

```
.
├── README.md
├── Week 1/
├── Week 2/
├── Week 3 - AI/
└── Week 4 - AI/
    ├── Project_Report.pdf
    ├── Task1_ML_Algorithms_Report.pdf
    ├── Week4_ML_Project.ipynb
    ├── Dataset.csv
    ├── Student_Marks.csv
    ├── Student_Performance.csv
    ├── charts/
    ├── Screenshots/
    └── README.md
```

Each week's folder holds its report (PDF), notebooks, datasets and screenshots.

---

## Datasets

| Dataset | Used in | Source |
|---------|---------|--------|
| Breast Cancer Wisconsin (Diagnostic) | Week 4, Task 2 | UCI Machine Learning Repository (Wolberg, Street and Mangasarian), loaded via scikit-learn |
| Student datasets (Weeks 2 to 4) | Analysis, regression and Pass/Fail prediction | Practice datasets created for learning (not real student data) |

---

## How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Install the libraries**
   ```bash
   pip install numpy pandas matplotlib scikit-learn jupyter
   ```

3. **Start Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

4. Open any `.ipynb` file and choose **Kernel, then Restart & Run All**.

   The notebooks load their CSV files by file name, so keep each notebook in the same folder as its dataset, or update the path in the `read_csv` line.

---

## Limitations

- The student datasets are small practice datasets, so the results show the workflow and not real-world conclusions.
- Results come from a single train/test split with small test sets, so accuracy can change with a different split. Cross-validation would give a more reliable estimate.
- The cancer model is for learning only and must never replace a doctor.

## What I Learned

- How AI, Machine Learning and Deep Learning relate to each other
- Working with data using NumPy and Pandas, and cleaning messy datasets
- Visualizing data to find patterns
- Why data is split into training and testing sets, and why features are scaled
- How Logistic Regression, Decision Trees, KNN and Linear Regression work
- Why accuracy alone is not enough, and what precision, recall, the confusion matrix and R2 show
- How to compare several models fairly on the same data

---

*Made as part of my 6-week AI internship.*


*Made as part of my AI learning program.*
