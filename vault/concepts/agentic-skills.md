---
type: concept
name: "Skills (Agentic AI)"
aliases: ["Skills", "AI Skills"]
description: "A package of instructions that teaches an AI agent to perform a task the way a specific person or team wants it done, created once and reused by everyone."
related_to: ["[[skill-md-file]]", "[[skill-trigger-mechanism]]", "[[skills-layered-model]]", "[[ai-plugins]]", "[[claude-cowork-interaction-model]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-03"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_skills"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Skills (Agentic AI)

> Think of a Skill as a "recipe" the AI knows how to read and execute.

## Description

A Skill packages instructions, best practices, and templates for a recurring task so it produces a consistent result every time it is invoked — by anyone on the team, with a single natural-language request. It is created once (by a person, a team, or an organization) and then reused indefinitely, avoiding the need to re-explain the task each time.

## Key Characteristics

- Defined in a [[skill-md-file]] containing the step-by-step process and best practices
- Bundles reusable resources (templates, golden examples, scripts) that guarantee output quality
- Invoked with a plain-language request rather than a technical command

## Where it Applies

- Taught as the core reuse mechanism in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026), layered across individual, team, and organization scopes.

## Related Concepts

- [[skill-md-file]] — the file format that defines a Skill
- [[skill-trigger-mechanism]] — how the AI decides which Skill to load for a given request
- [[skills-layered-model]] — how Skills are personalized across you, your team, and your organization
- [[ai-plugins]] — Skills combined with Connectors into a one-click installable bundle

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[skill-md-file]]` | "Related Concepts" section |
| Concept → Concept | `[[ai-plugins]]` | "Related Concepts" section |
