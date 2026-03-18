# Capstone — EDNS 491/492 Capstone Design I & II

**Colorado School of Mines · Interdisciplinary Capstone Engineering Design**

Course materials for the two-semester, multi-disciplinary capstone design sequence.

## Documents

| Document | Description | Pages | Words |
|----------|-------------|-------|-------|
| `main.tex` → `main.pdf` | Student Course Text | 248 | 77,978 |
| `student_guide.tex` → `student_guide.pdf` | Sprint-by-Sprint Student Guide | 16 | 3,027 |

## Repository Structure

```
EDNS491/
├── main.tex                    # Master document (preamble + \input{} calls)
├── student_guide.tex           # Companion sprint-by-sprint guide
├── frontmatter/
│   ├── how_to_use.tex          # Three-document ecosystem, reading by role
│   ├── triage_table.tex        # "What Should I Be Reading Right Now?"
│   └── lab_safety.tex          # Laboratory and workshop safety
├── chapters/
│   ├── ch01.tex                # Engineering Design as a Professional Practice
│   ├── ch02.tex                # Understanding Your Client and Defining the Problem
│   ├── ch03.tex                # Requirements Engineering
│   ├── ch04.tex                # Concept Generation, Selection, and Early Design
│   ├── ch05.tex                # Sustainability, Equity, and Societal Impact
│   ├── ch06.tex                # Verification, Validation, and Test Planning
│   ├── ch07.tex                # The Statement of Work and Project Plan
│   ├── ch08.tex                # Preliminary Design Review (PDR)
│   ├── ch09.tex                # Critical Design Review (CDR)
│   ├── ch10.tex                # Final Design Review (FDR) and Design Showcase
│   ├── ch11.tex                # Hybrid Project Management for Capstone
│   ├── ch12.tex                # Fabrication Spaces, Resources, and Manufacturing
│   ├── ch13.tex                # Team Dynamics, Leadership, and Professional Conduct
│   ├── ch14.tex                # Budgeting and Financial Management
│   ├── ch15.tex                # Purchasing Procedures
│   ├── ch16.tex                # Travel Planning and Policies
│   ├── ch17.tex                # Client Engagement and Management
│   ├── ch18.tex                # Professional Communication — Written
│   ├── ch19.tex                # Professional Communication — Oral
│   ├── ch20.tex                # Resumes, Interviews, and Career Preparation
│   ├── ch21.tex                # Environmental Health and Safety (EHS)
│   └── ch22.tex                # Professional Ethics, Licensure, and Course Policies
├── appendices/
│   ├── glossary.tex            # Appendix A: Glossary of Key Terms (40 entries)
│   ├── fail_patterns.tex       # Appendix B: Why Capstone Projects Fail (12 patterns)
│   ├── checklists.tex          # Appendix C: Quick Reference Checklists
│   └── references.tex          # References and Further Resources
├── .github/
│   └── workflows/
│       └── build.yml           # GitHub Actions CI/CD for PDF compilation
├── .gitignore
└── README.md
```

## Course Text Structure

| Part | Chapters | Focus |
|------|----------|-------|
| I | 1–6 | The Design Process |
| II | 7–10 | Major Project Milestones (SOW, PDR, CDR, FDR) |
| III | 11–16 | Project Management and Operations |
| IV | 17–20 | Professional Skills |
| V | 21–22 | Safety, Compliance, and Professional Practice |
| App A–C | — | Glossary, Fail Patterns + Health Check, Checklists |

## Building Locally

Requires a full TeX Live installation.

```bash
# Course Text (3 passes for TOC/references)
pdflatex main.tex && pdflatex main.tex && pdflatex main.tex

# Student Guide
pdflatex student_guide.tex && pdflatex student_guide.tex && pdflatex student_guide.tex
```

## CI/CD

Every push to `main` triggers a GitHub Actions workflow that compiles both PDFs and uploads them as build artifacts.

## Author

**Adam Duran** · Assistant Teaching Professor, Mechanical Engineering · PE, PMP  
Colorado School of Mines

## License

These materials are proprietary to Colorado School of Mines. All rights reserved.
