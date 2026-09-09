---
type: concept
name: "Automation Routines (Scheduled AI Tasks)"
aliases: ["Automação (Rotinas)", "AI routines"]
description: "A task scheduled once that an AI agent then executes on its own, at a frequency the user defines, without further manual intervention."
related_to: ["[[automation-best-practices]]", "[[scheduled-task-command]]", "[[claude-cowork-interaction-model]]", "[[compound-effect-ai]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-03"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_automacao_rotinas"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Automation Routines (Scheduled AI Tasks)

> A routine = a scheduled task: from a daily reminder to a report that assembles itself.

## Description

A routine follows a three-step loop: the user schedules it by describing what to do and when ("every Monday at 8am, put together this week's report"); the agent then executes the full flow on its own — pulling data, analyzing it, and producing the deliverable; the user only reviews the result and approves, adjusts, or sends it. This turns a previously manual, recurring task into a self-running one.

## Key Characteristics

- Scheduled once, in plain language, with a defined frequency
- Executes end-to-end without further manual steps once triggered
- Produces a deliverable that only needs human review before use

## Where it Applies

- Demonstrated live in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026) with a routine that pulls data from Drive/SharePoint, drafts a Word report, and prepares an email draft every Monday.

## Related Concepts

- [[automation-best-practices]] — governance practices for routines to avoid wasted token spend
- [[scheduled-task-command]] — the concrete command used to create a routine
- [[compound-effect-ai]] — how routines compound with Connectors and Context to keep producing value continuously

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[automation-best-practices]]` | "Related Concepts" section |
