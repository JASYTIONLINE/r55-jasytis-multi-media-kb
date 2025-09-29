---
title: "Project Management Plan — Project PASS PMP"
description: "PMI-compliant Project Management Plan tailored for an incremental + agile hybrid study website project."
tags: [pmp, pmi, project-plan, eco, hybrid, obsidian, quartz, github-pages]
date: 2025-09-18
version: 1.0
---

# Project Management Plan — Project PASS PMP

## 1. Introduction & Integration Approach

### Purpose
This Project Management Plan (PMP) integrates the **Project Charter**, the **Scope Statement**, and the **Agenda (Schedule Baseline)** into a single controlling document. It is the guiding reference for executing, monitoring, and closing the **Project PASS PMP** website project.

The PMP ensures:
- All work is traceable to the **Examination Content Outline (ECO: Domain → Task → Enabler)**.  
- Execution follows a **hybrid approach**: predictive for site scaffolding, adaptive for content development.  
- The sponsor (you) has full authority for scope, cadence, and acceptance.  

### Approach
The PMP reflects the **incremental and hybrid nature** of this project:  

- **Phase 1 – Build (Predictive)**  
  Create the structural scaffold of the site: index, syllabus agenda, site map, glossary skeleton, ECO anchor files, and resources.  
  This phase is predictive because the deliverables are fixed, known, and sequenced.  

- **Phase 2 – Fill (Adaptive)**  
  Incrementally populate the scaffold with content derived from Simplilearn videos, transcripts, and course notes.  
  This phase is adaptive because the exact content details evolve as lessons are captured, cleaned, and refined.  

### Tailoring Principle
Per the ECO and PMI guidance, the PMP only includes the **plans, baselines, and controls necessary** to make this project effective. Extraneous sections (e.g., vendor procurement) are excluded unless directly relevant.

### Integration with Existing Artifacts
- **Charter**: Provides purpose, justification, high-level scope, objectives, risks, milestones, and stakeholder roles.  
- **Scope Statement**: Provides locked numbering system, exclusions, assumptions, governance, and acceptance criteria.  
- **Agenda (Schedule Baseline)**: Mirrors the Simplilearn cadence and defines the sprint-like rhythm of updates.  

Together, these artifacts are harmonized in this PMP to ensure execution is both **predictable in structure** and **adaptive in content delivery**.

## 2. Scope Management Plan

### Purpose
The Scope Management Plan defines how the project scope will be **established, validated, and controlled**. It integrates the locked numbering system, exclusions, and acceptance criteria from the Scope Statement into day-to-day execution.

### Scope Definition
- **Baseline Scope** is defined in the approved Scope Statement.  
- Scope is anchored to the **Examination Content Outline (ECO: Domain → Task → Enabler)**.  
- The project consists of two phases:  
  1. **Build (Predictive):** Create the structural scaffold of the site (index, agenda, site map, ECO anchors, glossary skeleton, templates).  
  2. **Fill (Adaptive):** Incrementally populate lessons and resources with content distilled from Simplilearn transcripts and readings.  

### Scope Control
- **Authority:** The Sponsor (you) is the sole authority to approve scope changes.  
- **Change Requests (CRs):** Any adjustment to numbering, structure, or exclusions must be confirmed with the Sponsor before execution. CRs may be noted informally but must be acknowledged explicitly.  
- **Validation:** Each `.md` file (lesson, glossary entry, case study, exam prep asset) must be reviewed and validated by the Sponsor before it is marked “final.”  

### Scope Verification
- **Definition of Done (DoD):**  
  - Each leaf follows the style model: BLUF → Student Learning Objectives → bullets (short explanation + example) → references (wiki-links).  
  - ECO codes are included in front matter and linked to `/eco/` anchors.  
  - Sideways, upward, and downward cross-links are present and functional.  
  - No deliverable is final until Sponsor approval.  

### Out of Scope
The following are explicitly excluded:  
- Verbatim PMI text or proprietary content.  
- Third-party exam question banks.  
- Non-study-site features (forums, chat, apps, integrations).  
- Any lesson or resource not mapped to ECO anchors.  

### Incremental Scope Delivery
- **Predictive Scaffold Build:** Follows the agenda and numbering structure in sequence.  
- **Adaptive Content Fill:** Lessons are drafted, revised, and finalized incrementally in sync with Simplilearn sessions.  
- **Cadence:** Scope deliverables must be published before each class session, per the locked agenda.  

## 3. Schedule Management Plan

### Purpose
The Schedule Management Plan defines how the project’s schedule will be **developed, monitored, and controlled**. The schedule baseline is the **Agenda** (Day 1–20), which mirrors the Simplilearn cadence and provides a sprint-like rhythm for execution.

### Schedule Development
- **Baseline:** The Agenda file (`/500-resources/agenda.md`) is the locked **Schedule Baseline**.  
- **Phases:**  
  1. **Phase 1 – Build (Predictive):** Deliver scaffold pages (index, site map, glossary skeleton, ECO anchors, agenda controller, templates).  
  2. **Phase 2 – Fill (Adaptive):** Incrementally populate lessons, glossary terms, case studies, and exam-prep leaves with content derived from transcripts and readings.  
- **Granularity:** Each class day (Tue–Fri) represents a **micro-sprint** with specific outputs.  

### Monitoring & Control
- **Daily Definition of Done (DoD):**  
  - Draft lesson leaf using BLUF → Student Learning Objectives → bullets (short explanation + example) → references (wiki-links).  
  - Include ECO codes in YAML front matter.  
  - Wire cross-links: sideways (related lessons), upward (ECO anchors), downward (glossary/resources).  
  - Publish via Obsidian → Quartz → GitHub Pages and verify all links resolve.  

- **Weekly Definition of Done (DoD):**  
  - Conduct a **link sweep** to confirm no broken or orphaned links.  
  - Perform an **ECO coverage check** to mark which enablers have been addressed.  
  - Review backlog and carry forward any unfinished work into the next week’s agenda block.  

### Schedule Control
- **Authority:** The Sponsor (you) is the sole authority to modify cadence or reorder topics.  
- **Change Requests:** Any deviation from the Agenda requires explicit Sponsor confirmation.  
- **Tolerance:**  
  - Minor slippage (≤1 day) may be absorbed if the full week’s deliverables are published by Friday.  
  - Major slippages must be logged, reviewed, and resolved before proceeding.  

### Tools & Methods
- **Primary tool:** Agenda (`/500-resources/agenda.md`) is the single controller of schedule commitments.  
- **Execution tools:** Obsidian for drafting, Quartz for publishing, GitHub for version control and tracking.  
- **Reporting:** GitHub commit history and Agenda checkboxes serve as progress reports.  

## 4. Quality Management Plan

### Purpose
The Quality Management Plan defines how deliverables will meet the standards of exam preparation, readability, usability, and site integrity. For Project PASS PMP, quality means that the site is **clear, engaging, user-friendly, and sufficient to prepare a learner to pass the PMP exam**.

### Quality Objectives
- Deliver concise, exam-oriented lesson leaves that follow a consistent structure.  
- Provide enough **information, context, and critical thinking practice** for learners to be exam-ready.  
- Maintain link hygiene: all sideways, upward, and downward links must resolve.  
- Ensure the site is readable, engaging, and navigable for new learners.  
- Publish only Sponsor-validated content as “final.”  

### Standards & Style
Every lesson page must follow the standard **leaf model**:  
1. **BLUF (Bottom Line Up Front):** a short summary of what the page covers.  
2. **Student Learning Objectives (SLOs):** clearly defined, exam-focused outcomes.  
3. **Content:** concise bullets or short sections, each with:  
   - A takeaway point (exam relevance).  
   - A brief explanation or clarification.  
   - A metaphor or example for context and comprehension.  
4. **References:** wiki-links to glossary entries, related lessons, or the central reference page.  

### Quality Assurance
- **Scaffold Quality (Predictive Phase):**  
  - Verify numbering, file naming, and folder layout against the Site Map.  
  - Confirm each scaffold element (index, agenda, glossary, ECO anchors) is present and functional.  
- **Content Quality (Adaptive Phase):**  
  - Verify that every lesson leaf follows the style model.  
  - Confirm ECO codes are included in YAML front matter and link correctly to anchors.  
  - Validate that leaves are readable, user-friendly, and exam-sufficient.  
- **Review Process:**  
  - Sponsor reviews every `.md` file for clarity, relevance, and sufficiency before it is marked final.  

### Quality Control
- **Daily:** Validate each deliverable against the Definition of Done.  
- **Weekly:** Perform link sweeps to ensure no broken or orphaned links; update glossary references as needed.  
- **Phase-End:** Conduct a quality review of completed sections (100, 200, 300, etc.) before moving to the next.  

### Definition of Done (Quality Gate)
A deliverable is considered **done** only when:  
- It is concise, exam-relevant, and aligned to ECO.  
- It provides **sufficient information, context, and practice to support PMP exam readiness**.  
- It follows the BLUF → SLOs → Content → References model.  
- It is user-friendly, navigable, and engaging for new learners.  
- All links resolve (no broken, missing, or circular links).  
- Sponsor validates the file and approves publication.


## 5. Cost Management Plan

### Purpose
The Cost Management Plan defines how project costs will be estimated, budgeted, and controlled.  
For Project PASS PMP, there is **no financial budget** — the only cost baseline is **time and effort**.  

### Cost Baseline
- Sponsor’s weekly commitment of **5–10 hours** is the cost baseline.  
- Tools (Obsidian, Quartz, GitHub Pages) are free and already available.  
- No external procurement or financial spend is planned.  

### Control
- Progress is tracked against the Agenda (schedule baseline).  
- If Sponsor availability drops below 5 hrs/week, a change must be logged and schedule adjusted.  

---

## 6. Communications Management Plan”

### Purpose
The Communications Management Plan defines how project information will be recorded and tracked. Since the Sponsor and Project Manager are the same person, there are no external communications required.

### Communication Methods
- **Progress Tracking:**  
  - GitHub commit history shows all changes and version history.  
  - The Agenda file (`/500-resources/agenda.md`) serves as a checklist of daily/weekly deliverables.  

- **Validation:**  
  - Deliverables are marked “final” only after the Sponsor reviews and approves them.  

### Frequency
- **Daily (micro-sprint):** Update lesson leaf, commit to GitHub.  
- **Weekly:** Perform link sweep, ECO coverage check, and update Agenda checkboxes.  

### Audience
- **Primary Audience:** Sponsor (you).  
- **Secondary Audience:** None.  

### Tools
- Obsidian for drafting.  
- GitHub for version control and progress reporting.  
- Quartz for publishing to GitHub Pages.  

## 7. Risk Management Plan

### Purpose
The Risk Management Plan identifies how risks will be recognized, tracked, and managed during the project. For Project PASS PMP, risks are limited but critical because the project depends on a single sponsor and a fixed cadence.

### Risk Categories
- **Scope Risks** — Adding features or content not aligned to the ECO (scope creep).  
- **Process Risks** — GPT drift, session loss of context, or thread integrity failures.  
- **Content Risks** — Information bloat (pages too long, duplicated, or cluttered).  
- **Schedule Risks** — Falling behind the locked agenda cadence.  
- **Link Hygiene Risks** — Broken or orphaned wiki-links within the site.  

### Risk Management Approach
- **Identification:** Risks are logged during daily/weekly work.  
- **Assessment:** Sponsor evaluates likelihood and impact informally, based on project progress.  
- **Response:**  
  - **Scope creep:** Deny changes unless raised as a Change Request and confirmed by Sponsor.  
  - **GPT drift / thread loss:** Always begin new sessions by re-reading the Scope Statement and PMP.  
  - **Information bloat:** Keep lesson leaves concise and cross-linked instead of overloaded.  
  - **Schedule risk:** Minor slips can be absorbed if the week closes cleanly; major slips must be logged and rescheduled.  
  - **Broken links:** Weekly link sweeps; fix immediately inside Obsidian.  
- **Monitoring:** Risks are reviewed weekly alongside the Agenda backlog.  

### Roles & Authority
- The Sponsor is solely responsible for identifying, assessing, and approving risk responses.  
- AI assistant may flag risks, but Sponsor decides whether action is taken.  

### Purpose
The Stakeholder Engagement Plan defines how stakeholders will be identified, engaged, and managed. For Project PASS PMP, the stakeholder landscape is intentionally simple and limited.

### Stakeholders
- **Primary Stakeholder:** Sponsor / Project Manager (you).  
- **Secondary Stakeholders:** Future learners who may benefit from the site as a study reference.  
- **External Touchpoints:** Education platforms (Simplilearn instructors, support staff).

### Engagement Approach
- **Sponsor Engagement:** Direct and continuous; you validate all deliverables before publication.  
- **Education Platform Engagement:** Handled through support tickets, live class chat, and transcript interactions. Used only to clarify content or resolve questions.  
- **Future Learners:** Not engaged during execution; considered only as passive beneficiaries once the site is complete.

### Monitoring Engagement
- Engagement with external stakeholders is ad hoc and limited to resolving blockers in content development.  
- No formal stakeholder communication plan is required beyond the Sponsor’s validation checkpoints.

## 9. Governance & Change Control

### Purpose
The Governance & Change Control section establishes how the project will be directed, monitored, and controlled. Because this project is executed by a single sponsor (you), governance focuses on preserving structure, integrity, and cadence through strict rules.

### Governance Principles
- **Sponsor Authority:**  
  - The Sponsor is the sole decision-maker.  
  - All scope, numbering, cadence, and acceptance decisions rest exclusively with the Sponsor.  
  - No deliverable is considered “final” without Sponsor validation.  

- **Recency Rule:**  
  - When conflicts arise between older and newer guidance, the most recent directive overrides prior ones.  
  - This ensures that project threads do not drift back to outdated decisions.  

- **No Inference / No Hallucination:**  
  - AI assistants must never invent content, scope rules, or features not explicitly stated.  
  - If a gap exists, they must ask the Sponsor for clarification before proceeding.  

### Change Control
- **Scope Changes:**  
  - Scope is locked to the approved Scope Statement.  
  - Any proposed change must be explicitly confirmed by the Sponsor before execution.  
  - Change Requests (CRs) are informal but must be logged as notes in `/500-resources/520-templates.md`.  

- **Numbering System:**  
  - Numbering (<100 admin, 100–500 content, 600 case studies, X10 lessons, X11 subsections) is locked.  
  - No changes are permitted unless raised as a CR and approved by the Sponsor.  

- **Agenda (Schedule Baseline):**  
  - The Agenda (`/500-resources/agenda.md`) is the controller of cadence.  
  - Dates and sequence are locked to Simplilearn sessions.  
  - Changes must be confirmed by the Sponsor before being applied.  

### Editing Rules
- **Editing Committed Files:**  
  - Once a `.md` file has been committed to the GitHub repository, all further edits must be performed inside **Obsidian**.  
  - This preserves wiki-links, anchors, and Quartz rendering integrity.  
  - Direct edits in GitHub, raw file replacements, or “quick fixes” outside Obsidian are forbidden.  

- **Editing Workflow:**  
  1. Open the file in Obsidian.  
  2. Apply edits, verify cross-links, glossary anchors, and references remain intact.  
  3. Commit via the standard Obsidian → Quartz → GitHub workflow.  

### Validation & Acceptance
- **Validation:** Deliverables are “draft” until reviewed and approved by the Sponsor.  
- **Acceptance:** Approval occurs when the Sponsor marks the deliverable as final and commits it to the working repository.  
- **Revisions:** Any post-commit revisions must follow the Obsidian editing workflow above.  

### Enforcement
If governance rules are violated (e.g., numbering altered, edits made outside Obsidian, unauthorized scope changes), the output is automatically invalid. The Sponsor will decide whether to reject, roll back, or rework the deliverable.

## 9.5 Integration & Performance Control

### Purpose
This section explains how all subsidiary plans (scope, schedule, cost, quality, communications, risk, and governance) are integrated and how overall project performance will be controlled.  
Integration ensures consistency across artifacts, while performance control provides a predictable way to measure progress.

### Integration
- The **Project Management Plan** itself is the integration artifact.  
- It harmonizes the Charter, Scope Statement, and Agenda into a single controlling document.  
- Conflicts between subsidiary plans are resolved by the Sponsor, applying the guiding rules: ECO alignment first, recency wins, and no scope changes without explicit approval.

### Performance Measurement
- **Definition of Done (DoD):** A deliverable is only considered complete when it is published, cross-linked, validated by the Sponsor, and free of broken links.  
- **Daily Control:** Each class day (Tue–Fri) functions as a micro-sprint. Deliverables for that day must be drafted, revised, and published before the next session.  
- **Weekly Control (Friday checkpoint):** Every Friday, performance is measured by verifying that all deliverables scheduled for the week are:  
  1. Complete,  
  2. Published to GitHub Pages,  
  3. Quality-checked (link hygiene, glossary updates, ECO tags verified).  
- **Final Success Metric:** Sponsor achieves PMP certification using this site as the primary preparation resource.

## 10. Baselines & Success Criteria

### Purpose
Baselines establish the reference points for project control, while success criteria define what it means for the project to be complete and effective.

### Baselines
- **Scope Baseline:**  
  - The approved Scope Statement (v2.0) is the scope baseline.  
  - Scope is locked to ECO-aligned deliverables: index, lessons, glossary, ECO anchors, case studies, and exam prep resources.  

- **Schedule Baseline:**  
  - The Agenda (`/500-resources/agenda.md`) is the schedule baseline.  
  - It mirrors the Simplilearn cadence (Day 1–20) and defines the predictive → adaptive workflow.  

- **Cost Baseline:**  
  - The Sponsor’s time commitment of **5–10 hours per week** is the cost baseline.  
  - No direct financial costs are allocated; tools (Obsidian, Quartz, GitHub) are free and already in place.  

### Success Criteria
The project is considered successful when:  
1. **Site Publication:**  
   - The site is live on GitHub Pages, fully navigable, and free of broken links.  
2. **ECO Alignment:**  
   - Every lesson is tagged to ECO codes and cross-linked to the correct domain anchors.  
3. **Lesson Quality:**  
   - All leaves follow the BLUF → SLOs → bullets + example → references style model.  
   - No leaf is overloaded; deeper dives use cross-linking.  
4. **User Experience:**  
   - The site is **user-friendly and navigable for new learners**.  
   - Content reads smoothly, is concise, and keeps readers engaged.  
   - Information is structured for **easy access and convenience**, allowing users to study either linearly or modularly.  
5. **Exam Sufficiency:**  
   - The content provides **enough information, context, and critical thinking practice** for a learner to pass the PMP exam.  
   - Lessons go beyond memorization, reinforcing comprehension and application through ECO-linked examples, cases, and practice assets.  
6. **Validation:**  
   - All deliverables are reviewed and approved by the Sponsor before being marked final.  
7. **Value Delivery:**  
   - The site consolidates all study material into a single source of truth (SoT).  
   - The Sponsor achieves PMP certification using the site as the primary preparation resource.  
   - The site provides long-term utility as a **usable reference source for other learners**.  

### Annex References
For structure and cadence, this plan must always be read together with:  
- [[pmp/site-map|Site Map]] — defines folder layout, numbering, and ECO anchors.  
- [[pmp/500-resources/agenda|Agenda]] — defines the locked cadence and daily/weekly deliverables.  

These references remain in their respective folders and are authoritative controllers for navigation and schedule.
