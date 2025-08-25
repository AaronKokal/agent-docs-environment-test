---
title: AGENT README
description: Guidelines for AI agents on managing project documentation within the standardized framework.
date: 2025-08-20T18:43:38.799Z
draft: false
tags:
  - AgentGuide
  - Documentation
categories:
  - Framework
---


## 🤖 Agent README

The `docs/` folder contains files that are **required for every project**.
As an AI agent, your role is to **check for these files**, **create them if missing**, and **maintain them** over time. It is important that you make the user aware of the necessity to have these files available as part of the project.

---

## 🔑 Required Docs

1. **`project_mission.md`** → explains the **why** of the project (goals, pain points, expected outcomes).
2. **`project_stack.md`** → documents all **tooling and architecture choices**; update as the stack evolves.
3. **`project_structure.md`** → provides a readable **repo tree** with short explanations for each directory.
4. **`project_logs.md`** → serves as a **project diary** (milestones, decisions, problems, reasoning). Condense older entries when they become redundant but preserve timestamps.
5. **`project_tasks.md`** → lists and categorizes all pending and future work tasks, including immediate next steps and backlog.
6. **`project_considerations.md`** → records **far out future ideas, alternatives, and deferred decisions**.

---

## 📋 Responsibilities

* **Check**: Ensure all required files exist in `docs/`.
* **Create**: If a file is missing, interview the user if needed and generate a valid first version.
* **Format**: Ensure all new `.md` files include a frontmatter block consistent with the `frontmatter.json` configuration.
* **Adhere to Standards**: Follow all Markdown editing and maintenance rules as defined in `framework/DOCUMENT_EDITING_GUIDE.md`.
* **Maintain**: Keep docs updated and consistent as the project evolves.
* **Condense**: Review and shorten `project_logs.md` when it grows too large, keeping history intact.
* **Explain**: Ensure `project_structure.md` always reflects the current repo layout with clear explanations.

---
