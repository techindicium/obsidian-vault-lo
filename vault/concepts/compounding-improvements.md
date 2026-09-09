---
type: concept
name: "Compounding Improvements"
aliases: ["Compounding Improvements", "Eval-Driven Context Hardening"]
description: "Using evaluation traces and failure taxonomies to durably fix foundational context gaps, instead of waiting on frontier models to compensate for them."
related_to: ["[[post-ai-data-stack]]", "[[trace-patterns]]", "[[agent-testable-consensus]]"]
sources:
  - url: "https://www.iandmacomber.com/blog/post-ai-data-stack"
    type: "remote-binary"
    synced_at: "2026-09-02"
updated_at: "2026-09-02"
updated_by: "preserve@agent"
tags: [type/concept, domain/analytics]
graphify_node_ids: ["post_ai_data_stack_compounding_improvements"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Compounding Improvements

> A correct answer reached through improvised logic is worth less than a correct answer reached through a trusted, repeatable process — the improvised path breaks the moment the model changes.

## Description

Evaluation traces reveal more than a correct/incorrect verdict. Failed queries typically skip required documentation, pick the wrong table, or apply the wrong filter; successful traces show the intended path — reading domain docs, consulting semantic views, navigating canonical dashboards (see [[trace-patterns]]).

The recommended discipline: normalize trace patterns, snapshot system state alongside every run, build "failure taxonomies" out of recurring eval breakdowns, and update context specifically to close those recurring gaps. This treats context-hardening as compounding capital — rather than waiting for the next frontier model release to paper over a persistent problem, the org fixes the underlying gap once and every future run benefits.

## Key Characteristics

- Traces are normalized into named steps (see [[trace-patterns]]) so failures are comparable across runs.
- **Failure taxonomies** categorize recurring breakdown modes (wrong table, skipped doc, bad filter, etc.).
- The goal is durability: fixes should survive a model swap, not just patch one bad run.
- Feeds directly into [[agent-testable-consensus]] — this is the mechanism for actually closing a measured divergence.

## Related Concepts

- [[post-ai-data-stack]] — one of the stack's six named components.
- [[trace-patterns]] — the concrete 5-step trace vocabulary this discipline is built on.
- [[agent-testable-consensus]] — the measurement this discipline is meant to improve.

---

## Expected Bidirectional Links

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[post-ai-data-stack]]`, `[[trace-patterns]]`, `[[agent-testable-consensus]]` | "Components" / "Related Concepts" |
