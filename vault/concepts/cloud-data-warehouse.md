---
type: concept
name: "Cloud Data Warehouse"
aliases: ["Cloud Data Warehouse", "Cloud DW"]
description: "The ~2016 era (Snowflake, Redshift, BigQuery) that solved infinite storage scaling, horizontal compute scaling, and native semi-structured (JSON) support."
related_to: ["[[modern-data-stack]]", "[[pre-modern-data-stack]]", "[[data-science-lifecycle]]"]
sources:
  - url: "https://www.iandmacomber.com/blog/post-ai-data-stack"
    type: "remote-binary"
    synced_at: "2026-09-02"
updated_at: "2026-09-02"
updated_by: "preserve@agent"
tags: [type/concept, domain/analytics]
graphify_node_ids: ["post_ai_data_stack_cloud_data_warehouse"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Cloud Data Warehouse

> Solved three problems at once: where does all the data live, how fast can we query it, and can it handle JSON.

## Description

Cloud data warehouses — the article cites Snowflake, Redshift, and GCP BigQuery as the examples — solved three problems that had capped the [[pre-modern-data-stack]] era: infinite storage scaling (all organizational data consolidated into one accessible repository), horizontal compute scaling (analytical queries separated from production workloads, so a big query no longer destabilized the systems running the business), and native semi-structured support (JSON became queryable and mainstream, unblocking product/web-analytics questions that earlier SQL dialects couldn't touch).

This expansion let data professionals answer questions that had previously been impossible even to pose.

## Key Characteristics

- Infinite storage scaling — no more per-database silos.
- Horizontal compute scaling — analytics no longer contends with production for resources.
- Native JSON/semi-structured support — mainstreamed product and web-analytics queries.
- Representative vendors named in the source: Snowflake, Redshift, GCP BigQuery.

## Related Concepts

- [[pre-modern-data-stack]] — the era this one directly replaced, and whose three constraints (data moats, JSON limits, scalability ceiling) it solved one-for-one.
- [[modern-data-stack]] — built on top of the warehouse this era established.
- [[data-science-lifecycle]] — this era solved data accessibility, which created the next scarcity: analytical capacity.

---

## Expected Bidirectional Links

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[pre-modern-data-stack]]`, `[[modern-data-stack]]`, `[[data-science-lifecycle]]` | "Related Concepts" section |
