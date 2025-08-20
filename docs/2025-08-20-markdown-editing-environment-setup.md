---
title: markdown editing environment setup
description: ""
date: 2025-08-20T17:58:31.405Z
preview: ""
draft: true
tags: []
categories: []
---

# 📖 Documentation Authoring Workflow

This repository uses a `docs/` folder for project documentation.
We edit and maintain it in **Visual Studio Code (WSL)** with a standardized set of extensions and configs.

The goals are:

* Make editing Markdown **easy and pleasant**.
* Keep formatting and style consistent across the team.
* Ensure compatibility with **MkDocs** and **Docusaurus** builds.

---

## 🚀 Setup

1. Clone this repository.
2. Open it in **VS Code (WSL: Ubuntu)**.
3. Install the recommended extensions below.
4. Verify that the repo includes `.prettierrc` and `.markdownlint.json`.

   * If not present, copy them from another project or request them from the team.
   * These files define the shared formatting and linting rules.

---

## 🛠️ Required VS Code Extensions

These are the extensions we standardize on for Markdown docs:

* **Markdown All in One** (`yzhang.markdown-all-in-one`)
  Shortcuts, TOC generation, and editing features for Markdown.

* **Markdownlint** (`davidanson.vscode-markdownlint`)
  Lints Markdown for consistent structure. Rules are configured via `.markdownlint.json` in the repo.

* **Prettier – Code formatter** (`esbenp.prettier-vscode`)
  Auto-formats Markdown and YAML. Configuration is defined in `.prettierrc` (present in the repo).

* **Front Matter** (`eliostruyf.vscode-front-matter`)
  Sidebar UI to edit front matter (`--- ... ---`) in Markdown. Useful for titles, descriptions, and tags.

* **Path Intellisense** (`christian-kohler.path-intellisense`)
  Autocompletes relative file paths when linking images or other docs.

* **YAML** (`redhat.vscode-yaml`)
  Validates and autocompletes `mkdocs.yml` or other YAML configs.

* **MDX** (`unifiedjs.vscode-mdx`)
  Syntax highlighting and validation for `.mdx` files (needed for Docusaurus).

* **Code Spell Checker** (`streetsidesoftware.code-spell-checker`)
  Highlights typos and spelling mistakes in Markdown text.

* **EditorConfig** (`editorconfig.editorconfig`)
  Enforces shared editor settings (indentation, line endings, etc.).

---

## 📂 Repository Structure

```
docs/
  img/         # images for documentation
  intro.md     # example entry point
.prettierrc    # Prettier config (required for consistent formatting)
.markdownlint.json # Markdownlint rules (required for style consistency)
mkdocs.yml     # if MkDocs is used
docusaurus.config.js # if Docusaurus is used
```

---

## 🧹 Formatting & Linting

* **Prettier**:

  * Formats Markdown automatically on save.
  * Rules come from `.prettierrc` (should be in the repo).
  * Key setting: `proseWrap: "always"` → avoids giant one-line paragraphs.

* **Markdownlint**:

  * Ensures headings, spacing, and lists are consistent.
  * Rules come from `.markdownlint.json`.
  * Common relaxations: disable line-length (`MD013`) and allow HTML in Markdown (`MD033`).

If either config file is missing, please set it up before contributing to docs.

---

## 🖼️ Images

* Store images in `docs/img/`.
* Insert with relative links:

  ```md
  ![Alt text](./img/screenshot.png)
  ```
* In Docusaurus projects, `/img/...` from `static/img/` is also supported.