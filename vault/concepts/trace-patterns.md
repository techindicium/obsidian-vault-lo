---
type: concept
name: "Trace Patterns"
aliases: ["Trace Patterns", "Evaluation Trace Flow"]
description: "The normalized 5-step trace an agent should follow to answer a data question reliably: READ_DOMAIN_DOC, VIEW_DASHBOARD, READ_SEMANTIC_VIEW, EXECUTE_SQL, SYNTHESIZE_ANSWER."
related_to: ["[[compounding-improvements]]"]
sources:
  - url: "https://www.iandmacomber.com/blog/post-ai-data-stack"
    type: "remote-binary"
    synced_at: "2026-09-02"
updated_at: "2026-09-02"
updated_by: "preserve@agent"
tags: [type/concept, domain/analytics]
graphify_node_ids: ["post_ai_data_stack_trace_patterns"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Trace Patterns

> The intended path a correct answer should follow — not just the correct number, but the correct route to it.

## Description

A named, normalized sequence of steps that a successful agent trace follows when answering a data question:

1. `READ_DOMAIN_DOC` — read the relevant domain documentation first.
2. `VIEW_DASHBOARD` — check the canonical dashboard for the metric in question.
3. `READ_SEMANTIC_VIEW` — consult the semantic layer's definition of the metric.
4. `EXECUTE_SQL` — run the query.
5. `SYNTHESIZE_ANSWER` — assemble the final answer from the above.

Normalizing traces into this vocabulary makes failures comparable across runs: a failed trace usually means one of these steps was skipped (e.g. SQL executed without reading the semantic view first), which is easy to spot and fix once traces share a common shape.

## Key Characteristics

- Five named steps, always in the same order for a well-formed trace.
- Used as the unit of analysis for [[compounding-improvements]] — failures are diagnosed as "skipped step N," not just "wrong answer."
- A correct answer that skips steps (e.g. straight to `EXECUTE_SQL`) is considered fragile — it tends to break when the underlying model changes.

## Related Concepts

- [[compounding-improvements]] — the broader discipline of turning trace failures into durable context fixes; this is the vocabulary it operates on.

---

## Expected Bidirectional Links

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[compounding-improvements]]` | "Related Concepts" section |
