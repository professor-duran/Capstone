# EDNS 491/492 — Capstone Design I & II

**Colorado School of Mines · Interdisciplinary Engineering Design**

[![Build LaTeX PDFs](https://github.com/professor-duran/Capstone/actions/workflows/build.yml/badge.svg)](https://github.com/professor-duran/Capstone/actions/workflows/build.yml)

## Latest Documents

| Document | Download |
|----------|----------|
| **Student Course Text** | [📥 Download PDF](https://raw.githubusercontent.com/professor-duran/Capstone/main/main.pdf) |
| **Student Guide** | [📥 Download PDF](https://raw.githubusercontent.com/professor-duran/Capstone/main/student_guide.pdf) |

> PDFs are automatically rebuilt on every push to `main` via GitHub Actions.

## Repository Structure
```
main.tex                             Build entry point (preamble + \input{} calls)
student_guide.tex                    Sprint-by-sprint companion guide

frontmatter/                         Front matter (modular LaTeX)
├── how_to_use.tex                      Three-document ecosystem, reading by role
├── triage_table.tex                    "What Should I Be Reading Right Now?"
└── lab_safety.tex                      Laboratory and workshop safety

chapters/                            22 chapters across 5 parts
├── ch01.tex – ch06.tex                 Part I: The Design Process
├── ch07.tex – ch10.tex                 Part II: Major Project Milestones (SOW, PDR, CDR, FDR)
├── ch11.tex – ch16.tex                 Part III: Project Management and Operations
├── ch17.tex – ch20.tex                 Part IV: Professional Skills
└── ch21.tex – ch22.tex                 Part V: Safety, Compliance, and Professional Practice

appendices/                          Back matter
├── glossary.tex                        Glossary of Key Terms (40 entries)
├── fail_patterns.tex                   Why Capstone Projects Fail (12 patterns + Health Check)
├── checklists.tex                      Quick Reference Checklists (6 checklists, 69 items)
└── references.tex                      References and Further Resources
```

## Building Locally
```bash
# Course Text (3-pass for TOC)
pdflatex main.tex && pdflatex main.tex && pdflatex main.tex

# Student Guide (2-pass)
pdflatex student_guide.tex && pdflatex student_guide.tex
```

## Author

**Adam Duran** · Assistant Teaching Professor · PE, PMP · March 2026
