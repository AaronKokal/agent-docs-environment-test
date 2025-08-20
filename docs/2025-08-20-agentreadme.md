---
title: AGENT_README
description: ""
date: 2025-08-20T18:43:38.799Z
preview: ""
draft: true
tags: []
categories: []
---

## 🤖 Agent README

This repository includes a `docs/` folder with files that are **required for every project**.
As an AI agent, your task is to **check for their presence**, **create missing ones**, and **maintain them** over time.

---

## 🔑 Required Docs

The following files must exist in `docs/`:

1. **`project_mission.md`**

   * Purpose: Explain the **why** of the project.
   * Content: Goals, pain points, expected outcomes.
   * Note: This should exist *before* coding begins. If missing, interview the user and create it.

2. **`project_stack.md`**

   * Purpose: Document all **tooling and architecture choices**.
   * Content: Tech stack, frameworks, infra decisions.
   * If missing, gather information from the user and create a first version.

3. **`project_structure.md`**

   * Purpose: Provide a readable **tree view of the repo** with short explanations.
   * Content: Directory tree + comments on what each part is for.
   * Must be kept up to date as the repo evolves.

4. **`project_logs.md`**

   * Purpose: Serve as a **project diary**.
   * Content: Milestones, decisions, problems, reasons behind choices.
   * Maintenance: If the file grows too large, condense redundant entries while preserving timestamps.

5. **`project_considerations.md`**

   * Purpose: Capture **future ideas and alternatives** not pursued right now.
   * Content: Options, trade-offs, deferred decisions, potential pivots.

---

## 📋 Your Responsibilities

* **Check presence**: Ensure all required files are in `docs/`.
* **Create if missing**: If a file doesn’t exist, interview the user (if needed) and create a valid first version.
* **Maintain**: Keep files updated and consistent as the project evolves.
* **Condense**: Periodically review `project_logs.md` and shorten older entries while preserving history.
* **Explain**: Make sure `project_structure.md` always reflects the repo layout with simple explanations.

---

## 📂 Location

All these files live under:

```text
/docs
  project_mission.md
  project_stack.md
  project_structure.md
  project_logs.md
  project_considerations.md
```

---

✅ By following this structure, the project documentation stays consistent, readable, and useful — for both humans and agents.
