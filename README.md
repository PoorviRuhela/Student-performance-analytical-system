# Student Performance Analytics System

A Python-based data analytics project that evaluates student academic performance and attendance using **Pandas** and **NumPy**. The notebook performs data-quality checks, calculates student percentages and grades, identifies pass/fail results, and summarizes class and subject performance.

## Table of Contents
- [Overview](#overview)
- [Objectives](#objectives)
- [Key Features](#key-features)
- [Technology Stack](#technology-stack)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Assumptions and Limitations](#assumptions-and-limitations)
- [Future Enhancements](#future-enhancements)
- [Author](#author)

## Overview
The **Student Performance Analytics System** demonstrates how basic data analytics techniques can turn student marks and attendance data into useful insights. It is implemented in a Jupyter-style notebook and can be run in Google Colab.

The analysis covers three subjects: Python, NumPy, and Pandas. It calculates each student's average percentage, assigns a grade, determines a pass/fail status, and produces a summary of overall class performance.

## Objectives
- Inspect and validate the student dataset.
- Calculate student percentages and grades.
- Identify pass/fail outcomes using the project's subject-mark rule.
- Summarize class-level performance.
- Compare average marks across subjects.
- Identify top-performing students and students with attendance below 75%.

## Key Features
- **Dataset overview:** displays dataset dimensions, column names, and data information.
- **Data-quality checks:** checks for missing values, duplicate rows, duplicate student IDs, out-of-range subject marks, and invalid attendance percentages.
- **Percentage calculation:** calculates the mean of the three subject marks for each student.
- **Grade assignment:** assigns a grade based on the calculated percentage.
- **Pass/fail analysis:** evaluates student results based on the marks rule implemented in the notebook.
- **Class performance summary:** reports student count, class average, highest and lowest percentages, and pass/fail counts.
- **Subject comparison:** calculates average marks for Python, NumPy, and Pandas and identifies the highest- and lowest-average subjects.
- **Top performers:** lists the three students with the highest percentages.
- **Attendance review:** identifies students with attendance below 75%.

## Technology Stack
| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data loading, manipulation, and analysis |
| NumPy | Numerical operations and result calculations |
| Google Colab / Jupyter Notebook | Running the analysis |
| CSV | Input dataset format |

## Dataset
The project uses a CSV dataset containing student details, subject marks, and attendance.

| Column | Description |
|---|---|
| `Student_ID` | Student identifier |
| `Name` | Student name |
| `Python_Marks` | Marks in Python |
| `NumPy_Marks` | Marks in NumPy |
| `Pandas_Marks` | Marks in Pandas |
| `Attendance_Percent` | Attendance percentage |
| `Percentage` | Calculated average of the three subject marks |
| `Grade` | Grade assigned from the calculated percentage |
| `Result` | Pass/fail result calculated by the notebook |

`Percentage`, `Grade`, and `Result` are derived fields created during analysis if they are not already present in the source data.

## Methodology
1. Load the CSV file into a Pandas DataFrame.
2. Inspect the dataset structure and check data quality.
3. Calculate each student's percentage from the three subject marks.
4. Assign grades using the thresholds defined in the notebook.
5. Determine pass/fail status using the notebook's implemented rule.
6. Calculate class and subject-level summaries.
7. Identify top performers and students with attendance below 75%.

## Getting Started

### Requirements
- Python 3
- Pandas
- NumPy
- Google Colab or Jupyter Notebook

### Run in Google Colab
1. Upload the notebook and CSV dataset to your Google Colab session.
2. Open the notebook.
3. Locate the CSV-loading cell and update the file path to match the uploaded dataset. For example:

   ```python
   import pandas as pd
   import numpy as np

   df = pd.read_csv('/content/student_performance_20_students.csv')
   ```

4. Run the notebook cells in order from top to bottom.
5. Review the generated data-quality checks, student-level calculations, and summary outputs.

> **Note:** The example CSV filename is illustrative. Use the exact filename of the dataset you upload.

## Project Structure
A suggested repository structure is:

```text
student-performance-analytics/
├── Student_performance_analytical_system.ipynb
├── student_performance_20_students.csv
└── README.md
```

Update the filenames above if your repository uses different names.

## Assumptions and Limitations
- The percentage is calculated as the average of Python, NumPy, and Pandas marks.
- Grade thresholds and pass/fail conditions follow the rules implemented in the notebook.
- Attendance below 75% is flagged for review; this is an analytical threshold used by the project.
- This is a notebook-based analysis project. It does not currently include a deployed web application or an interactive dashboard.
- Data-quality checks identify potential issues; they should not be interpreted as automatic correction of every issue.

## Future Enhancements
- Add charts to visualize marks, grades, and attendance.
- Build an interactive dashboard in Power BI.
- Add student-level filtering and comparison.
- Export summary reports to CSV or PDF.
- Extend the data-cleaning workflow and add automated validation tests.

## Author
**Poorvi Ruhela**

## License
No license has been specified yet. Add a license file if you intend to make the project available for reuse by others.

##This is our internship project
