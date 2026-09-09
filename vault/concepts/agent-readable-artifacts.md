---
type: concept
name: "Agent-Readable Artifacts"
aliases: ["Agent-Readable Artifacts", "LLM-Optimized Data Products"]
description: "Designing data outputs — dashboards, docs, queries — for algorithmic/agent consumption first, human consumption second."
related_to: ["[[post-ai-data-stack]]", "[[agent-operable-tools]]"]
sources:
  - url: "https://www.iandmacomber.com/blog/post-ai-data-stack"
    type: "remote-binary"
    synced_at: "2026-09-02"
updated_at: "2026-09-02"
updated_by: "preserve@agent"
tags: [type/concept, domain/analytics]
graphify_node_ids: ["post_ai_data_stack_agent_readable_artifacts"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Agent-Readable Artifacts

> Data outputs built to be decomposed and reassembled by agents, not just viewed by humans.

## Description

Dashboards stop being the endpoint. Instead they become repositories of facts and explanations that agents parse, extract from, and recombine — the same way audiences increasingly encounter Saturday Night Live through algorithmically-surfaced clips rather than the full broadcast. By 2027, the framework predicts executives will learn about product launches through agents scanning dashboards weekly, never opening them manually.

This requires data products optimized for LLM comprehension: machine-readable dashboard descriptions (markdown-based `llms.txt` files), clear provenance linking models/code/business context, and cached values plus executable SQL alongside the visual layer. The comparison to SEO is deliberate — teams must ensure their work surfaces when agents go looking for relevant information, the same discipline as ranking for a search query.

## Key Characteristics

- Machine-readable descriptions (e.g. `llms.txt`) sit alongside the human-facing dashboard.
- Provenance is explicit: which model, which code, which business context produced this number.
- Cached values and executable queries are exposed, not just rendered charts.
- The "SEO for agents" framing: discoverability by an agent is now a design requirement, not an afterthought.

## Related Concepts

- [[post-ai-data-stack]] — this is one of the four infrastructure components the stack requires.
- [[agent-operable-tools]] — readable artifacts are the data side of the same shift; operable tools are the action side.

---

## Expected Bidirectional Links

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[post-ai-data-stack]]` | "Components" section of post-ai-data-stack |
