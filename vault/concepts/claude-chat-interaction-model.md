---
type: concept
name: "Claude Chat (2023 Interaction Model)"
aliases: ["Chat (2023)", "Chat-mode AI"]
description: "The 2023-era AI interaction model: a conversational interface where the user asks and the AI answers, and the human does all the execution."
related_to: ["[[claude-code-interaction-model]]", "[[claude-cowork-interaction-model]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-03"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_chat_2023"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Claude Chat (2023 Interaction Model)

> Ask questions, get answers, do the work yourself.

## Description

The first stage in the evolution of AI-at-work interaction models. In Chat mode, the user has a single conversation at a time, asks questions, receives answers, and must manually copy results and gather context themselves. The AI does not act on external systems or files — it only responds.

## Key Characteristics

- One conversation at a time, no persistent multi-step execution
- User manually copies and pastes outputs between tools
- Context must be gathered and provided by hand for every request

## Where it Applies

- Baseline stage referenced in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026) to contrast with later, more autonomous interaction models.

## Related Concepts

- [[claude-code-interaction-model]] — the next stage, where developers gained execution capability beyond Q&A
- [[claude-cowork-interaction-model]] — the stage where all functions (not just developers) gain the same execution power

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[claude-code-interaction-model]]` | "Related Concepts" section |
