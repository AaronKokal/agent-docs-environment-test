---
title: Project Stack
description: Documents all tooling and architecture choices for this project.
date: 2025-08-25T17:59:07Z
draft: false
tags:
  - Project
  - Stack
  - Architecture
categories:
  - Documentation
---

## Project Stack

This document outlines the key technologies, tools, and architectural decisions relevant to this **Documentation Framework Repository** itself.

## Technologies/Languages

* **Markdown**: Primary language for all documentation files.
* **YAML**: Used for frontmatter in Markdown files and configuration files.
* **Bash/Shell**: For scripting and command-line operations (e.g., `mkdir`, `mv`).

## Frameworks/Libraries

* **Front Matter (VS Code Extension/Schema)**: Used for managing metadata in Markdown files.
* **Prettier**: Code formatter for consistent styling of Markdown and other files.
* **Markdownlint**: Linter for enforcing Markdown style and best practices.

## Design Principles

* **Separation of Concerns**: Differentiating between framework templates (`framework/`) and project-specific documentation (`docs/`).
* **Single Source of Truth**: Minimizing redundant information by referencing primary documents (e.g., `README.md` references guides in `framework/`).
* **Agent-Friendly**: Documentation is designed to be easily parsed and maintained by AI agents.
* **Human-Readable**: Prioritizing clarity and ease of understanding for human contributors.
* **Extensible**: Designed to be easily adaptable and expandable for future needs.

## Architecture Decisions

* **Directory Structure**: Deliberate separation of `framework/` (templates) and `docs/` (project-specific living documents).
* **Frontmatter Standard**: Adherence to a consistent frontmatter schema across all Markdown files for metadata management.
* **Linting & Formatting**: Enforcement through `.markdownlint.json` and `.prettierrc` to maintain quality and consistency.
