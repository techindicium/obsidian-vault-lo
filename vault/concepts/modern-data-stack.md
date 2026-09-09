---
type: concept
name: "Modern Data Stack"
aliases: ["Modern Data Stack", "MDS"]
description: "The ~2020 era of managed ETL (e.g. Fivetran) plus Reverse ETL, which democratized data-source access and enabled operational impact."
related_to: ["[[reverse-etl]]", "[[cloud-data-warehouse]]", "[[data-science-lifecycle]]", "[[post-ai-data-stack]]"]
sources:
  - url: "https://www.iandmacomber.com/blog/post-ai-data-stack"
    type: "remote-binary"
    synced_at: "2026-09-02"
updated_at: "2026-09-02"
updated_by: "preserve@agent"
tags: [type/concept, domain/analytics]
graphify_node_ids: ["post_ai_data_stack_modern_data_stack"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Modern Data Stack

> Before: adding a new data source meant an engineering team building a custom pipeline. After: a data professional clicks a button and pays a subscription.

## Description

By 2020, managed ETL services (the article names Fivetran as the example) let data professionals add new sources independently, without engineering building a bespoke pipeline for each one. [[reverse-etl]] closed the loop in the other direction: instead of insights disappearing into a presentation deck, they could flow automatically back into operational systems — a price-sensitivity finding could trigger a product change or a personalized customer experience directly.

Together, managed ETL and Reverse ETL democratized data access and operational impact at the same time — the defining shift of this era.

## Key Characteristics

- Managed ETL (e.g. Fivetran) removes engineering as the bottleneck for adding a new source.
- [[reverse-etl]] pushes insights back into operational systems instead of ending in a deck.
- Marks the era where data professionals gained *and* operational impact simultaneously, rather than one at a time.

## Related Concepts

- [[cloud-data-warehouse]] — the immediate predecessor era; this stack is built on top of the warehouse it enabled.
- [[reverse-etl]] — the specific technique that gives this era its operational-impact half.
- [[data-science-lifecycle]] — this era solved analytical capacity, which created the next scarcity: operator capability.
- [[post-ai-data-stack]] — the era that immediately follows; it solved dashboard/query creation, the bottleneck this era's tooling still left in place.

---

## Expected Bidirectional Links

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[reverse-etl]]`, `[[cloud-data-warehouse]]`, `[[data-science-lifecycle]]` | "Related Concepts" section |
