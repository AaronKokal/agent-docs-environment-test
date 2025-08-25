---
title: Project Structure
description: Provides a readable repository tree with short explanations for each directory.
date: 2025-08-25T17:59:23Z
draft: false
tags:
  - Project
  - Structure
  - Files
categories:
  - Documentation
---

## Project Structure

This document outlines the file and directory structure for this **Documentation Framework Repository**.

```text
.
├── frontmatter.json                  # Front Matter extension configuration for MD files
├── LICENSE                           # Project license
├── README.md                         # Main repository README (this file describes the framework)
├── .frontmatter/                     # Front Matter extension internal files
├── .git/                             # Git repository data
├── .vscode/                          # VS Code workspace settings
├── docs/                             # Project-specific documentation (living documents)
│   ├── project_mission.md            # Defines the project's goals, pain points, and outcomes
│   ├── project_stack.md              # Documents tooling and architecture decisions
│   ├── project_structure.md          # This file, describes current repo structure
│   ├── project_logs.md               # Project diary with milestones and decisions
│   ├── project_tasks.md              # Lists all pending and future tasks
│   └── project_considerations.md     # Future ideas, alternatives, and deferred decisions
└── framework/                        # Core framework templates (fixed documents)
    ├── AGENT_README.md               # Instructions for AI agents
    ├── DOCUMENT_EDITING_GUIDE.md     # Guide for Markdown editing standards
    ├── MIGRATION_GUIDE.md            # Guide for agents to migrate documentation
    └── PROJECT_README.md             # Template for a new project's README
```

## Directory Explanations

* `.`: The root directory of the repository.
* `frontmatter.json`: Configuration file for the Front Matter VS Code extension, defining the schema for Markdown frontmatter.
* `LICENSE`: Contains the licensing information for the project.
* `README.md`: The main entry point for the repository, explaining the documentation framework itself and how to use it.
* `.frontmatter/`: Internal directory used by the Front Matter VS Code extension.
* `.git/`: Standard Git directory for version control.
* `.vscode/`: Contains VS Code workspace-specific settings and recommendations.
* `docs/`: This directory houses the "living documents" for a project. These files are updated and grow as the project evolves. In this framework repository, these files are examples of what would be found in a project adopting the framework.
* `framework/`: This directory contains the "fixed" or "template" documentation files. These are designed to be copied into the root or `docs/` folder of a new project when adopting the framework. They include essential guides and instructions for both human contributors and AI agents.
