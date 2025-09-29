---
title: "PMP Study Website Intake Interview — Skeleton v1"
description: "Initial intake interview scaffold for PMP exam prep site."
tags: [pmp, eco, intake, skeleton]
date: 2025-09-17
---

# Skeleton Customer Intake Interview (v1)

## A. Extracted Summary
The site is being built as a **single source of truth (SoT)** for PMP exam prep, aligned directly to the **Examination Content Outline (ECO: Domains → Tasks → Enablers)**. It is meant for **self-study learners (you, primarily)** but can also support peers or future students. Users can study the site **linearly, like a book**, or **modularly, by jumping to lessons/domains/glossary**. The structure is **index page → numbered sections (100 Business Environment, 200 Process, 300 People, 400 Exam Prep, 500 Resources) → lessons (X10 pattern) → ECO anchors + glossary cross-links**. Publishing stack is **Obsidian → Quartz → GitHub Pages**. Navigation choices include shallow folder depth, predictable numbering, and a dedicated **Site Map** for structure (kept off the index to avoid clutter). Recent decisions locked in: **ECO-first alignment, cross-linking lessons to ECO domain files, glossary at the end, and SoT rule (all approved sources distilled here, no duplication of PMI books or messy bootcamp UI).**  

## B. Assumptions Not Being Made (Need Confirmation)
- Not assuming your **GitHub repo name/branch structure** for publishing — need confirmation.  
- Not assuming if you want **Prev/Next navigation** on lesson pages, or just Index + wiki links.  
- Not assuming the **cadence of updates** (weekly after class? daily study notes?).  
- Not assuming whether you want **practice questions/recall prompts** embedded in every lesson, or kept only in 400 Exam Prep.  
- Not assuming if **case studies** will be their own section or stay inside lessons.  

## C. Skeleton Interview

### Sponsor & Scope Check
- Problem statement (from you, 1 sentence) → Confirm/Correct: The current PMP study process is fragmented across multiple platforms, so this site will consolidate into one authoritative, ECO-aligned guide. ______  
- Success criteria (bullets) → Confirm/Add:  
  * Fully aligned to ECO (Domains → Tasks → Enablers)  
  * Usable linearly (book-style) and modularly (jump by topic)  
  * Shallow, stable structure (index + lessons + glossary)  
  * Published via GitHub Pages with cross-links and glossary  

### Users & Use Cases
- Primary users / scenarios (bullets) → Confirm/Adjust:  
  * Sponsor (you) as the daily study user  
  * Possible peers/future learners using it as a structured PMP prep guide  

### Content Inputs & Timing
- Source streams (self-learning matrix, transcripts, class notes) → Confirm: ______  
- Weekly pipeline (watch → notes → class → revise → finalize/publish) → Confirm: ______  

### Information Architecture
- **Numbering & Headings Convention**:  
  * Numbers < 100 = Admin/Meta (syllabus, outline, grading, etc.).  
  * 100, 200, 300… = Major sections/domains (render as `##` headings).  
  * 110, 120, 130… = Lessons inside that section (render as `###` headings).  
  * 111, 112, etc. = Sub-points under a lesson (render as `####` headings, deeper as needed).  
  * Structure keeps repo shallow and lets folders accordion open/closed in Obsidian.  
- Sections/lessons numbering (100/200/300/400/500; X10 pattern) → Confirm: ______  
- ECO mapping (D1/D2/D3 with Task/Enabler anchors) → Confirm: ______  
- Cross-linking + glossary placement → Confirm: ______  

### Output Standards
- Lesson template (Overview, Objectives, Key Topics, Activities, Summary, ECO Links) → Confirm/Modify: ______  
- Voice/formatting rules (plain, exam-oriented; no PMI text; relative links) → Confirm: ______  

### Navigation & Publishing
- Index as TOC; separate Site Map; README with live-site link → Confirm: ______  
- GitHub Pages URL shown in README → Confirm: ______  

### Risks & Gaps
- Top 3 risks (e.g., scope creep, missing ECO codes, link hygiene) → Confirm/Prioritize: ______  
- Open questions (list) → Answer: ______  

## D. Next Step Instruction
Please fill in the blanks and confirm/adjust the skeleton fields inline. Once you do, I’ll move to **Step 2: stakeholder engagement** to resolve remaining gaps, then draft a **Formal Customer Request (1 page)** that locks scope, success criteria, information architecture, and cadence.
