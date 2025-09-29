Alright — let’s draft **Sections 1–3** of your **PMI-compliant Project Charter** for *Project PASS PMP*.

---

# Project Charter — Project PASS PMP

## 1. Project Purpose / Justification

The PMP exam preparation process is currently fragmented across multiple vendor platforms, interfaces, and resources. This makes navigation inefficient, creates duplication of effort, and increases the risk of information gaps.

**Project PASS PMP** will consolidate all exam-relevant study material into a **single source of truth (SoT)**: a structured, ECO-aligned study website authored in Obsidian, published with Quartz, and hosted on GitHub Pages. This site will provide an organized, navigable, and reliable study environment that removes the friction of managing multiple learning systems.

The project supports the sponsor’s goal of achieving PMP certification by ensuring that study efforts are focused, traceable to the Examination Content Outline (ECO), and free from the navigational challenges of the current learning platforms.

---

## 2. Measurable Objectives & Success Criteria

**Objectives:**

* Build a **knowledge base website** aligned to the ECO (Domain → Task → Enabler) and cross-referenced to PMBOK 6/7 principles.
* Enable both **linear (book-style)** and **modular (jump-to-topic)** study methods.
* Incorporate cross-links, glossary terms, and case studies into lessons for easy navigation and deeper learning.
* Publish updates consistently before each class session, as defined in the course agenda.

**Success Criteria:**

* Website index provides clear syllabus-style navigation.
* All lessons are tagged to ECO codes and cross-linked to their domain anchors.
* Each lesson follows the standard format (Overview, Objectives, Key Topics, Activities, Summary, ECO Links).
* Glossary is populated incrementally and accessible from lessons and the index.
* GitHub Pages live site is published at [https://jasytionline.github.io/r72-pmp-exam-prep-knowledge-base/](https://jasytionline.github.io/r72-pmp-exam-prep-knowledge-base/) and fully navigable.
* Sponsor validates accuracy and completeness of each lesson before it is marked “final.”

---

## 3. High-Level Project Description

**Scope (Included):**

* Development of a PMP exam prep study site in Markdown, organized by a locked numbering system (<100 admin/meta; 100 Business Environment; 200 Process; 300 People; 400 Exam Prep; 500 Resources).
* Creation of lesson pages (`X10 pattern`) with standardized structure and ECO alignment.
* Establishment of glossary, crosswalk, and case study files linked into lessons.
* Weekly cadence for producing finalized lesson files based on self-learning matrix and class agenda.
* Publishing through GitHub Pages using Quartz/Obsidian wiki-compliant links.

**Out of Scope (Excluded):**

* Copy-pasting proprietary PMI content or third-party question banks.
* Development of non-study-site features (forums, chat, external apps).
* Alteration of the numbering system without a formal change request.

**Key Deliverables:**

* `index.md` with syllabus-style navigation.
* Numbered lesson files (100–500 series) with cross-links to ECO anchors.
* Glossary file (`510-glossary.md`).
* ECO domain files (`/eco/D1-people.md`, `D2-process.md`, `D3-business-environment.md`).
* Case study .md files, linked from lessons in source material sequence.
* Exam prep materials: formulas, ITTO patterns, quizzes, mock exams.

---

# Project Charter — Project PASS PMP

## 4. High-Level Requirements

* The site must be structured around the **PMP Examination Content Outline (ECO)**, with every lesson mapped to Domain → Task → Enabler codes.
* Content will be authored in **Markdown** within **Obsidian**, with **Quartz** ensuring wiki-style links remain functional on GitHub Pages.
* Numbering system is locked (<100 admin/meta, 100+ for content, X10 = lessons, X11+ = subsections). Any changes require a **formal change request**.
* Each lesson must follow a **standard template**: Overview, Learning Objectives, Key Topics, Activities, Summary, ECO Links.
* **Cross-links** between lessons, ECO anchors, glossary, and case studies must be present.
* **Glossary** must exist as a skeleton and expand incrementally as new terms are introduced.
* **Case studies** must exist as separate .md files, linked from lessons where they first appear in the source material.
* All site updates must be **published before each class**, following the cadence defined in the agenda.

---

## 5. High-Level Risks

1. **Scope Creep** — adding features or sections beyond ECO alignment.
2. **Thread Integrity (AI/GPT constraints)** — inconsistencies or drift during session-based content development.
3. **Information Bloat** — individual pages becoming too dense, or duplicate pages created across sessions.
4. **Schedule Risk** — missing the cadence of publishing finalized notes before each class.
5. **Link Hygiene Risk** — broken or misaligned wiki links between lessons, glossary, and ECO anchors.

---

## 6. High-Level Milestones / Schedule Summary

* **Project Initiation (Charter Approved):** September 2025
* **Section 100 (Business Environment) Finalized:** per self-learning agenda timeline
* **Section 200 (Process) Finalized:** per agenda
* **Section 300 (People) Finalized:** per agenda
* **Section 400 (Exam Prep Assets) Available:** before first mock exam session
* **Section 500 (Resources & Glossary) Skeleton Established:** during Section 100 build; updated incrementally
* **Case Studies Added:** as they appear in source material
* **Final Site Walkthrough & Sponsor Approval:** aligned to course end date (TBD by agenda)

---

## 7. High-Level Budget / Resource Summary

This project does not involve direct financial expenditure beyond existing tools. The “budget” is expressed in **time, effort, and existing platforms**:

* **Sponsor/Customer Effort:** 5–10 hours weekly (self-study, transcript conversion, site population).
* **Project Management Tools:** Obsidian, Quartz, GitHub (no cost beyond standard hosting).
* **Supporting References:** PMI ECO, Process Groups Practice Guide, Agile Practice Guide, Simplilearn bootcamp transcripts.
* **Primary Resource Allocation:** Sponsor time for note conversion, GPT assistance for formatting/scaffolding, GitHub repo for hosting/publishing.

---
## 8. Project Approval Requirements  
- **Approval Authority:** The Sponsor (you, as both sponsor and customer) has final approval authority for all project deliverables.  
- **Completion Criteria:**  
  - All lesson files created and cross-linked to ECO anchors.  
  - Glossary skeleton established and populated incrementally.  
  - Case studies documented and linked in source-material order.  
  - Exam Prep section (400-series) populated with formulas, ITTO patterns, quizzes, and mock exams.  
- **Acceptance Criteria:** The site must be published and fully navigable via GitHub Pages, with ECO-aligned content, functional cross-links, and glossary access.  

---

## 9. Assigned Project Manager & Authority Level  
- **Project Manager:** Jasyti (Sponsor/Customer also serving as PM).  
- **Authority Level:**  
  - Full authority to define structure, numbering, and cadence.  
  - Authority to approve or reject deliverables before publication.  
  - Authority to submit change requests for numbering or scope changes.  
  - Authority to coordinate AI/GPT support for scaffolding, formatting, and drafting under controlled constraints.  

---

## 10. Key Stakeholders / Roles  
- **Sponsor & Customer:** Jasyti — sets vision, validates deliverables, and owns the outcome (PMP certification).  
- **Project Manager:** Jasyti — responsible for execution, site population, and cadence adherence.  
- **Supporting Role (AI Assistant):** Provides scaffolding, formatting, intake interviews, and drafting aligned to ECO and PMI standards.  
- **External References/Inputs:**  
  - Simplilearn bootcamp self-learning matrix (primary timeline driver).  
  - PMI references (ECO, Process Groups Practice Guide, Agile Practice Guide, PMBOK 6/7 as needed).  
  - Class instructors and course agenda (secondary drivers for cadence).  

---
