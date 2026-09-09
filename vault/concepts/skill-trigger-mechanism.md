---
type: concept
name: "Skill Trigger Mechanism"
aliases: ["Skill triggering", "Mecanismo de Acionamento de Skills"]
description: "The process by which an agent matches a user's natural-language request to the right Skill, loads its SKILL.md, and executes it."
related_to: ["[[agentic-skills]]", "[[skill-md-file]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-03"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_skill_trigger_mechanism"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Skill Trigger Mechanism

> You write in plain words, the AI finds the Skills it needs.

## Description

A four-step process: (1) the user sends a request containing trigger words (e.g., "put together a presentation with this quarter's results"); (2) the agent matches keywords in the message against known Skill triggers (e.g., "presentation" matches a pptx-building Skill); (3) it loads that Skill's [[skill-md-file]] into context, reading its best practices, tools, and flows; (4) it executes following the Skill's instructions to produce the deliverable.

## Key Characteristics

- Keyword/intent matching against a message, not an explicit command
- Loads only the matched Skill's instructions into context, not all Skills at once
- Falls through to normal agent behavior when no Skill trigger matches

## Where it Applies

- Explained step-by-step in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026) using a "build a presentation" example.

## Related Concepts

- [[agentic-skills]] — the capability this mechanism activates
- [[skill-md-file]] — the file loaded once a match is found

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[agentic-skills]]` | "Related Concepts" section |
