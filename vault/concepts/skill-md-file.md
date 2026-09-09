---
type: concept
name: "SKILL.md"
aliases: ["SKILL.md file"]
description: "The file format that defines a Skill's rules, process, and best practices, loaded by an agent into its context when triggered."
related_to: ["[[agentic-skills]]", "[[skill-trigger-mechanism]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-03"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_skill_md"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# SKILL.md

> The instructions file: rules, process, and best practices for one task.

## Description

SKILL.md is the concrete artifact behind a [[agentic-skills]]: a file containing the step-by-step process, rules, and best practices for a specific task. When an agent's trigger mechanism matches a request to a Skill, it loads that Skill's SKILL.md into its working context before executing.

## Key Characteristics

- Holds the step-by-step process and best practices for one task
- Loaded into the agent's context only when the matching Skill is triggered
- Paired with supporting resources (templates, examples, scripts) referenced from it

## Where it Applies

- Documented as the concrete mechanism behind Skills in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026).

## Related Concepts

- [[agentic-skills]] — the reusable capability this file defines
- [[skill-trigger-mechanism]] — the process that decides when to load this file

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[agentic-skills]]` | "Related Concepts" section |
