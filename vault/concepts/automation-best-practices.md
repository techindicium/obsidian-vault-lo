---
type: concept
name: "Automation Best Practices"
aliases: ["Automação: Boas Práticas"]
description: "Governance guidance for scheduled AI routines: unowned automations quietly consume compute quota every run even when nobody reads the output."
related_to: ["[[ai-automation-routines]]"]
sources:
  - url: "https://docs.google.com/presentation/d/1TBAMg5BpdXgbZ2pfnHboCW9WP2IpAc5cpZfWw5IaNEs/edit"
    type: "gdoc"
    synced_at: "2026-09-03"
updated_at: "2026-09-03"
updated_by: "preserve@agent"
tags: [type/concept, domain/product]
graphify_node_id: "claude_cowork_workshop_portobank_automacao_boas_praticas"
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Automation Best Practices

> Rule of thumb: if nobody has read the result in the last two weeks, delete the routine.

## Description

An [[ai-automation-routines|automation routine]] without a clear owner wastes compute every day it runs: each scheduled execution consumes the team's quota even when nobody reads the output. The recommended practice is to periodically audit what is scheduled (frequency, recipient), and to delete or pause routines with no recent readership rather than leaving them running by default — recreating a routine later takes only a minute.

## Key Characteristics

- The invisible cost: a forgotten routine runs daily and burns quota for no one
- Review: regularly audit what is scheduled, at what frequency, and for whom
- Clean up: delete or pause unused routines without hesitation — recreation is cheap

## Where it Applies

- Presented as a governance guardrail alongside Automation Routines in Indicium's Claude Cowork enablement workshops (e.g., Portobank, Aug 2026).

## Related Concepts

- [[ai-automation-routines]] — the mechanism this guidance governs

---

## Expected Bidirectional Links

> This section is a reference for agents and can be removed in real pages.

| From | To | Field |
|---|---|---|
| Concept → Concept | `[[ai-automation-routines]]` | "Related Concepts" section |
