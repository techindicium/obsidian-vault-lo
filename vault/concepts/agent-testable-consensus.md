---
type: concept
name: "Agent-Testable Consensus"
aliases: ["Agent-Testable Consensus", "Consensus Engineering", "Consensus Divergence Rate"]
description: "Treating organizational agreement on a metric as an engineerable, measurable property, tracked via a Consensus Divergence Rate across interfaces and models."
related_to: ["[[post-ai-data-stack]]", "[[semantic-layers]]", "[[compounding-improvements]]"]
sources:
  - url: "https://www.iandmacomber.com/blog/post-ai-data-stack"
    type: "remote-binary"
    synced_at: "2026-09-02"
updated_at: "2026-09-02"
updated_by: "preserve@agent"
tags: [type/concept, domain/analytics]
graphify_node_ids: ["post_ai_data_stack_agent_testable_consensus"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Agent-Testable Consensus

> Consensus used to emerge from org structure and scarcity. Now that dashboards cost nothing to create, consensus itself is the scarce resource — so it has to be engineered and measured directly.

## Description

Pre-AI, consensus was a side effect of scarcity: building a dashboard took real resources, so an org's BI folder structure implicitly mirrored its priorities (nested folders mimicking the org chart). That dynamic has inverted — creating a dashboard now costs almost nothing, so every stakeholder can slice the same question differently and land on a different answer.

The framework proposes making consensus **testable**:

1. Extract the metrics used in recent board presentations.
2. Query each metric through every interface/model combination available (coding agents, direct SQL, BI tools, conversational interfaces).
3. Count how many distinct answers come back.
4. When answers diverge, debug the discrepancy and iterate on the underlying context.

Success is when interface or tool choice stops changing the answer or the reasoning path. Organizations should track a **Consensus Divergence Rate** — the percentage of questions that yield different answers depending on the interface used — and drive it toward zero for board and executive materials.

## Key Characteristics

- Consensus is measured, not assumed: query the same metric across every surface and count the distinct answers.
- **Consensus Divergence Rate**: the named metric for this — % of questions with inconsistent answers across interfaces.
- Achieving it depends on [[compounding-improvements]] — systematic evaluation compounds the context needed to close divergence.

## Related Concepts

- [[post-ai-data-stack]] — one of the stack's six named components; this one and [[compounding-improvements]] are framed as its "operating disciplines" half.
- [[semantic-layers]] — a strong semantic layer is the concrete asset that keeps answers consistent across interfaces, directly lowering the divergence rate.
- [[compounding-improvements]] — the mechanism for actually reducing divergence once it's measured.

---

## Expected Bidirectional Links

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[post-ai-data-stack]]`, `[[semantic-layers]]`, `[[compounding-improvements]]` | "Components" / "Related Concepts" |
