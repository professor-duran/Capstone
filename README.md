# EDNS 491/492 — Capstone Design I & II

**Colorado School of Mines · Interdisciplinary Engineering Design**

[![Build LaTeX PDFs](https://github.com/professor-duran/Capstone/actions/workflows/build-pdfs.yml/badge.svg)](https://github.com/professor-duran/Capstone/actions/workflows/build-pdfs.yml)

## Latest Documents

| Document | Download |
|----------|----------|
| **Student Course Text** | [📥 Download PDF](https://raw.githubusercontent.com/professor-duran/Capstone/main/edns491_course_text.pdf) |
| **Student Guide** | [📥 Download PDF](https://raw.githubusercontent.com/professor-duran/Capstone/main/EDNS491_Student_Guide.pdf) |
| **PA Instructor's Guide** | [📥 Download PDF](https://raw.githubusercontent.com/professor-duran/Capstone/main/PA_Instructors_Guide.pdf) |

> PDFs are automatically rebuilt on every push to `main` via GitHub Actions.

## Repository Structure
```
mrd/                                 Course Text (modular LaTeX)
├── main.tex                            Driver file
├── preamble.tex                        Packages, colors, custom environments
├── frontmatter/
│   ├── how_to_use.tex                  Three-document ecosystem, reading by role
│   ├── triage_table.tex                "What Should I Be Reading Right Now?"
│   └── lab_safety.tex                  Laboratory and workshop safety
├── chapters/
│   ├── ch01.tex – ch06.tex             Part I: The Design Process
│   ├── ch07.tex – ch10.tex             Part II: Major Project Milestones
│   ├── ch11.tex – ch16.tex             Part III: Project Management and Operations
│   ├── ch17.tex – ch20.tex             Part IV: Professional Skills
│   └── ch21.tex – ch22.tex             Part V: Safety, Compliance, and Professional Practice
└── appendices/
    ├── glossary.tex                    Glossary of Key Terms (40 entries)
    ├── fail_patterns.tex               Why Capstone Projects Fail (12 patterns + Health Check)
    ├── checklists.tex                  Quick Reference Checklists (6 checklists, 69 items)
    └── references.tex                  References and Further Resources

student_guide/                       Student Guide (modular LaTeX)
├── EDNS491_Student_Guide.tex           Driver file
└── sections/                           25 section files
    ├── philosophy.tex                  Course philosophy
    ├── sprint_week.tex                 Typical sprint week
    ├── sdi_sprint0.tex – sdi_sprint6.tex    SDI sprints
    ├── sdii_sprint7.tex – sdii_sprint14.tex SDII sprints
    ├── assignments_rubrics.tex         Assignment & rubric reference appendix
    └── ...                             Operations, checklists, quick references

pa_guide/                            PA Instructor's Guide (modular LaTeX)
├── PA_Instructors_Guide.tex            Driver file
└── sections/                           10 section files
    ├── overview.tex                    Document ecosystem, PA quick-start
    ├── role_of_pa.tex                  Responsibilities, authority, time commitment
    ├── sprint_facilitation.tex         Sprint-by-sprint facilitation notes
    ├── design_review_facilitation.tex  Mock PDR/CDR/FDR scripts
    ├── common_misconceptions.tex       Student misconceptions by topic
    ├── grading_guidance.tex            Grade determination, Feedback Loop
    ├── team_dynamics.tex               Managing teams, escalation paths
    ├── fdvse_facilitation.tex          FDVSE value assessment facilitation
    ├── project_health.tex              Health Check as management tool
    └── track_specific.tex              Build/Paper/Competition track guidance
```

## Editing Workflow

Each chapter is a self-contained `.tex` file. Edit any file under `mrd/`, `student_guide/`, or `pa_guide/`, commit, push. GitHub Actions recompiles **all three** PDFs automatically.

**Fast local build of a single chapter:**
```bash
# Uncomment this line in mrd/main.tex:
#   \includeonly{chapters/ch14}
cd mrd && pdflatex main.tex    # ~5 seconds instead of ~60
```

Re-comment `\includeonly` before pushing.

## Building Locally
```bash
# Course Text (3-pass for TOC)
cd mrd && pdflatex main.tex && pdflatex main.tex && pdflatex main.tex

# Student Guide (2-pass)
cd student_guide && pdflatex EDNS491_Student_Guide.tex && pdflatex EDNS491_Student_Guide.tex

# PA Instructor's Guide (2-pass)
cd pa_guide && pdflatex PA_Instructors_Guide.tex && pdflatex PA_Instructors_Guide.tex
```

## Author

**Adam Duran** · Assistant Teaching Professor · PE, PMP · March 2026
