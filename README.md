# NUS Course Work

A personal archive of my university coursework at the **National University of Singapore (NUS)**, grouped by **discipline** and then by **course code**. Each course holds my **notes** and **projects**, written primarily in **LaTeX**.

## Repository structure

```
NUS-Course-Work/
├── templates/                  # Shared LaTeX starting points
│   ├── note-template.tex       # Copy into a course's notes/
│   └── project-template.tex    # Copy into a course's projects/
└── <Discipline>/               # Mathematics, Statistics, QuantitativeFinance, Computing, GeneralEducation
    └── <COURSE_CODE>/          # One folder per course, e.g. MA2101/
        ├── README.md           # Course title + short description
        ├── notes/              # Lecture notes, summaries, cheat sheets (.tex)
        └── projects/           # Assignments, reports, project write-ups (.tex)
```

## Disciplines & courses

### Mathematics
MA1100 Basic Discrete Mathematics · MA2001 Linear Algebra I · MA2002 Calculus · MA2101 Linear Algebra II · MA2104 Multivariable Calculus · MA2108 Mathematical Analysis I · MA2202 Algebra I · MA2213 Numerical Analysis I · MA2214 Combinatorics and Graphs I · MA3211 Complex Analysis I · MA3238 Stochastic Processes I · MA3252 Linear and Network Optimisation · MA4268 Mathematics for Visual Data Processing · MA4270 Data Modelling and Computation · MA4275 Mathematics of Reinforcement Learning

### Statistics
ST2131 Probability · ST2132 Mathematical Statistics · ST3131 Regression Analysis

### QuantitativeFinance
QF1100 Introduction to Quantitative Finance · QF2103 Computing for Quantitative Finance · QF2104 Fundamentals of Quantitative Finance · QF3101 Investment Instruments and Risk Management · QF3103 Advanced Mathematics in Quantitative Finance

### Computing
CS1010S Programming Methodology · DSA1101 Introduction to Data Science · IT1244 Artificial Intelligence: Technology and Impact

### GeneralEducation
CFG1002 Career Catalyst · CFG1003 Financial Wellbeing – Introduction · CFG1004 Financial Wellbeing – Art and Science of Investing · DTK1234 Design Thinking · ES1103 English for Academic Purposes · GEN2062Y Community Activities for Seniors · HS2902 "Do Play Play": The Importance of Play · HSA1000 Asian Interconnections · HSH1000 The Human Condition · HSI1000 How Science Works, Why Science Works · HSS1000 Understanding Social Complexity · SP1541 Communication Practices in Popular Science

> Note: MA2101 (Linear Algebra II) was taken twice — withdrawn (W) in AY2024/25 Sem 2 and retaken (A) in AY2025/26 Sem 1. It lives in a single folder.

## Naming convention

- **Course folder** = the official course code in uppercase, e.g. `MA2101`, `QF3103`, placed under its discipline directory.
- Inside each course, put study material under `notes/` and graded/project work under `projects/`.
- LaTeX source files use lowercase, hyphenated names, e.g. `week-03-graphs.tex`, `assignment-1.tex`.

## Adding a new course

1. Create a folder named after the course code inside the right discipline (e.g. `Mathematics/MA3201/`).
2. Add `notes/` and `projects/` subfolders inside it.
3. Copy a file from `templates/` as your starting point (note the path is now `../../templates/` from inside a course folder).

## Compiling LaTeX

With a TeX distribution installed (e.g. TeX Live / MiKTeX):

```bash
pdflatex your-file.tex
```

## A note on `.gitignore`

Build artifacts (`*.aux`, `*.log`, etc.) are ignored. **Compiled PDFs are ignored by default** — if you want to commit a final PDF for a specific course, add an exception in `.gitignore` (e.g. `!Mathematics/MA2101/projects/report.pdf`).

## ⚠️ Academic integrity

This repository is **public**. Please do not copy graded solutions — sharing or reusing assignment answers may violate NUS academic-integrity policies. Material here is for personal reference and portfolio purposes.
