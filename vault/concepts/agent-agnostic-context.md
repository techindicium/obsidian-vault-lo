---
type: concept
name: "Agent-Agnostic Context"
aliases: ["Agent-Agnostic Context", "Headless Semantic Context"]
description: "Keeping data semantics and context headless and portable across interfaces and models, instead of locking them into one vendor's proprietary system."
related_to: ["[[post-ai-data-stack]]", "[[semantic-layers]]"]
sources:
  - url: "https://www.iandmacomber.com/blog/post-ai-data-stack"
    type: "remote-binary"
    synced_at: "2026-09-02"
updated_at: "2026-09-02"
updated_by: "preserve@agent"
tags: [type/concept, domain/analytics]
graphify_node_ids: ["post_ai_data_stack_agent_agnostic_context"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Agent-Agnostic Context

> The same data question should get the same answer whether asked through a coworker, a coding agent, a BI tool, or a Slack bot.

## Description

Some post-AI vendors push complete lock-in — migrate every semantic layer, model, dashboard, and user into their proprietary system. This eliminates optionality and creates dependencies an org can't easily unwind. The alternative is keeping context **headless and portable**: avoid proprietary data languages, keep answers consistent across every interface, and build infrastructure that isn't tied to any single vendor's UI. Model preferences, interfaces, and tool choices shift quarterly — the infrastructure underneath should not have to move with them.

## Key Characteristics

- No proprietary data languages or locked-in contexts.
- Consistency of answers across interfaces is a design requirement, not a nice-to-have.
- Infrastructure is built to outlast any single vendor's tool or model choice.

## Related Concepts

- [[post-ai-data-stack]] — the third of the four infrastructure components.
- [[semantic-layers]] — a strong semantic layer is the concrete mechanism that keeps context agent-agnostic; without it, direct agent-to-raw-data connections fragment into inconsistent answers.

---

## Expected Bidirectional Links

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[post-ai-data-stack]]`, `[[semantic-layers]]` | "Components" / "Related Concepts" |
