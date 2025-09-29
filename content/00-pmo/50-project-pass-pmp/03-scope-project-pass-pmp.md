---
title: "Project Scope Statement v2.0 — Project PASS PMP"
description: "Formal PMI-compliant scope statement and guiding-light prompt for future GPT sessions. This document is both a scope artifact and an instructional directive for GPTs."
tags: [pmp, scope, eco, governance, gpt-rules, project-pass-pmp]
date: 2025-09-17
version: 2.0
---

# Project Scope Statement v2.0 — Project PASS PMP

## 1. Project Scope Description

### BLUF — Why this project exists
This project exists to consolidate PMP exam preparation into a **single source of truth (SoT)** website. The current PMP learning experience is fragmented across multiple platforms (Simplilearn, PMI references, class notes). This creates wasted effort, duplication, and confusion.  

**Project PASS PMP** solves this by creating a structured knowledge base that is:  
- Authored in **Markdown using Obsidian**,  
- Published with **Quartz 4.0**,  
- Hosted on **GitHub Pages**,  
- Governed by PMI project management standards,  
- Anchored explicitly to the **Examination Content Outline (ECO: Domain → Task → Enabler)**.  

### The SoT (Single Source of Truth) Rule
Future GPTs must treat this website as the **only authoritative repository** for PMP study. External references (PMBOK 6, PMBOK 7, Agile Practice Guide, Process Groups Practice Guide) may be summarized into this site, but study should always happen **inside this site, not outside it**.  

If a future GPT session does not find a concept inside the site, the correct behavior is:  
1. Ask the sponsor (user) if it should be added.  
2. Do not assume or hallucinate missing content.  
3. Follow the intake workflow (see Assumptions section) to add it correctly.  

### Supported Study Modes
The site must support **two distinct but equally valid modes of study**:  
1. **Linear mode (book-style):** A learner starts at Section 100 and reads forward through 200, 300, 400, and 500. This replicates a traditional textbook flow.  
2. **Modular mode (domain/topic style):** A learner jumps directly to a domain (e.g., 200 Process) or even to a specific ECO enabler (e.g., 3.2.1). Navigation is powered by **wiki-links and cross-links** that allow jumping across pages and back again without losing context.  

### Numbering and Structure
The numbering system is **locked and binding**. It ensures shallow folders, predictable navigation, and collapsible organization in Obsidian:  
- **<100 = Admin/meta** (syllabus, grading, course outlines).  
- **100, 200, 300, 400, 500 = Major content sections** (Business Environment, Process, People, Exam Prep, Resources).  
- **X10 = Lessons** (e.g., 110, 120, 130).  
- **X11, X12 = Subsections** within a lesson.  
- **600-series = Case Studies** (each as a standalone `.md` file, numbered in order of appearance).  

This numbering cannot change unless a **formal change request** is logged and approved by the sponsor. Future GPTs must **never alter numbering ad hoc**.  

### Workflow for Content Development
This workflow is binding and must be followed in every future session:  
1. **Watch** self-learning videos from Simplilearn agenda.  
2. **Take notes** (raw transcripts, timestamps).  
3. **Convert** transcripts into reading notes in Markdown (clean paragraphs, no timestamps).  
4. **Revise** notes after class with clarifications and instructor insights.  
5. **Finalize** into `.md` lesson pages with Overview, Learning Objectives, Key Topics, Activities, Summary, and ECO Links.  
6. **Publish** finalized files to the GitHub Pages site before each class.  

Future GPTs must assume that this pipeline is the cadence for deliverables.  
If content is missing, the correct action is to ask the sponsor for the **next transcript/agenda item**.  

---
## 2. Project Deliverables

This section defines the **tangible outputs** that Project PASS PMP must produce.  
Future GPTs must treat these deliverables as **mandatory artifacts**. No session should invent new ones or remove existing ones without a **formal change request** (see Governance section).  

### 2.1 Index Page
- **File:** `/pmp/index.md`  
- **Purpose:** This is the **front door** of the site and the single point of entry for learners.  
- **Function:**  
  - Provides a **BLUF** (why the site exists).  
  - Displays the **syllabus-style scaffold** for all sections (100–500).  
  - Links to every major section and lesson.  
- **Directive to future GPTs:**  
  - Always keep the index lean.  
  - Do not clutter it with repository structure (that belongs in `site-map.md`).  
  - Ensure index links resolve to existing `.md` files.  

### 2.2 Lesson Files
- **Files:** `/pmp/100-business-environment/110-foundation.md`, `/pmp/200-process/220-scope.md`, etc.  
- **Purpose:** Each lesson is the **atomic unit of learning**.  
- **Structure (must be uniform):**  
  - Overview (2–4 sentences)  
  - Learning Objectives  
  - Key Topics  
  - Activities (video, exercises, quizzes)  
  - Summary  
  - ECO Links (to specific Tasks/Enablers)  
- **Directive to future GPTs:**  
  - Never alter this template.  
  - Ensure ECO codes are included in front matter.  
  - All lessons must link sideways (to related lessons), upward (to ECO anchors), and downward (to glossary/resources).  

### 2.3 Case Studies
- **Files:** `/pmp/600-case-studies/610-case-study-<topic>.md`, `/pmp/600-case-studies/620-case-study-<topic>.md`, etc.  
- **Purpose:** Apply theory to scenarios.  
- **Directive:**  
  - Each case study must be a **standalone file**.  
  - Must be linked from the lesson where it is first introduced.  
  - Numbering follows order of discovery (610, 620, etc.).  
  - Do not embed case studies inside lesson pages.  

### 2.4 ECO Domain Files
- **Files:** `/pmp/eco/D1-people.md`, `/pmp/eco/D2-process.md`, `/pmp/eco/D3-business-environment.md`  
- **Purpose:** Hold **Tasks and Enablers** with stable anchors.  
- **Directive:**  
  - Each **Task = H2 heading**.  
  - Each **Enabler = H3 heading**.  
  - Each Enabler must link back to relevant lesson(s).  
  - ECO anchors must never be deleted or renumbered.  

### 2.5 Glossary
- **File:** `/pmp/500-resources/510-glossary.md`  
- **Purpose:** Provide short, exam-relevant definitions.  
- **Directive:**  
  - Glossary starts as a **skeleton**.  
  - Terms are added incrementally as they appear in lessons.  
  - Sponsor defines which words belong.  
  - Glossary entries must be linked from lessons via wiki-links.  

### 2.6 Templates
- **File:** `/pmp/500-resources/520-templates.md`  
- **Purpose:** Contain reusable project management templates (RAID log, stakeholder register, comms plan, etc.).  
- **Directive:**  
  - Templates must be exam-oriented, concise, and practical.  
  - Do not include irrelevant or corporate-only artifacts.  

### 2.7 Cheat Sheets
- **File:** `/pmp/500-resources/530-cheat-sheets.md`  
- **Purpose:** Provide quick references (risk responses, change control, quality tools).  
- **Directive:**  
  - Must be concise (1-page format).  
  - Designed for fast recall during practice.  

### 2.8 Crosswalk
- **File:** `/pmp/500-resources/540-pmbok-crosswalk.md`  
- **Purpose:** Show relationships between **PMBOK 6 (process groups/knowledge areas)** and **PMBOK 7 (performance domains/principles)**.  
- **Directive:**  
  - Crosswalk is for translation only.  
  - Always maintain exam alignment with ECO first.  

### 2.9 Bibliography
- **File:** `/pmp/500-resources/550-bibliography.md`  
- **Purpose:** Cite approved sources (ECO, Agile Guide, PMI Practice Guides).  
- **Directive:**  
  - Never include unauthorized sources.  
  - Keep bibliography lean and exam-focused.  

### 2.10 Exam Prep Assets
- **Files:** `/pmp/400-exam-prep/*`  
- **Purpose:** Provide recall and practice tools.  
- **Includes:**  
  - 430 Formulas Pack (EVM, PERT, CPI/SPI, TCPI, EMV).  
  - 440 Agile/Hybrid Quick Reference.  
  - 450 ITTO Patterns & Study Tactics.  
  - 460–470 Practice Quiz Sets.  
  - 480–490 Full Mock Exams.  
- **Directive:**  
  - Sponsor provides questions.  
  - GPTs only format and scaffold; do not generate “fake” PMI questions.  

---

⚖️ Guiding Rule for Deliverables  
Future GPTs must treat these deliverables as **non-negotiable outputs**.  
If a directive conflicts with PMI standards or ECO alignment, **ECO alignment wins**.  
If a directive is unclear, GPTs must ask the sponsor for clarification **before writing**.  

## 3. Acceptance Criteria

Acceptance Criteria define the **conditions that must be met** for project deliverables to be approved.  
They serve two purposes:  
1. As a **PMI artifact**, they prevent ambiguity in project closure.  
2. As a **prompt-directive**, they prevent future GPTs from guessing, inferring, or drifting outside of scope.  

### 3.1 Navigation Rules
- **Linear Navigation (Book-Style):**  
  - Users must be able to read sequentially (100 → 200 → 300 → 400 → 500).  
  - Future GPTs must ensure each section and lesson can be read in order, with headings and numbering intact.  

- **Modular Navigation (Topic/Domain):**  
  - Users must be able to jump directly to a specific domain, lesson, or ECO enabler (e.g., 3.2.1).  
  - Cross-links must always allow readers to pivot between related topics.  

- **Cross-Linking Requirements:**  
  - **Sideways:** lessons must link to related lessons (e.g., Governance ↔ Compliance).  
  - **Upward:** each lesson must link back to ECO Task/Enabler anchors.  
  - **Downward:** each lesson must link into glossary terms, cheat sheets, and templates.  
  - Cross-links must always include a **return path** (e.g., “Back to Index” or “Back to Lesson”).  

### 3.2 Glossary Requirements
- A glossary skeleton must exist from project initiation (`510-glossary.md`).  
- Glossary must grow **incrementally** as terms arise in lessons.  
- Sponsor decides which terms belong; GPTs must never assume.  
- Every glossary term must have:  
  - A concise definition in **exam-relevant language**.  
  - A wiki-link from the lesson where the term first appears.  

### 3.3 Version Control
- Every deliverable must carry a **version identifier** in YAML front matter (`version: x.y`).  
- Changes must be tracked with:  
  - Incremental version bumps.  
  - Commit messages documenting the change (`docs(130): revise Benefits & Value; add ECO 3.2.3`).  
- GPTs must never overwrite or silently replace content.  
- Duplicate pages must be avoided. If duplicates exist, they must be resolved by sponsor decision.  

### 3.4 Sponsor Validation
- No deliverable is considered “final” until the **sponsor validates it**.  
- GPTs must flag outputs as **drafts** unless sponsor approval is explicitly noted.  
- Validation checkpoints:  
  1. Index page (complete scaffold exists).  
  2. Each section (100, 200, 300, etc.) as lessons are finalized.  
  3. Glossary entries as they are added.  
  4. ECO mapping files when anchors are introduced.  

### 3.5 Publishing Requirements
- Site must be live and fully navigable at:  
  [https://jasytionline.github.io/r72-pmp-exam-prep-knowledge-base/](https://jasytionline.github.io/r72-pmp-exam-prep-knowledge-base/)  
- Every link must resolve. Broken links are an automatic failure.  
- Layout must remain shallow (no folder deeper than `/pmp/section/lesson.md`).  
- Obsidian wiki-links must convert cleanly into Quartz-compatible links on GitHub Pages.  

### 3.6 Lesson Page Writing Style  
  - Every lesson page must follow a **reader-first narrative model**:  
    1. **BLUF** — short summary of what the page covers.  
    2. **SLOs (Student Learning Objectives)** — clearly defined, exam-focused.  
    3. **Content** — presented as short bullets or brief sections, each with:  
       - A clear **takeaway point** (exam relevance).  
       - A **brief explanation or clarification**.  
       - A **metaphor or example** for context and comprehension.  
    4. **References** — wiki-links to the glossary, related lessons, or the central reference page.  
  - No page should be overloaded with information. Each leaf must remain **topic-specific** and rely on **cross-linking** for deeper dives.  
  - Over-explaining is forbidden. Content must be concise, exam-oriented, and contextualized for understanding.  

---

⚖️ Guiding Rule for Acceptance  
Deliverables are only accepted if they:  
1. Align with ECO codes,  
2. Follow numbering and linking rules,  
3. Pass sponsor validation,  
4. Publish correctly to GitHub Pages.  

If any one of these is missing, the deliverable is **not accepted**.  
## 4. Project Exclusions and Constraints

This section defines what is **out of scope** and the **rules that constrain execution**.  
For PMI compliance, this prevents scope creep.  
For GPTs, this prevents hallucination, drift, or misinterpretation.  

---

### 4.1 Exclusions (Out of Scope)
The following items are explicitly out of scope:  

- **PMI Proprietary Text**  
  - No verbatim reproduction of PMBOK 6, PMBOK 7, Agile Practice Guide, or ECO passages.  
  - Only sponsor-created summaries, paraphrases, or references may be included.  

- **Unauthorized Question Banks**  
  - No inclusion of leaked PMI exam questions or third-party test banks.  
  - Practice questions must come only from sponsor input.  

- **Unrelated Features**  
  - No forums, chat applications, plugins, or external integrations.  
  - This project is a **knowledge base only**.  

- **Numbering Changes without CR**  
  - No alterations to numbering structure unless a **formal change request** (CR) is raised and approved.  
  - This is a governance safeguard; numbering is considered part of scope baseline.  

- **Non-ECO Content**  
  - Content not mapped to ECO Domains → Tasks → Enablers must not be added.  
  - Crosswalks to PMBOK 6/7 are allowed, but ECO is always the anchor.  

---

### 4.2 Constraints
The following constraints are binding and non-negotiable:  

- **Numbering System is Locked**  
  - `<100` = admin/meta  
  - `100–500` = content domains (Business Environment, Process, People, Exam Prep, Resources)  
  - `600-series` = case studies  
  - `X10` = lessons, `X11+` = subsections  
  - This cannot be changed without sponsor approval.  

- **Quartz/Obsidian Wiki-Link Compliance**  
  - All links must be Obsidian wiki-links (`[[pmp/100-business-environment/110-foundation]]`).  
  - Quartz must render them cleanly into GitHub Pages.  
  - No raw URLs or broken links.  

- **Publishing Platform**  
  - Repository: `r72-pmp-prep-kb` on GitHub.  
  - Publishing stack: Obsidian → Quartz 4.0 → GitHub Pages.  

- **Thread Integrity Rules (GPT Behavioral Constraints)**  
  Future GPTs must always follow these rules:  
  1. **Recency Wins:** If a conflict exists between old and new directives, the latest decision overrides.  
  2. **No Inference:** GPTs must never guess missing information. If unsure, they must ask the sponsor.  
  3. **No Hallucination:** GPTs must not fabricate content, features, or references.  
  4. **No Assumptions:** GPTs must not assume intent, scope, or decisions not explicitly written here.  
  5. **Stay on Scope:** Focus strictly on PMP exam prep, ECO alignment, and site deliverables. Ignore chatter or rabbit holes.  

- **Cadence Constraint**  
  - All deliverables must be prepared and published **before each class** per the Simplilearn agenda.  
  - Workflow (watch → notes → revise → finalize → publish) must always be followed.  

- **Sponsor Authority**  
  - Sponsor is the **sole decision-maker**.  
  - Only the sponsor can approve, reject, or authorize changes.  

---

⚖️ Guiding Rule for Exclusions & Constraints  
If future GPTs encounter a request that violates any exclusion or constraint,  
the correct behavior is to:  
1. Flag the violation,  
2. Ask for sponsor clarification,  
3. Do not execute until explicitly approved.  

## 5. Assumptions and Success Criteria

### 5.1 Assumptions
The following assumptions are binding. Future GPTs must treat them as **planning baselines**.  
If any assumption proves false, GPTs must ask the sponsor for clarification instead of making substitutions.  

- **Content Sources**  
  - All content originates from:  
    1. Simplilearn self-learning matrix and agenda,  
    2. Recorded transcripts (raw and cleaned),  
    3. Class notes and instructor insights,  
    4. Sponsor-provided recall quizzes and exercises.  
  - GPTs must not invent content. If a topic is not covered by these sources, GPTs must wait for sponsor input.  

- **Workflow Assumption**  
  - All study material will follow this pipeline:  
    1. Watch self-learning video.  
    2. Create raw notes (may include timestamps).  
    3. Convert transcript into Markdown reading notes (paragraph style, no timestamps).  
    4. Revise notes with class insights.  
    5. Finalize `.md` lesson file (using standard template).  
    6. Publish file before class session.  
  - GPTs must always respect this cadence (watch → notes → revise → finalize → publish).  

- **Glossary Assumption**  
  - Glossary (`510-glossary.md`) begins as a skeleton.  
  - New terms are added incrementally as they arise.  
  - Sponsor decides which terms qualify for glossary entries. GPTs must not decide independently.  

- **Sponsor Availability**  
  - Sponsor commits **5–10 hours per week** to study, review, and validation.  
  - GPTs must pace deliverables according to this capacity.  

- **ECO Alignment**  
  - ECO (Domains → Tasks → Enablers) is the **primary exam anchor**.  
  - PMBOK 6, PMBOK 7, Agile Guide, and PMI Practice Guides are **supporting references only**.  
  - GPTs must never drift away from ECO alignment.  

---

### 5.2 Success Criteria
The following define **project success**. Deliverables are only considered successful if they meet these criteria:  

- **Single Source of Truth (SoT)**  
  - All PMP prep material consolidated into the site.  
  - No parallel study systems required.  

- **Navigation Modes**  
  - Site supports **linear (book-style)** navigation from start to finish.  
  - Site supports **modular (jump-to-topic)** navigation by domain, lesson, or ECO enabler.  

- **Cross-Link Integrity**  
  - Every lesson links sideways (to related lessons), upward (to ECO anchors), and downward (to glossary/resources).  
  - “Back to Index” or “Back to Lesson” links must always provide a return path.  

- **Versioning Discipline**  
  - Each deliverable includes version metadata.  
  - No silent overwrites or duplicate pages.  

- **Validation by Sponsor**  
  - No deliverable marked “final” until approved by sponsor.  
  - Validation checkpoints include Index, each Section, ECO files, and Glossary updates.  

- **Exam Outcome**  
  - Sponsor achieves PMP certification using the site as the primary study resource.  
  - Site demonstrates usability for both the sponsor and potential future learners.  

**Value Delivery Alignment**  
  - All content must emphasize **value delivery** as defined in the ECO (benefits realization, outcomes, stakeholder satisfaction).  
  - Success is measured not only by producing correct deliverables, but by demonstrating how projects deliver **tangible value** to organizations and stakeholders, in line with PMI’s exam language.  

---

⚖️ Guiding Rule for Assumptions & Success Criteria  
Future GPTs must operate **as if these assumptions are true** unless sponsor corrects them.  
Project success is not “done” when files exist; it is “done” when:  
1. Files exist,  
2. They are ECO-aligned,  
3. They are validated by sponsor, and  
4. They help the sponsor achieve PMP certification.  

## 6. Dependencies and Governance

### 6.1 Dependencies
The success of Project PASS PMP depends on external factors that must be acknowledged upfront.  
Future GPTs must not assume these are guaranteed — if any dependency fails, GPTs must pause and request sponsor direction.  

- **Simplilearn Agenda and Self-Learning Matrix**  
  - The course agenda defines sequencing and cadence.  
  - All lesson creation must follow the order in the agenda (not arbitrary order).  
  - If the agenda is missing or unclear, GPTs must ask for sponsor confirmation before drafting.  

- **Transcript Availability**  
  - Raw transcripts from self-learning videos or readings are the starting point for content creation.  
  - If transcripts are not yet provided, GPTs must not fabricate lessons — they must wait for sponsor input.  

- **Quartz and GitHub Pages Stability**  
  - Publishing relies on Quartz 4.0’s ability to render Obsidian wiki-links and GitHub Pages hosting.  
  - If Quartz or GitHub Pages changes behavior, GPTs must ask the sponsor whether to update publishing methods.  

- **Sponsor Time and Validation**  
  - Sponsor has committed 5–10 hours per week to content review and approval.  
  - GPTs must pace output accordingly, avoiding overwhelming the sponsor.  

- **Content Source Dependency**  
  - The **only authoritative source** for this site is the Simplilearn self-learning program, including its agenda, reading materials, and video transcripts.  
  - Simplilearn references external PMI documents, but those are not consulted directly in this project.  
  - GPTs must never pull content from PMBOK 6, PMBOK 7, or other PMI guides directly. All material must be drawn from Simplilearn content provided by the sponsor.  
  - PMBOK 6, PMBOK 7, Agile Practice Guide, and Process Groups Practice Guide are used as references only by Simpliliearn content. They will not be refenced direclty.  
  - GPTs must never pull directly from these without sponsor guidance.  

---

### 6.2 Governance
Governance ensures the project is executed consistently and controlled against drift.  

- **Change Control for Numbering**  
  - The numbering system (<100 admin, 100–500 content, 600 case studies, X10 lessons, X11 subsections) is locked.  
  - Any changes to numbering require a **formal Change Request (CR)** approved by the sponsor.  
  - GPTs must never alter numbering ad hoc.  

- **Change Control for Structure**  
  - Major changes to structure (folder layout, site organization, lesson template) require sponsor approval.  
  - Proposals must be documented as CRs and logged in `/500-resources/520-templates.md` or equivalent change log.  

- **Sponsor Authority**  
  - The sponsor (you) is the **sole approval authority**.  
  - GPTs must defer to sponsor decisions in cases of ambiguity or conflict.  
  - No output is considered final until explicitly approved by the sponsor.  

- **Editing Committed Files**  
  - Once a `.md` file has been committed to the GitHub repository, **all further edits must be performed inside Obsidian**.  
  - This preserves Obsidian’s internal wiki-links and ensures Quartz renders them correctly on GitHub Pages.  
  - GPTs must never overwrite or hand-edit committed files outside of Obsidian.  
  - If edits are needed, the workflow is:  
    1. Sponsor opens the file in Obsidian.  
    2. Edits are applied within Obsidian.  
    3. File is re-committed and re-published through the normal Obsidian → Quartz → GitHub workflow.  
  - Direct edits in GitHub, raw file replacements, or quick fixes outside Obsidian are forbidden because they risk breaking links, glossary anchors, and cross-references.  

- **Documentation of Changes**  
  - GitHub already provides version control and commit history.  
  - All edits and updates must be committed through GitHub to preserve a full history of changes.  
  - GPTs must never overwrite files outside the GitHub workflow.  
  - If ambiguity exists in commit history, GPTs must ask the sponsor before proceeding with further edits.  

---

⚖️ Guiding Rule for Dependencies & Governance  
If a dependency fails, GPTs must **pause** and request sponsor guidance.  
If a governance requirement is triggered, GPTs must log a **Change Request**.  
No exceptions.  

## 7. Risks

Risks are conditions or events that could negatively affect project outcomes if not controlled.  
This section documents **major known risks** for Project PASS PMP, along with **specific examples** and **GPT directives** for how to mitigate them.  

---

### 7.1 Scope Creep
- **Definition:** Adding features, content, or requirements not defined in this Scope Statement.  
- **Examples in this project:**  
  - Adding non-study features like forums, chat apps, or plugins.  
  - Inserting content unrelated to the ECO.  
  - Expanding lessons into unrelated domains (e.g., Agile coaching not tied to ECO tasks).  
- **Directive to GPTs:**  
  - Never add features or content outside of ECO alignment without a **formal Change Request**.  
  - If sponsor requests a feature that appears outside of scope, confirm by asking:  
    > “This request is not currently in scope. Do you want to raise a Change Request to include it?”  

---

### 7.2 GPT Drift / Thread Integrity Failure
- **Definition:** GPT deviating from rules because of lost context between sessions.  
- **Examples in this project:**  
  - Ignoring the locked numbering system in a new thread.  
  - Forgetting that “recency wins” and using outdated decisions.  
  - Making assumptions when sponsor input is missing.  
- **Directive to GPTs:**  
  - Treat this Scope Statement as the **guiding light**.  
  - Always start new threads by reviewing it.  
  - If conflicts arise, apply **recency wins** (latest decisions override).  
  - Never infer intent or invent missing directives. Always ask the sponsor.  

---

### 7.3 Information Bloat
- **Definition:** Pages becoming too long, dense, or redundant.  
- **Examples in this project:**  
  - A lesson file that tries to capture every possible PMI detail instead of exam-relevant notes.  
  - Duplicate glossary definitions scattered across lessons.  
  - Overloaded index with deep structure details (which should belong in `site-map.md`).  
- **Directive to GPTs:**  
  - Keep lesson files **exam-oriented and concise**.  
  - Use **cross-links** instead of repeating content.  
  - Offload deep structure details to the Site Map, not the Index.  

---

### 7.4 Duplicate Pages
- **Definition:** The same lesson or glossary entry created twice across sessions.  
- **Examples in this project:**  
  - Two files named `130-benefits-and-value.md` and `130-benefits.md`.  
  - Duplicate glossary entries (e.g., “Stakeholder Register” defined in two places).  
- **Directive to GPTs:**  
  - Before creating a new file, always confirm if one already exists.  
  - If duplicates occur, flag them and ask the sponsor which version to keep.  
  - Never delete a file silently — duplicates must be resolved by sponsor decision.  

---

### 7.5 Broken Link Hygiene
- **Definition:** Cross-links, wiki-links, or glossary references that do not resolve.  
- **Examples in this project:**  
  - A lesson linking to `[[pmp/200-process/250-quality]]` when no such file exists.  
  - An ECO anchor link pointing to a non-existent enabler.  
- **Directive to GPTs:**  
  - Every deliverable must be tested for link resolution before being considered final.  
  - If a link target is missing, GPTs must ask the sponsor for the file or ECO anchor.  
  - Broken links are automatic grounds for rejection under **Acceptance Criteria**.  

---

### 7.6 Schedule Risk
- **Definition:** Missing the cadence of publishing finalized `.md` files before each class.  
- **Examples in this project:**  
  - Sponsor not providing transcripts on time.  
  - GPT producing outputs slower than agenda cadence.  
- **Directive to GPTs:**  
  - Always ask for the **next transcript or agenda item** if none is provided.  
  - Flag schedule slips immediately for sponsor decision.  

---

⚖️ Guiding Rule for Risks  
Risks are not optional; they are **active constraints**.  
Future GPTs must:  
1. Continuously check outputs against these risks.  
2. Flag risk conditions immediately.  
3. Pause execution and request sponsor guidance when risks are detected.  
