---
title: "Developer README"
description: "Developer-focused README for the JASYTI Multimedia Knowledge Base repo. Explains structure, conventions, and publishing flow."
tags: [developer, readme, repo, quartz, obsidian]
draft: false
date: 2025-09-29
---

# Developer README – JASYTI Multimedia Knowledge Base  

This repository contains the **source vault** for JASYTI’s Multimedia Knowledge Base.  
It is built in **Obsidian**, published via **Quartz 4.0**, and deployed through **GitHub Pages**.  

This README is developer-facing: it documents how the repo is organized and how to maintain/publish it.  

---

## Repo Structure  

- `content/` → The site root. Everything published to GH Pages lives here.  
  - `00-pmo/` → Project Management Office (governance, standards, policies).  
  - `10-platforms/` → YouTube, Twitch, Spotify, Suno AI, etc.  
  - `20-tools/` → Production tools like HitFilm, OBS, Video Express.  
  - `30-portfolio/` → Finished creative works (songs, albums, tutorials, KBs).  
  - `10-sunoai/` → Dedicated sub-KB for Suno AI songwriting and video production.  
- `assets/` → Images, diagrams, supporting media.  
- `LICENSE.md` → Project license.  
- `README.md` (this file) → Developer setup and workflow.  
- `index.md` → Root KB index for site navigation.  

---

## File Naming Conventions  

- All published Markdown files use **Quartz-compatible YAML frontmatter**:  
  ```yaml
  ---
  title: "Page Title"
  description: "Short one-line summary"
  tags: [topic, kb, quartz]
  draft: false
  date: YYYY-MM-DD
  ---
  ```  

- File names are lowercase, hyphenated, and reflect the page purpose:  
  - `suno-guide.md`  
  - `guide-music-video-creation.md`  
  - `example-lyric-sheet-ill-always-remember.md`  

- Index pages for categories are always named `index.md`.  

---

## Linking Conventions  

- **Internal folder links**: use wiki-style links (`[[page-name|Label]]`) inside a KB folder.  
- **Cross-folder or repo-level links**: use GH Pages markdown links `[Label](../path/file.md)` for reliability.  
- **Quick Links** sections → always point to files in the *same folder* (typically `README.md` and `LICENSE.md`).  
- **Navigation Links** sections → connect indexes, glossary pages, and related sub-KBs.  

---

## Workflow  

1. **Authoring**  
   - Use Obsidian locally to draft and cross-link content.  
   - Maintain YAML frontmatter and link format discipline.  

2. **Publishing**  
   - Quartz 4.0 builds from `content/`.  
   - GitHub Actions deploy the compiled static site to GH Pages.  

3. **Maintaining**  
   - Add new KB entries in the appropriate folder (`content/10-sunoai/`, etc.).  
   - Update `index.md` in each category for navigation.  
   - Expand `suno-glossary.md` when new terms appear.  

---

## Development Notes  

- **Consistency** is critical: all KBs should share the same structure (Purpose, How to Use, Main Categories, Quick Links, Navigation Links).  
- **Circular navigation**: every page should let you move laterally (Quick Links) and vertically (Navigation Links).  
- **Version control**: treat `content/` as the single source of truth; don’t keep stray drafts elsewhere.  
- **Future growth**: new categories should follow the `## Main Categories` pattern established in the root index.  

---

## References  

- [Quartz 4.0 Documentation](https://quartz.jzhao.xyz/)  
- [GitHub Pages Docs](https://docs.github.com/en/pages)  
- [Obsidian](https://obsidian.md/)  

---
