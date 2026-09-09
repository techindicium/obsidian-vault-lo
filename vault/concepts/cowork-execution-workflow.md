---
type: concept
name: "Cowork Execution Workflow (Understand-Plan-Execute-Verify-Deliver)"
aliases: ["Fluxo Entender-Planejar-Executar-Verificar-Entregar", "Cowork 5-step loop"]
description: "The five-step internal loop an agentic AI follows when operating autonomously: understand, plan, execute, verify, and deliver."
related_to: ["[[claude-cowork-interaction-model]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-03"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_cowork_workflow"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Cowork Execution Workflow (Understand-Plan-Execute-Verify-Deliver)

> And the AI pushes back: it asks hard questions, flags risks you didn't ask about, and doesn't just tell you you're right.

## Description

The internal loop an agent like [[claude-cowork-interaction-model|Claude Cowork]] follows once given a goal: (1) Understand — asks clarifying questions; (2) Plan — breaks the work into tasks; (3) Execute — acts across tools, files, and the web; (4) Verify — checks quality and accuracy; (5) Deliver — produces a result ready to share. Distinct from a passive assistant, the agent also questions the user's framing rather than simply agreeing.

## Key Characteristics

- Five explicit stages: Understand, Plan, Execute, Verify, Deliver
- Includes a verification step before delivery, not just execution
- The agent is expected to challenge assumptions and surface unrequested risks

## Where it Applies

- Presented as "how Claude Cowork works" in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026).

## Related Concepts

- [[claude-cowork-interaction-model]] — the interaction model that runs this workflow

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[claude-cowork-interaction-model]]` | "Related Concepts" section |
