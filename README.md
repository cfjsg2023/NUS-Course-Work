# NUS Course Work

A personal archive of my university coursework at the **National University of Singapore (NUS)**, organized by **course code**. Each course holds my **notes** and **projects**, written primarily in **LaTeX**.

## Repository structure

```
NUS-Course-Work/
├── templates/                 # Shared LaTeX starting points
│   ├── note-template.tex      # Copy into a course's notes/
│   └── project-template.tex   # Copy into a course's projects/
└── <COURSE_CODE>/             # One folder per course, e.g. CS2040/
    ├── README.md              # Course title + short description
    ├── notes/                 # Lecture notes, summaries, cheat sheets (.tex)
    └── projects/              # Assignments, reports, project write-ups (.tex)
```

## Naming convention

- **Course folder** = the official course code in uppercase, e.g. `CS2040`, `MA1521`, `EC1101E`.
- Inside each course, put study material under `notes/` and graded/project work under `projects/`.
- LaTeX source files use lowercase, hyphenated names, e.g. `week-03-graphs.tex`, `assignment-1.tex`.

## Adding a new course

1. Create a folder named after the course code (e.g. `ST2334/`).
2. Add `notes/` and `projects/` subfolders inside it.
3. Copy a file from `templates/` as your starting point.

(There's no automation required — just mirror the structure of an existing course.)

## Compiling LaTeX

With a TeX distribution installed (e.g. TeX Live / MiKTeX):

```bash
pdflatex your-file.tex
```

## A note on `.gitignore`

Build artifacts (`*.aux`, `*.log`, etc.) are ignored. **Compiled PDFs are ignored by default** — if you want to commit a final PDF for a specific course, add an exception in `.gitignore` (e.g. `!CS2040/projects/report.pdf`).

## ⚠️ Academic integrity

This repository is **public**. Please do not copy graded solutions — sharing or reusing assignment answers may violate NUS academic-integrity policies. Material here is for personal reference and portfolio purposes.
