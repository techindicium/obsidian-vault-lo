---
type: concept
name: "Beyond SQL"
aliases: ["Beyond SQL", "Structured Extraction for Narrative Questions"]
description: "Handling narrative, unstructured business questions by pre-processing unstructured data once into structured fields, instead of forcing users into SQL-shaped phrasing."
related_to: ["[[post-ai-data-stack]]", "[[semantic-layers]]"]
sources:
  - url: "https://www.iandmacomber.com/blog/post-ai-data-stack"
    type: "remote-binary"
    synced_at: "2026-09-02"
updated_at: "2026-09-02"
updated_by: "preserve@agent"
tags: [type/concept, domain/analytics]
graphify_node_ids: ["post_ai_data_stack_beyond_sql"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Beyond SQL

> SQL is excellent at numerical aggregation and useless at "why are we losing construction deals?"

## Description

SQL falters on narrative questions — "why" and "what's our north star" don't reduce cleanly to aggregation. As agent-first workflows spread, stakeholders will ask an increasingly diverse mix of question types, and training everyone to phrase questions in "SQL-shaped" language doesn't scale.

The proposed fix mirrors data modeling but targets *meaning* rather than *shape*: pre-process unstructured data once, offline and cheaply, and write structured outputs back into the same organized models used for structured data. For sales call transcripts, that means extracting fields like `loss_reason`, `objection_type`, and `mentioned_competitor` — the same normalization discipline already applied to card transaction data, just aimed at text instead of numbers.

## Key Characteristics

- One-time, offline, cheap pre-processing of unstructured sources (call transcripts, tickets, notes).
- Extracted fields (`loss_reason`, `objection_type`, etc.) live in the same structured models as numerical data.
- Infrastructure handles both structured and unstructured questions through one consistent entry point, rather than training users to think in SQL.

## Related Concepts

- [[post-ai-data-stack]] — one of the stack's six named components.
- [[semantic-layers]] — the structured outputs from this extraction step become part of the same semantic layer that grounds numerical questions.

---

## Expected Bidirectional Links

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[post-ai-data-stack]]`, `[[semantic-layers]]` | "Components" / "Related Concepts" |
