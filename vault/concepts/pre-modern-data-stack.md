---
type: concept
name: "Pre-Modern Data Stack"
aliases: ["Pre-Modern Data Stack", "On-Premises Data Era"]
description: "The ~2013 on-premises era constrained by data moats between databases, SQL's inability to handle semi-structured JSON, and a scalability ceiling around 10-100M rows."
related_to: ["[[cloud-data-warehouse]]", "[[data-science-lifecycle]]"]
sources:
  - url: "https://www.iandmacomber.com/blog/post-ai-data-stack"
    type: "remote-binary"
    synced_at: "2026-09-02"
updated_at: "2026-09-02"
updated_by: "preserve@agent"
tags: [type/concept, domain/analytics]
graphify_node_ids: ["post_ai_data_stack_pre_modern_data_stack"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Pre-Modern Data Stack

> Whether American Express cardholders showed different price sensitivity was, in this era, a reasonable question that was simply unanswerable at scale.

## Description

The on-premises era (~2013) confined analysis to single servers with structured data, under three constraints: **data moats** (different business functions on separate databases that couldn't communicate efficiently — cross-database queries needed manual DBA intervention and had no query optimization), **web analytics limitations** (early SQL dialects couldn't natively handle the semi-structured JSON objects that product/web-traffic analytics depend on), and a **scalability ceiling** (queries over roughly 10-100 million rows would fail outright and destabilize shared resources).

## Key Characteristics

- Data moats: siloed databases requiring manual DBA intervention for cross-database queries.
- SQL dialects couldn't natively query semi-structured JSON.
- Hard scalability ceiling around 10-100M rows before queries failed and destabilized shared infrastructure.
- Reasonable business questions were often literally unanswerable at scale.

## Related Concepts

- [[cloud-data-warehouse]] — solved each of these three constraints directly (storage/compute scaling and native JSON support).
- [[data-science-lifecycle]] — this era is the starting point of the lifecycle's bottleneck-removal chain, confined almost entirely to the Data Capture stage.

---

## Expected Bidirectional Links

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[cloud-data-warehouse]]` | "Related Concepts" section |
