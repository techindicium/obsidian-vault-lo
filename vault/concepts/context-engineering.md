---
type: concept
name: "Context Engineering"
aliases: ["Context Engineering"]
description: "The practice of supplying an AI agent with a clear objective, data sources, evaluation criteria, and output format up front so it produces a usable result on the first pass."
related_to: ["[[claude-cowork-interaction-model]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-03"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_context_engineering"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Context Engineering

> Response quality starts with the request.

## Description

An AI agent works with whatever context it is given. A vague request (e.g., "make a sales report" with no period, data source, or format) forces the agent to guess, producing a generic result and multiple rounds of rework. A request that states the objective, the data sources, the evaluation criteria, and the desired output format up front (e.g., "using the spreadsheets in /closing, build June's closing report for the South region, following the bank's template, and flag variances over 5% vs. May in a .docx with an executive summary") is typically ready for review on the first pass. Good context = a clear objective + where the data lives + the analysis criteria + the delivery format.

## Key Characteristics

- Vague requests force the agent to guess and produce generic, low-value output
- Explicit objective + data source + criteria + format sharply reduces rework
- Applies to any agentic request, not only document generation

## Where it Applies

- Taught as the foundational skill before Skills/Connectors/Automation in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026), contrasting a vague vs. a well-specified request.

## Related Concepts

- [[claude-cowork-interaction-model]] — the interaction model whose output quality depends most directly on this practice

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[claude-cowork-interaction-model]]` | "Related Concepts" section |
