# 📚 Documentation Environment Setup

This repository is part of our effort to **standardize Markdown documentation workflows** across all projects in our team.
It provides:

* A **VS Code environment setup** with recommended extensions and formatting rules.
* A **docs framework** that defines core project documentation files.
* An **Agent README** (`AGENT_README.md`) with instructions for AI assistants to maintain and extend our docs automatically.

---

## 🚀 Purpose

The goal is to make working with Markdown files in VS Code:

* **Simple** → easy editing with previews, spell checking, and autocompletion.
* **Consistent** → shared formatting and linting rules across all projects.
* **Extendable** → AI agents can read, maintain, and improve docs with minimal setup.

By adopting this repo structure, every project begins with the same baseline for documentation.

---

## 🛠️ VS Code Setup

To contribute to this repo, please install the recommended VS Code extensions and configs.
These are optimized for **MkDocs** and **Docusaurus** projects, but work for any Markdown-based docs.

### Required Extensions

* **Markdown All in One** – shortcuts, TOC, better editing.
* **Markdownlint** – consistent style (rules in `.markdownlint.json`).
* **Prettier – Code formatter** – auto-formatting (rules in `.prettierrc`).
* **Front Matter** – GUI for editing YAML front matter.
* **Path Intellisense** – autocomplete file/image links.
* **YAML (Red Hat)** – schema support for `mkdocs.yml`.
* **MDX (unifiedjs)** – `.mdx` syntax support (for Docusaurus).
* **Code Spell Checker** – catch typos.
* **EditorConfig** – shared editor settings.

### Config Files

This repo either includes or expects:

* `.prettierrc` → formatting rules for Markdown/YAML.
* `.markdownlint.json` → linting rules (relaxed where necessary).

If missing, copy them from another project before contributing.

---

## 📖 Agent Workflow

See [`AGENT_README.md`](./AGENT_README.md) for details.

This special README defines the files every project must include in `docs/` (e.g., `project_mission.md`, `project_structure.md`, `project_logs.md`).
AI agents should use it as the entry point to check, create, and maintain these files.

---

## 📂 Repo Structure

```bash
README.md          # Human-readable instructions (this file)
AGENT_README.md    # Instructions for AI agents
docs/
  project_mission.md
  project_stack.md
  project_structure.md
  project_logs.md
  project_considerations.md
  ...
```

---

## ✅ Summary

This repo is the **foundation of our docs framework**:

* Every project starts with the same `docs/` structure.
* VS Code is set up with a consistent toolchain.
* AI agents can automatically maintain project documentation.

By following this standard, we make our documentation **uniform, reliable, and easier to maintain** across all future projects.
