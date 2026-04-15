# EDNS 491/492 — Capstone Design I & II

**Colorado School of Mines | Interdisciplinary Engineering Design**

[![Build LaTeX PDFs](https://github.com/professor-duran/Capstone/actions/workflows/build-pdfs.yml/badge.svg)](https://github.com/professor-duran/Capstone/actions/workflows/build-pdfs.yml)
![Built](https://img.shields.io/badge/built-2026--03--24-blue)
![Version](https://img.shields.io/badge/version-v1.0.0-green)

---

## Course Overview

EDNS 491/492 is the two-semester interdisciplinary senior capstone design sequence at Colorado School of Mines. Student teams tackle real-world engineering challenges sponsored by industry and faculty, progressing from problem definition and conceptual design through prototyping, testing, and final delivery. The course emphasizes systems thinking, professional communication, project management, and cross-disciplinary collaboration — preparing graduates to lead complex engineering projects from day one.

---

## Documents

All documents are open educational resources and are automatically rebuilt on every push to `main` via GitHub Actions.

| Document | Description | Download |
|----------|-------------|----------|
| **Course Text** | Comprehensive 22-chapter reference covering the full design process, project milestones, management, and professional practice | [PDF](https://raw.githubusercontent.com/professor-duran/Capstone/main/edns491_course_text.pdf) |
| **Student Guide** | Sprint-by-sprint roadmap with assignments, rubrics, schedules, and operational checklists for both semesters | [PDF](https://raw.githubusercontent.com/professor-duran/Capstone/main/EDNS491_Student_Guide.pdf) |
| **PA Instructor's Guide** | Facilitation playbook for PA instructors — sprint guides, design review scripts, grading guidance, and team dynamics | [PDF](https://raw.githubusercontent.com/professor-duran/Capstone/main/PA_Instructors_Guide.pdf) |

---

## Repository Structure

```
Capstone/
├── .github/workflows/
│   └── build-pdfs.yml                  GitHub Actions CI workflow
│
├── mrd/                                Course Text (modular LaTeX)
│   ├── main.tex                           Driver file
│   ├── preamble.tex                       Packages, colors, custom environments
│   ├── frontmatter/
│   │   ├── how_to_use.tex                 Three-document ecosystem, reading by role
│   │   ├── triage_table.tex               "What Should I Be Reading Right Now?"
│   │   └── lab_safety.tex                 Laboratory and workshop safety
│   ├── chapters/
│   │   ├── ch01.tex – ch06.tex            Part I: The Design Process
│   │   ├── ch07.tex – ch10.tex            Part II: Major Project Milestones
│   │   ├── ch11.tex – ch16.tex            Part III: Project Management and Operations
│   │   ├── ch17.tex – ch20.tex            Part IV: Professional Skills
│   │   └── ch21.tex – ch22.tex            Part V: Safety, Compliance, and Professional Practice
│   └── appendices/
│       ├── glossary.tex                   Glossary of Key Terms (40 entries)
│       ├── fail_patterns.tex              Why Capstone Projects Fail (12 patterns + Health Check)
│       ├── checklists.tex                 Quick Reference Checklists (6 checklists, 69 items)
│       └── references.tex                 References and Further Resources
│
├── student_guide/                      Student Guide (modular LaTeX)
│   ├── EDNS491_Student_Guide.tex          Driver file
│   └── sections/                          25 section files
│       ├── philosophy.tex                 Course philosophy
│       ├── sprint_week.tex                Typical sprint week
│       ├── sdi_sprint0.tex – sdi_sprint6.tex    SDI sprints
│       ├── sdii_sprint7.tex – sdii_sprint14.tex SDII sprints
│       ├── assignments_rubrics.tex        Assignment & rubric reference appendix
│       └── ...                            Operations, checklists, quick references
│
├── pa_guide/                           PA Instructor's Guide (modular LaTeX)
│   ├── PA_Instructors_Guide.tex           Driver file
│   └── sections/                          10 section files
│       ├── overview.tex                   Document ecosystem, PA quick-start
│       ├── role_of_pa.tex                 Responsibilities, authority, time commitment
│       ├── sprint_facilitation.tex        Sprint-by-sprint facilitation notes
│       ├── design_review_facilitation.tex Mock PDR/CDR/FDR scripts
│       ├── common_misconceptions.tex      Student misconceptions by topic
│       ├── grading_guidance.tex           Grade determination, Feedback Loop
│       ├── team_dynamics.tex              Managing teams, escalation paths
│       ├── fdvse_facilitation.tex         FDVSE value assessment facilitation
│       ├── project_health.tex             Health Check as management tool
│       └── track_specific.tex             Build/Paper/Competition track guidance
│
├── edns491_course_text.pdf             Pre-built Course Text (committed by CI)
├── EDNS491_Student_Guide.pdf           Pre-built Student Guide (committed by CI)
├── PA_Instructors_Guide.pdf            Pre-built PA Instructor's Guide (committed by CI)
└── README.md
```

---

## Course Text Structure (22 Chapters)

### Part I: The Design Process
1. **Engineering Design as a Professional Practice** — Capstone vs. coursework, engineering judgment, the contracted design firm model, project tracks (Build, Paper, Competition)
2. **Understanding Your Client and Defining the Problem** — Client kickoff, stakeholder engagement, contextual inquiry, scope negotiation
3. **Requirements Engineering** — Anatomy of good requirements, MoSCoW prioritization, SDRD, traceability
4. **Concept Generation, Selection, and Early Design** — Divergent/convergent ideation, morphological charts, decision matrices, trade studies
5. **Sustainability, Equity, and Societal Impact Assessment** — FDVSE value framework, LEED/ENVISION/DFE/ESJ tools, ethical responsibility
6. **Verification, Validation, and Test Planning** — V&V distinction, TAID methods, lifecycle mapping, test procedure design

### Part II: Major Project Milestones
7. **The Statement of Work and Project Plan** — SOW structure, scope definition, Gantt charts, track-specific SOW considerations
8. **Preliminary Design Review (PDR)** — "Should this design work?" Design gate concept, preparation timeline, review expectations
9. **Critical Design Review (CDR)** — "Will this design work?" Design freeze, detailed design completeness, BOM, manufacturing plan
10. **Final Design Review (FDR) and Design Showcase** — "How well did it work?" V&V results, as-built documentation, lessons learned, showcase poster

### Part III: Project Management and Operations
11. **Hybrid Project Management for Capstone** — Waterfall milestones + Agile sprints, Scrum framework, roles, sprint planning
12. **Fabrication Spaces, Resources, and Manufacturing** — Labriola Innovation Hub, Thorson Center, xWorks bays, InnoHub shop access and training
13. **Team Dynamics, Leadership, and Professional Conduct** — Tuckman model, conflict resolution, leadership roles, professional standards
14. **Budgeting and Financial Management** — Budget creation, contingency planning (15–20%), financial accountability
15. **Purchasing Procedures** — Purchasing workflow, PA approval requirements, vendor selection, tax-exempt documentation
16. **Travel Planning and Policies** — Go/no-go decisions, travel approval timeline, Mines travel policies, competition logistics

### Part IV: Professional Skills
17. **Client Engagement and Management** — Professional services model, communication protocols, scope and timeline management
18. **Professional Communication: Written** — Engineering report structure, technical writing best practices, executive summaries
19. **Professional Communication: Oral** — Design review presentations, narrative arc, slide design, data visualization
20. **Resumes, Interviews, and Career Preparation** — Capstone as career asset, quantifying contributions, interview preparation

### Part V: Safety, Compliance, and Professional Practice
21. **Environmental Health and Safety (EHS)** — Mines EHS framework, hazard identification, 5×5 risk matrix, engineering controls
22. **Professional Ethics, Licensure, and Course Policies** — PE licensure path, NCEES Model Rules, professional responsibility

---

## Student Guide Structure

The Student Guide provides sprint-by-sprint navigation for both semesters:

| Section | Coverage | Course Text Reference |
|---------|----------|----------------------|
| Course Philosophy | Contracted design firm model, independence, the three-document ecosystem | Ch. 1 |
| Project Track Pathways | Paper Track, Competition Track, and Hybrid project deep-dives | Ch. 1, 7, 10 |
| **SDI Sprint 0** | Project Expo, team formation, client kickoff | Ch. 1–2 |
| **SDI Sprint 1** | Project plan, Scrum training, client meeting prep | Ch. 7, 11, 13 |
| **SDI Sprint 2** | Concept generation, trade study, career day | Ch. 4, 20 |
| **SDI Sprint 3** | Concept development, client approval of approach | Ch. 3–4, 17 |
| **SDI Sprint 4** | Functional prototypes, FDVSE assessment, ethics essay | Ch. 5, 12, 22 |
| **SDI Sprint 5** | PDR preparation, mock PDR, PDR execution | Ch. 6, 8, 18–19 |
| **SDI Sprint 6** | Design refinement, SDII handoff, long-lead procurement | Ch. 8, 10 |
| **SDII Sprint 7** | Re-engagement, goal setting, hazard assessment | Ch. 2, 11, 21 |
| **SDII Sprint 8** | CDR report, engineering calculation package, CDR execution | Ch. 6, 9, 14–15 |
| **SDII Sprints 9–11** | Build/test/iterate, broader impacts essay | Ch. 5–6, 12 |
| **SDII Sprints 12–13** | FDR preparation, system V&V, final testing | Ch. 6, 10, 18 |
| **SDII Sprint 14** | FDR, design showcase, documentation, final checkout | Ch. 10, 19 |
| Operations | CFO purchasing, travel, career prep, module checklist, abbreviations | Ch. 14–16, 20 |

---

## PA Instructor's Guide Structure

The PA Guide provides facilitation playbooks for Project Advisors:

| Section | Description |
|---------|-------------|
| Overview & Quick-Start | Document ecosystem, "Your First Week as a PA" checklist |
| The PA Role | Five core responsibilities, authority boundaries, time commitment (~3–5 hrs/week per team) |
| Sprint-by-Sprint Facilitation | Half-page facilitation notes for all 15 sprints with health indicators and red flags |
| Design Review Facilitation | 20-question mock PDR reviewer script, CDR readiness checklist, FDR evaluation criteria |
| Common Student Misconceptions | 2–3 misconceptions per topic area across 7 domains with remediation strategies |
| Grading Guidance | Grade determination process, rubric philosophy, individual differentiation methods |
| Team Dynamics | Tuckman model mapped to sprints, underperformer identification, 4-step escalation path |
| FDVSE Facilitation | Integration with PDR/CDR/FDR gates, guiding questions for all five dimensions |
| Project Health Monitoring | Green/Yellow/Red indicators, productive vs. destructive struggle, documentation debt |
| Track-Specific Guidance | Build, Paper, Competition, and Hybrid track considerations with sprint-by-sprint PA focus |
| Purchasing & Travel Oversight | PA approval workflow, budget tracker review, travel logistics and safety |

---

## Editing Workflow

Each chapter is a self-contained `.tex` file. Edit any file under `mrd/`, `student_guide/`, or `pa_guide/`, commit, and push. GitHub Actions recompiles all three PDFs automatically.

**Fast local build of a single chapter:**
```bash
# Uncomment this line in mrd/main.tex:
#   \includeonly{chapters/ch14}
cd mrd && pdflatex main.tex    # ~5 seconds instead of ~60
```

Re-comment `\includeonly` before pushing.

---

## Building Locally

Requires a TeX Live or MiKTeX installation with `pdflatex`.

```bash
# Course Text (3-pass for TOC and cross-references)
cd mrd && pdflatex main.tex && pdflatex main.tex && pdflatex main.tex

# Student Guide (2-pass)
cd student_guide && pdflatex EDNS491_Student_Guide.tex && pdflatex EDNS491_Student_Guide.tex

# PA Instructor's Guide (2-pass)
cd pa_guide && pdflatex PA_Instructors_Guide.tex && pdflatex PA_Instructors_Guide.tex
```

---

## Built With

- **LaTeX** — Typesetting and document preparation
- **GitHub Actions** — Continuous integration; PDFs rebuild automatically on every push to `main`
- **Modular document architecture** — Each chapter and section is an independent `.tex` file for parallel authoring

---

## Adoption and License

These materials are open educational resources developed at Colorado School of Mines and licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You are free to **share** and **adapt** the materials for any purpose, including commercially, provided you give appropriate credit. See [LICENSE](LICENSE) for full details.

**Suggested attribution:**
> EDS 491/492: Senior Capstone Design course materials by Adam W. Duran, Colorado School of Mines, used under CC BY 4.0. Source: https://github.com/professor-duran/Capstone

Documents are living resources that evolve each semester as the course is refined. If you adopt these materials, I'd love to hear about it -- please reach out so I can learn from your experience.

---

## Author and Contact

**Adam W. Duran** | Assistant Teaching Professor, PE, PMP | Department of Mechanical Engineering | Colorado School of Mines

Email: [aduran@mines.edu](mailto:aduran@mines.edu)
Website: [adamwduran.com](https://adamwduran.com)
