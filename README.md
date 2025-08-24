# 📚 Documentation Framework

This repository defines our **standardized documentation workflow** for all future projects.

It provides:

* A **docs framework** that defines the required documentation files every project must maintain.
* An **Agent README** (`framework/AGENT_README.md`) with instructions for AI assistants to manage and extend project documentation.
* A **DOCUMENT EDITING GUIDE** (`framework/DOCUMENT_EDITING_GUIDE.md`) with setup and maintenance rules for contributors working in their respective IDE.

---

## 🚀 Purpose

The goal is to make project documentation:

* **Simple** → clear structure and required files.
* **Consistent** → every project starts with the same baseline.
* **Extendable** → AI agents can read, maintain, and improve docs automatically.

By adopting this framework, documentation becomes **uniform, reliable, and easy to maintain** across all projects.

---

## 📖 Docs Framework

Project-specific documentation lives in the `docs/` folder.
These are living documents that accumulate content over time:

* `project_mission.md` → explains the **why** of the project (goals, outcomes, pain points).
* `project_stack.md` → lists **tooling and architecture** decisions.
* `project_structure.md` → shows the repo’s tree structure with short explanations.
* `project_logs.md` → project diary with milestones, decisions, and reasoning.
* `project_considerations.md` → captures future ideas, alternatives, and deferred decisions.

## ⚙️ Core Framework

Fixed, foundational files used at the start of all future projects are located in the `framework/` folder:

* `AGENT_README.md` → detailed explanation for Agent workflow and rules.
* `DOCUMENT_EDITING_GUIDE.md` → explains environment setup, extensions, and maintenance rules for Markdown editing.

---

## 🤖 Agent Workflow

See [`framework/AGENT_README.md`](./framework/AGENT_README.md).

Agents should:

* Ensure required files exist in `docs/`.
* Create missing ones by interviewing the user if needed.
* Keep docs updated and condensed when appropriate.

---

## 🛠️ Editing Environment

See [`framework/DOCUMENT_EDITING_GUIDE.md`](./framework/DOCUMENT_EDITING_GUIDE.md).

Contributors follow this guide to set up VS Code with the required extensions and rules for working on Markdown docs.

---

## 📂 Repo Structure

```bash
README.md                     # This file
framework/
  AGENT_README.md             # Entry point for AI agents
  DOCUMENT_EDITING_GUIDE.md   # Setup and editing guide for contributors
  PROJECT_README.md           # Template for new project READMEs
docs/
  project_mission.md          # describes project goal and intended outcomes
  project_stack.md            # complete tooling for the project with notes
  project_structure.md        #
  project_logs.md             #
  project_considerations.md   #
  ...
```

---

## 🚀 How to Use This Framework

To set up a new project using this documentation framework:

1.  **Integrate the Framework:**
    *   Copy the entire `framework/` directory into your new project's root. This directory contains the `AGENT_README.md` (for AI agents) and `DOCUMENT_EDITING_GUIDE.md` (for human contributors).
    *   **Pro-tip:** Consider adding `framework/` to your `.gitignore` if these are purely templates and you don't want them tracked in your new project's main repository, or if you plan to manage them as a submodule or external dependency.

2.  **Initialize Project Documentation:**
    *   Create a `docs/` directory in your new project's root (if it doesn't already exist).
    *   Fill the `docs/` directory with the required project-specific documentation files: `project_mission.md`, `project_stack.md`, `project_structure.md`, `project_logs.md`, and `project_considerations.md`. You can start with empty files or use templates you define.

3.  **Set up Your Project's `README.md`:**
    *   Copy `framework/PROJECT_README.md` to the root of your new project and rename it to `README.md`.
    *   Open your new `README.md` and fill in the bracketed placeholders (`[YOUR PROJECT TITLE HERE]`, etc.) with your project's specific details.

4.  **Adhere to Standards:**
    *   Ensure your team and any contributing AI agents refer to `framework/DOCUMENT_EDITING_GUIDE.md` for consistent Markdown formatting and style.

This process ensures your new project benefits from a standardized, consistent, and maintainable documentation structure from the start.
