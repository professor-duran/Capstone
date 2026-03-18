# EDNS 491/492: Capstone Design I & II — Course Materials

[![Build Capstone PDFs](https://github.com/professor-duran/Capstone/actions/workflows/build.yml/badge.svg)](https://github.com/professor-duran/Capstone/actions/workflows/build.yml)

**Author:** Adam Duran, PE, PMP  
**Institution:** Colorado School of Mines, Interdisciplinary Engineering Design  
**Term:** Spring 2026  

---

## Download PDFs

| Document | Description | Link |
|---|---|---|
| **Student Course Text** | 248-page comprehensive reference covering the engineering design process, project milestones, hybrid project management, professional skills, safety, and ethics for the two-semester capstone sequence | [**Download PDF**](main.pdf) |
| **Student Guide** | 16-page sprint-by-sprint companion with top priorities, common pitfalls, checklists, and quick references for each sprint | [**Download PDF**](student_guide.pdf) |

PDFs are auto-compiled by GitHub Actions on every push and committed to this branch.

---

## Repository Structure

```
Capstone/
├── main.tex                         Build entry point (preamble + \input{} calls)
├── student_guide.tex                Sprint-by-sprint companion guide
├── frontmatter/
│   ├── how_to_use.tex               Three-document ecosystem, reading by role
│   ├── triage_table.tex             "What Should I Be Reading Right Now?"
│   └── lab_safety.tex               Laboratory and workshop safety
├── chapters/
│   ├── ch01.tex                     Engineering Design as a Professional Practice
│   ├── ch02.tex                     Understanding Your Client and Defining the Problem
│   ├── ch03.tex                     Requirements Engineering
│   ├── ch04.tex                     Concept Generation, Selection, and Early Design
│   ├── ch05.tex                     Sustainability, Equity, and Societal Impact
│   ├── ch06.tex                     Verification, Validation, and Test Planning
│   ├── ch07.tex                     The Statement of Work and Project Plan
│   ├── ch08.tex                     Preliminary Design Review (PDR)
│   ├── ch09.tex                     Critical Design Review (CDR)
│   ├── ch10.tex                     Final Design Review (FDR) and Design Showcase
│   ├── ch11.tex                     Hybrid Project Management for Capstone
│   ├── ch12.tex                     Fabrication Spaces, Resources, and Manufacturing
│   ├── ch13.tex                     Team Dynamics, Leadership, and Professional Conduct
│   ├── ch14.tex                     Budgeting and Financial Management
│   ├── ch15.tex                     Purchasing Procedures
│   ├── ch16.tex                     Travel Planning and Policies
│   ├── ch17.tex                     Client Engagement and Management
│   ├── ch18.tex                     Professional Communication — Written
│   ├── ch19.tex                     Professional Communication — Oral
│   ├── ch20.tex                     Resumes, Interviews, and Career Preparation
│   ├── ch21.tex                     Environmental Health and Safety (EHS)
│   └── ch22.tex                     Professional Ethics, Licensure, and Course Policies
├── appendices/
│   ├── glossary.tex                 Glossary of Key Terms (40 entries)
│   ├── fail_patterns.tex            Why Capstone Projects Fail (12 patterns + Health Check)
│   ├── checklists.tex               Quick Reference Checklists (6 checklists, 69 items)
│   └── references.tex               References and Further Resources
├── .github/workflows/               GitHub Actions auto-build
├── main.pdf                         ← auto-built by CI
└── student_guide.pdf                ← auto-built by CI
```

---

## Document Structure

### Front Matter
- How to Use This Document (three-document ecosystem, reading by role)
- What Should I Be Reading Right Now? (triage table, sprint-to-chapter mapping)
- Laboratory and Workshop Safety

### Part I: The Design Process
1. Engineering Design as a Professional Practice
2. Understanding Your Client and Defining the Problem
3. Requirements Engineering
4. Concept Generation, Selection, and Early Design
5. Sustainability, Equity, and Societal Impact Assessment
6. Verification, Validation, and Test Planning

### Part II: Major Project Milestones
7. The Statement of Work and Project Plan
8. Preliminary Design Review (PDR)
9. Critical Design Review (CDR)
10. Final Design Review (FDR) and Design Showcase

### Part III: Project Management and Operations
11. Hybrid Project Management for Capstone
12. Fabrication Spaces, Resources, and Manufacturing
13. Team Dynamics, Leadership, and Professional Conduct
14. Budgeting and Financial Management
15. Purchasing Procedures
16. Travel Planning and Policies

### Part IV: Professional Skills
17. Client Engagement and Management
18. Professional Communication — Written
19. Professional Communication — Oral
20. Resumes, Interviews, and Career Preparation

### Part V: Safety, Compliance, and Professional Practice
21. Environmental Health and Safety (EHS)
22. Professional Ethics, Licensure, and Course Policies

### Appendices
- A: Glossary of Key Terms (40 entries)
- B: Why Capstone Projects Fail (12 patterns + Project Health Check)
- C: Quick Reference Checklists (Sprint 0, SOW, PDR, CDR, FDR, Final Checkout)

---

## Editing Workflow

Each chapter is a self-contained `.tex` file. Edit any file under `chapters/`, `frontmatter/`, or `appendices/`, commit, push. GitHub Actions recompiles **both** PDFs automatically.

```bash
# Edit a chapter
vim chapters/ch14.tex

# Commit just the changed file
git add chapters/ch14.tex
git commit -m "Ch 14: Update budget guidance for Spring 2027"
git push
```

## Building Locally

**Prerequisites:** TeX Live (full) or MacTeX

```bash
# Course Text (3 passes for TOC/references)
pdflatex main.tex && pdflatex main.tex && pdflatex main.tex

# Student Guide
pdflatex student_guide.tex && pdflatex student_guide.tex && pdflatex student_guide.tex
```

## Zero Textbook Cost (ZTC)

All 20 figures are generated inline using TikZ. No external image files are required. The document compiles from source on any system with a standard TeX Live installation.
