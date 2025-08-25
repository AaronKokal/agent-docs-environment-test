---
title: DOCUMENT EDITING GUIDE
description: Guide for editing and maintaining Markdown documentation, focusing on consistency across projects.
date: 2025-08-24T18:00:00Z
categories:
  - Documentation
tags:
  - Markdown
  - Editing
  - Guide
---

# 📖 DOCUMENT EDITING GUIDE

This guide explains how we **edit and maintain Markdown documentation** in our projects.
It ensures everyone uses the same environment, extensions, and rules — so our docs stay clean, consistent, and future-proof.

## contents

1. **Setup & Environment Preparation**
2. **Requirements (extensions + configs)**
3. **Rules for Maintenance (formatting, structure, images, etc.)**

---

## 1️⃣ Setup & Environment Preparation

1. Clone the repository.
2. Open it in **VS Code (when on Windows, WSL: Ubuntu)**.
3. Install the required extensions listed below.
4. Ensure `.prettierrc` and `.markdownlint.json` exist in the repo:

   * If missing, copy them from another project or ask the agent to generate them.
   * These files define the shared formatting and linting rules.

---

## 2️⃣ Requirements

### VS Code Extensions

* **Markdown All in One** → shortcuts, TOC, better editing.
* **Markdownlint** → checks Markdown style (rules in `.markdownlint.json`).
* **Prettier – Code formatter** → auto-formatting for Markdown & YAML (rules in `.prettierrc`).
* **Front Matter** → sidebar for editing YAML front matter (`--- ... ---`).
* **Path Intellisense** → autocomplete for relative file/image links.
* **YAML (Red Hat)** → schema validation for `mkdocs.yml`.
* **MDX (unifiedjs)** → syntax support for `.mdx` files (Docusaurus).
* **Code Spell Checker** → catch typos.
* **EditorConfig** → consistent indentation, line endings, and whitespace.

### Config Files

* `.prettierrc` → defines formatting rules (e.g., line wrapping, quotes).
* `.markdownlint.json` → defines linting rules (e.g., relaxed line length).

---

## 3️⃣ Rules for Maintenance

### Formatting

* Prettier auto-formats Markdown **on save**.
* Key Prettier setting: `proseWrap: "always"` → avoids giant one-line paragraphs.
* Markdownlint ensures consistent headings, spacing, and lists.
* Common rule relaxations:

  * Disable line-length rule (`MD013`).
  * Allow inline HTML in Markdown (`MD033`).

### Structure

*   All docs live under `/docs`.
*   Use subfolders only when necessary (e.g., `docs/img/` for images).
*   Keep filenames lowercase with underscores, e.g., `project_mission.md`.

### Front Matter

*   All new Markdown files **must** include a YAML front matter block.
*   The required fields and their types are defined in `frontmatter.json`.
*   Consult this file to ensure all new documents have the correct metadata structure.

### Images

* Store all images in `docs/img/`.
* Insert with relative links:

  ```md
  ![Alt text](./img/screenshot.png)
  ```

* For Docusaurus projects: images in `static/img/` can be referenced as `/img/...`.

### Maintenance

* Update `project_structure.md` when the repo layout changes.
* Keep docs concise but complete.
* When logs (`project_logs.md`) grow too large, condense old entries while preserving timestamps.

---

✅ With this setup, everyone contributes to documentation in the same way — making it **consistent, reliable, and easy to maintain** across projects.
